	拉氏变换
将一个时域上的函数转化到复数域上：
$$
f(t) \longrightarrow F(s),s = \sigma + j \omega
$$

可以大大减小系统复杂程度与分析难度。
# 定义概念
定义式，有关 s 的信息可以在前言里找到：
$$
\mathcal{L}[f(t)] = \int_{0}^{+\infty}f(t)e^{-st}dt
$$
时间是从 0 以后开始取的，这是为了符合实际情况，毕竟现实里的时间并不会取负数。（当然我们有双边拉普拉斯变换）
让我们搬出傅立叶变换与之做个比较：
$$
\mathcal{F}[f(t)] = \int_{-\infty}^{+\infty}f(t)e^{-i\omega t}dt
$$
我们发现，拉普拉斯变换事实上就是比傅立叶变换多了一个 $e^{-\sigma t}$ 的项，我们称之为衰减因子。
## 拉普拉斯变换存在定理

# 相关公式
我们来推导一个常用的拉普拉斯变换：
$$
\begin{align}
\mathcal{L}[f(t)] &= \mathcal{L}[e^{-at}] \\
&= \int_{0}^{+\infty}e^{-at}e^{-st}dt \\
&= \int_{0}^{+\infty}e^{-(a+s)t}dt \\
&= -\frac{1}{a+s}e^{-(a+s)t}\big|_{0}^{+\infty} \\
&= \frac{1}{a+s}
\end{align}
$$
- $\mathcal{L}[af(t) + bg(t)] = aF(s) + bG(s)$
- $\mathcal{L}[f^{(n)}(t)] = s^{n}F(s) - s^{n-1}f(0)-s^{n-2}f''(0)-\cdots -f^{(n-1)}(0)$
- $\mathcal{L}[\int_{0}^{t}\int_{0}^{t}\cdots\int_{0}^{t}f(t)dtdtdt] = \frac{1}{s^{n}}\mathcal{L}f(t)$
# 收敛域 ROC
	Region of convergence
对一个时域函数进行拉氏变换后，我们通常会遇到一个可积性的问题，见下：
$$
\mathcal{L}[f(t)] = \int_{0}^{+\infty}e^{-at}e^{-st}dt = \int_{0}^{+\infty}e^{-(a+s)t}dt = -\frac{1}{s+a}e^{-(a+s)t}\bigg|_{0}^{+\infty}
$$
我们发现下函数不一定是可积的，积分值可能趋向于正无穷，不满足可积性的定义：
$$
g(t) = e^{-(a+s)t}
$$
为了使这个函数可积，我们需要让拉氏变换后的复数，也就是 s 满足一些特定的条件。而满足这些条件的 s 的集合就是我们所说的可积域了。
	只是起了个高大上的名字嘛
我们来试着求解 $f(t)$ 的可积域：
$$
\mathcal{L}[f(t)] = \int_{0}^{+\infty}e^{-at}e^{-st}dt = \int_{0}^{+\infty}e^{-at}e^{-(\sigma + j \omega)t}dt = \int_{0}^{+\infty}e^{-(a + \sigma) t}e^{-j \omega t}dt
$$
后面虚指数部分模长恒为 1，不用考虑。只考虑前面，为了使其在时间趋向于无穷大时收敛，我们需要：
$$
-(a + \sigma) < 0
$$
$$
\sigma > -a
$$
这就是这个函数的收敛域了。

# 逆变换 ILT
	Inverse Laplace Transform
我们之所以要研究拉普拉斯逆变换，是为了更方便的求解微分方程。
微分方程是描述动态世界的一种数学手段，动态世界是不断变化的，写成数学就是一个状态变量随时间的变化：
$$
\frac{dx}{dt}
$$
	在经典控制理论和线代控制理论中，我们大部分的研究对象都是常系数微分方程，对应的就是线性时不变系统。
进入该部分正题。拉普拉斯变换求微分方程通常分为三步：
1. $t \longrightarrow s$：拉普拉斯变换
2. $+-\times\div$：求解代数方程
3. $s \longrightarrow t$：逆拉普拉斯变换
## E.g.
去看[[Transfer function]]里的那个例子。