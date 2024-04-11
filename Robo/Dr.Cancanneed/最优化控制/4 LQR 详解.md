此前在 [[LQR 控制器]] 中我们已经初步的探索了线性控制和 LQR 的部分思想。现在我们来详细推导一下 LQR 的整个过程。
# 线性二次型调节器
我们说 LQR 全名线性二次型调节器，我们先来对这三个名称做详解：
- 线性：系统模型是线性的
也就是系统的状态空间方程一般都可以直接写成以下形式：
$$
\vec{x}[k+1] = A\vec{x}[k] + B\vec{u}[k]
$$
非线性系统看我们的第一节。
- 二次型：代价函数是一个二次型形式
$$
J = \frac{1}{2}(\vec{x}[N] - \vec{x}_d[N])^{\top}S(\vec{x}[N] - \vec{x}_d[N]) + \sum_{k=1}^{N-1} (\frac{1}{2}(\vec{x}[k] - \vec{x}_d[k])^{\top}S(\vec{x}[k] - \vec{x}_d[k]) + u[k]^{\top}Ru[k])
$$
该函数第一项叫末端代价，第二项叫运行代价。
需要注意的是，S 矩阵可以是半正定矩阵，就算她为零，也只是系统达不到我们的控制目标，不会发疯。而 R 矩阵一定得是个正定矩阵。如果她为 0，那么调节器会做的就是取一个无穷大的控制量，使得系统在一瞬间内达到期望状态。这是没有任何意义的。因此这个矩阵必须正定。
- 调节器：目标为 $\vec{0}$
根据这个特性，我们可以改写代价函数：
$$
J = \frac{1}{2}\vec{x}[N]^{\top}S\vec{x}[N] + \sum_{k=1}^{N-1} (\frac{1}{2}\vec{x}[k]^{\top}S\vec{x}[k] + u[k]^{\top}Ru[k])
$$
# 寻找最优策略
我们先看 [[2 最优控制问题 & 性能指标]] 中的控制策略部分，我们发现可以由初始状态和控制策略推导出任意时刻状态。我们需要做的就是确定这个控制策略。但我们发现所有时刻的控制量都嵌套在了一起，所以我们采用逆向分级的思想，每次只求其中一个就会方便很多。
## 逆向分级
- 假设我们的时刻处于最后时刻 $k = N$
$$
\begin{align}
J_{N\rightarrow N} &= \frac{1}{2}x^{\top}[N] \ S \ x[N] \\
&= \frac{1}{2}x^{\top}[N] \ P[0] \ x[N]
\end{align}
$$
- 处于 $k = N - 1$
$$
\begin{align}
J_{N-1\rightarrow N} &= \frac{1}{2}\vec{x}[N]^{\top}S\vec{x}[N] + \frac{1}{2}\vec{x}[N-1]^{\top} \ Q \ \vec{x}[N-1] + \frac{1}{2}u[N-1]^{\top} \ R \ u[N-1] \\
&= \frac{1}{2}x^{\top}[N] \ P[0] \ x[N] + \frac{1}{2}\vec{x}[N-1]^{\top} \ Q \ \vec{x}[N-1] + \frac{1}{2}u[N-1]^{\top} \ R \ u[N-1] \\
&= J_{N\rightarrow N}^* + \frac{1}{2}\vec{x}[N-1]^{\top} \ Q \ \vec{x}[N-1] + \frac{1}{2}u[N-1]^{\top} \ R \ u[N-1]
\end{align}
$$
可以看出这一步的代价函数包含了下一步的代价函数，这是非常显然的。如果我们继续往前推导代价函数也会得到一样的结论。之所以下一步的代价函数一定是最优的到家函数，是根据贝尔曼最优性原理，我们知道之后采取的策略一定是最优决策。
- 处于 $k = N - 2$
$$
J_{N-2\rightarrow N-1} = J_{N\rightarrow N-1}^* + \frac{1}{2}\vec{x}[N-2]^{\top}Q\vec{x}[N-2] + \frac{1}{2}u[N-2]^{\top} \ R \ u[N-2]
$$

这样逆向分级，逆向推导的好处是，我们每次只需要推导当前这步的控制决策就好了。
## 求解
例如我们要求解 $u[N-1]$，采取对 $J_{N\rightarrow N-1}$ 对 $u[N-1]$ 求导的策略。但在此之前，我们知道有以下关系：
$$
\vec{x}[N] = A\vec{x}[N-1] + B\vec{u}[N-1]
$$
我们需将其带入代价函数，然后才能获得只关于当前状态 $\vec{x}[N-1]$ 的反馈。将代价函数写作：
$$
\begin{align}
J_{N-1\rightarrow N} &= \frac{1}{2}(A\vec{x}[N-1] + B\vec{u}[N-1])^{\top}P[0](A\vec{x}[N-1] + B\vec{u}[N-1]) \\
&+ \frac{1}{2}\vec{x}[N-1]^{\top} \ Q \ \vec{x}[N-1] + \frac{1}{2}u[N-1]^{\top} \ R \ u[N-1]
\end{align}
$$
可以看出，这个式子的第一项是一个复合函数求导：
$$
\begin{align}
\frac{\partial \frac{1}{2}\vec{x}[N]^{\top} \ P[0] \ \vec{x}[N]}{\partial \vec{u}[N-1]} &= \frac{\partial \vec{x}[N]}{\partial \vec{u}[N-1]} \cdot \frac{\partial \frac{1}{2}\vec{x}[N]^{\top} \ P[0] \ \vec{x}[N]}{\vec{x}[N]} \\
&= B^{\top}P[0]^{\top}\vec{x}[N] \\
&= B^{\top}P[0]^{\top}(A\vec{x}[N-1] + B\vec{u}[N-1])
\end{align}
$$
为了求二次型的极值，我们希望这个导数为 0，这样可以求出最优控制为：
$$
\begin{align}
u^*[N-1] &= (B^{\top}P[0]B + R)^{-1}B^{\top}P[0]A \vec{x}[n-1] \\
&= -F[N-1]\vec{x}[N-1]
\end{align}
$$
算了半天终于得到了我们的反馈系数！ 
再往前递推，过程跟上面几乎是一模一样的。同时，可以体现出我们设 $P[0]$ 矩阵的用处：
$$
\begin{align}
J_{N-1\rightarrow N}^* &= \frac{1}{2}\vec{x}[N-1]^{\top} ((A - BF[N-1])^{\top}P[0](A - BF[N-1]) + F[N-1]^{\top}RF[N-1] + Q)\vec{x}[N-1] \\
&= \frac{1}{2}\vec{x}[N-1]^{\top} \ P[1] \ \vec{x}[N-1]
\end{align}
$$
后面就跟上面一样算就好了。

# 结论
$$
J_{N-k\rightarrow N}^* = \frac{1}{2}\vec{x}[N-k]^{\top} \ P[k] \ \vec{x}[N-k]
$$
$$
P[k] = (A - BF[N-k])^{\top}P[0](A - BF[N-k]) + F[N-k]^{\top}RF[N-k] + Q
$$
$$
F[N-k] = (B^{\top}P[k-1]B + R)^{-1}B^{\top}P[k-1]A
$$
$$
u^*[N-k] = -F[N-k]\vec{x}[N-k]
$$