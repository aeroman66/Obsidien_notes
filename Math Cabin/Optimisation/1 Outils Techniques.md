主要介绍这门课用到的一些数学工具，涵盖了线性代数、拓扑、微分和凸分析等。
# 线性代数
- 正定矩阵
正定性是一个复数矩阵的性质，而不是一个函数的二次偏导的性质。
# 拓扑
- 开闭集
- 领域
- 有限集合
- 强制泛函
函数在无穷远处必须趋向于正无穷：
$$
\lim_{\| x \|\rightarrow +\infty,x\in A}f(x) = +\infty
$$
# 微分
- 偏导
$$
\frac{\partial f}{\partial x_{j}},\partial_{i}f
$$
	- 方向导数
- 可微方程
Fonction différentiable et différentielle
一个方程在 $x_{0}$ 上被称作可微的如果存在一个线性映射 $df_{x_{0}}$，使得：
$$
f(x_{0} + h) = f(x_{0}) + df_{x_{0}}(h) + o_{h\rightarrow 0_{\mathbb{R}^{n}}}(\| h \|)
$$
这个线性映射称作这个方程在 $x_{0}$ 上的微分。我们再看一下微分和导数之间的关系：
$$
f(x_{0} + h) = f(x_{0}) + f'(x_{0})h + o_{h\rightarrow 0}(h)
$$
所以说：
$$
df_{x_{0}}(h) = f'(x_{0})h, df_{x_{0}}(1) = f'(x_{0})
$$
对于一个多元函数来说，$h \in \mathbb{R}^{n}$ ：
$$
df_{x_{0}} : h \longmapsto \sum_{j=1}^{n}\partial_{i}f(x_{0})h_{j}
$$
- 梯度
$$
\nabla f(a) =
\begin{bmatrix}
\frac{\partial f}{\partial x_{1}}(a) \\
\frac{\partial f}{\partial x_{2}}(a) \\
\vdots \\
\frac{\partial f}{\partial x_{n}}(a) \\
\end{bmatrix}
$$
- 微分和梯度之间的关系
$$
df_{x_{0}}(h) = <\nabla f(x_{0}),h>
$$
- 雅可比矩阵
- 海森矩阵
Soit $x_{0} \in \mathbb{R}^{n},f:\mathbb{R}^{n}\rightarrow \mathbb{R}$:
$$
H_{f}(x_{0}) = \left[ \frac{\partial^{2}f}{\partial x_{i}\partial x_{j}} \right]_{(i,j)\in [| 1,n |]^{2}} \in \mathcal{M}_{n,n}(\mathbb{R})
$$
- Developpement limite
$$
f(x_{0} + h) = f(x_{0}) + df_{x_{0}}(h) + o(\| h \|)
$$
$$
f(x_{0} + h) = f(x_{0}) + <\nabla f(x_{0}),h>  + o(\| h \|)
$$
$$
f(x_{0} + h) = f(x_{0}) + df_{x_{0}}(h) + \frac{1}{2} d^{2}f_{x_{0}}(h,h) + o(\| h \|^{2})
$$
$$
f(x_{0} + h) = f(x_{0}) + <\nabla f(x_{0}),h> + \frac{1}{2}<H_{f}(x)\cdot h,h> + o(\| h \|^{2})
$$
# 凸分析
- 凸集
$$
\forall (x,y) \in S^{2}, \forall t \in [0,1], tx + (1-t) y \in S
$$
- 凸函数
$$
\forall (x,y) \in S^{2}, \forall t \in [0,1], f(tx + (1-t) y) \le tf(x) + (1-t)f(y)
$$
- 严格凸函数
$$
\forall (x,y) \in S^{2}, \forall t \in [0,1], f(tx + (1-t) y) < tf(x) + (1-t)f(y)
$$
- 强凸函数
Fortement convexe de module $m > 0$, si:
	m-fortement convexe
$$
f(tx + (1-t) y) \le tf(x) + (1-t)f(y) - \frac{m}{2}t(1-t)\| x - y \|^{2}
$$
强凸函数满足几条性质：
1. f est strictement convexe.
2. $\forall (x,y)\in (\mathbb(R)^{n})^{2}$
$$
f(y) \ge f(x) + <\nabla f(x), y - x> + \frac{m}{2}\| y-x \|^{2}
$$
3. f est coercive.
4. f admet un unique minimum global $x^{*}$
5. $\forall x \in \mathbb{R}^{n}$
$$
f(x^{*}) \ge f(x) - \frac{1}{2m}\| \nabla f(x) \|^{2}, \| x-x^{*} \| \le \| \nabla f(x) \|
$$
- 梯度判断凸函数
$$
f(y) \ge f(x) + <\nabla f(x), y - x>, \forall (x,y) \in C^{2}
$$
- 海森矩阵判断凸函数
Soit $C \subset \mathbb{R}^{n}$ un ouvert convexe, $f: \mathbb{R}^{n} \longrightarrow \mathbb{R}$ une fonction deux fois différentiable, alors
1. Convexe $\Leftrightarrow H_{f}$ 半正定
2. Strictement Convexe $\Leftarrow H_{f}$ 正定
3. Fortement Convexe $\Leftrightarrow H_{f}$ 正定
