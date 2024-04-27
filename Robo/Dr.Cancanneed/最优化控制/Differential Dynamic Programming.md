DDP。这是为了解决非线性轨迹优化问题，即：Nonlinear trajectory optimization. 这个问题是指，当我们想控制系统从一个状态到另一个状态，我们希望整个过程中系统状态沿着特定的轨迹做转移。这条轨迹也提供了我们代价函数中的参考值。
# 轨迹优化问题
一个标准的轨迹优化问题可以写成以下形式：
$$
\begin{align}
\min_{x:N,u:N-1}J &= \sum_{n=1}^{N-1}l_n(x_n,u_n) + l_{N}(x_N) \\
s.t. \ x_{n+1} &= f(x_n,u_n) \\
x_n &\in \mathcal{X}_n \\
u_n &\in \mathcal{U}_n \\
\end{align}
$$
这里代价函数不需要是 Convex 的但是在实际情况中我们 90% 会采用二次型形式的代价函数。我们的状态转移关系也不一定得是线性的，约束不一定是 Convex 的。总之这里的约束非常的少。
为了后续的计算，我们需要假设我们的代价函数和约束都是 $\mathcal{C}^2$ 。
# DDP 方法介绍
- 用 DP 来慢慢近似一条最优轨迹
- 用 Cost-to-go Function 的二阶泰勒展开对其进行近似并使用牛顿法进行优化
- 收敛非常的快啊（大概因为牛顿法是种二阶方法）
## 原理
- Cost-to-go expansion
$$
\begin{align}
V_N (x + \Delta x) &\simeq V_N (x) + p_n^{\top} \Delta x + \frac{1}{2}\Delta x ^{\top} P_n \Delta x \\
p_n &= \nabla_x l_n(x) \\
P_n &= \nabla^2_{xx} l_n(x)
\end{align}
$$
- Action-Value Function expansion
$$
Q_N(x + \Delta x, u + \Delta u) \simeq Q_N(x, u) + 
\begin{bmatrix}
g_x \\
g_y
\end{bmatrix}^{\top}
\begin{bmatrix}
\Delta x \\
\Delta u
\end{bmatrix}
+
\frac{1}{2}
\begin{bmatrix}
\Delta x \\
\Delta u
\end{bmatrix}^{\top}
\begin{bmatrix}
G_{xx} & G_{xu} \\
G_{ux} & G_{uu}
\end{bmatrix}
\begin{bmatrix}
\Delta x \\
\Delta u
\end{bmatrix}
$$
- Bellman Equation
我们利用贝尔曼最优性来求出新的 Value-Function
$$
V_{N-1}(x) = \min_{\Delta u} [Q(x, u) + g_x^{\top}\Delta x + g_u^{\top}\Delta u + \frac{1}{2} \Delta x^{\top}G_{xx}\Delta x + \frac{1}{2} \Delta u^{\top}G_{uu}\Delta u + \frac{1}{2} \Delta x^{\top}G_{xu}\Delta u + \frac{1}{2} \Delta u^{\top}G_{ux}\Delta x]
$$
这是一个二次型，为了求其最小值，我们需要求它的导数为 0 的点：
$$
\Delta V_{N-1} = g_u + G_{uu} \Delta u + G_{ux} \Delta x = 0
$$
我们可以得出一个线性反馈：
$$
\begin{align}
\Delta u_{N-1} &= -G_{uu}^{-1}g_u - G_{uu}^{-1}G_{ux} \Delta x \\
&= -d_{N-1} - K_{N-1}\Delta x
\end{align}
$$
- 将 $\Delta u$ 回带入 $Q_{N-1}(x + \Delta x, u + \Delta u)$ 去获得 $V_{N-1}(x + \Delta x)$
$$
V_{N-1}(x + \Delta x) \simeq \cdots
$$
得出：
$$
P_{N-1} = G_{xx} + K_{N-1}^{\top}G_{uu}K_{N-1} - G_{xu}K_{N-1} - K_{N-1}^{\top}G_{ux}
$$
$$
p_{N-1} = g_x - K_{N-1}^{\top}g_u + K_{N-1}^{\top} G_{uu} d_{N-1} - G_{xu}d_{N-1}
$$
## 算法实现
- Forward Rollout
```
deltaJ = 0
x1' = x1
for k = 1:N-1
	uk' = uk - adk - Kk*(xk' - xk)
	xk+1' = f(xk', uk')
	deltaJ = deltaJ + ag_uu^Tdk
end
```
- Line search
```
a = 1
do:
	x',u',deltaJ = rollout(x,u,d,k,a)
	a = ca
while J(x',u') > J(x,u) - b * deltaJ
```
- Repeat
```
until $|d|_{\infty} < tol$
```
