快速傅里叶变换是极其重要的一种复数矩阵，真正的改变了世界，所以我们在这节简单的介绍一下它。
结合数字信号处理可以极大的简化理解，所以以下会结合数字信号处理的内容。
# 傅里叶变换矩阵
我们通过 DSP 中的 DFT 来引出傅里叶变换矩阵，同时我们还可以了解后面对该矩阵做变换的时候为什么需要将它的奇偶行进行互换。
假设我们在时域中对连续信号采了四次样，要将其转化为频域中的四个离散的点：
$$
[x_{0},x_{1},x_{2},x_{3}] \Rightarrow [X_{0},X_{1},X_{2},X_{3}]
$$
	下标表示采样序列
根据 DTFT 的经验，我们知道:
$$
X_{\omega} = \sum_{n=-\infty}^{+\infty}x_{n}e^{-j\omega n}
$$
而现在因为是 DFT，我们只在 Nyquist Interval 离散的几个 $\omega$ 值上进行计算。假设时域采样次数为 L，而频域采样次数为 N，我们将那几个频率记作：
$$
\omega_{k} = \dfrac{2\pi}{N}k,k\in[|0,N-1|]
$$
	在现实情况中，我们通常会令 L = N，使得傅里叶变换矩阵可逆。
于是我们可以将我们的 DFT 过程写成矩阵形式：
$$
\begin{bmatrix}
X_{0} \\
X_{1} \\
X_{2} \\
X_{3}
\end{bmatrix}
=
\begin{bmatrix}
e^{-j\omega_{0} \times 0} & e^{-j\omega_{0} \times 1} & e^{-j\omega_{0} \times 2} &e^{-j\omega_{0} \times 3} \\
e^{-j\omega_{1} \times 0} & e^{-j\omega_{1} \times 1} &e^{-j\omega_{1} \times 2} &e^{-j\omega_{1} \times 3}\\
e^{-j\omega_{2} \times 0} & e^{-j\omega_{2} \times 1} &e^{-j\omega_{2} \times 2} &e^{-j\omega_{2} \times 3}\\
e^{-j\omega_{3} \times 0} & e^{-j\omega_{3} \times 1} &e^{-j\omega_{3} \times 2} &e^{-j\omega_{3} \times 3}\\
\end{bmatrix}
\begin{bmatrix}
x_{0} \\
x_{1} \\
x_{2} \\
x_{3}
\end{bmatrix}
$$
为了简化矩阵表示，我们定义一个新符号：
$$
w_{N}^{kn} = e^{-j\frac{2\pi}{N}k\times n}
$$
所以原矩阵表达式就可以表示为：
$$
\begin{bmatrix}
X_{0} \\
X_{1} \\
X_{2} \\
X_{3}
\end{bmatrix}
=
\begin{bmatrix}
w_{4}^{0 \times 0} & w_{4}^{0 \times 1} & w_{4}^{0 \times 2} & w_{4}^{0 \times 3} \\
w_{4}^{1 \times 0} & w_{4}^{1\times 1} & w_{4}^{1 \times 2} & w_{4}^{1 \times 3} \\
w_{4}^{2 \times 0} & w_{4}^{2 \times 1} & w_{4}^{2 \times 2} & w_{4}^{2 \times 3} \\
w_{4}^{3 \times 0} & w_{4}^{3 \times 1} & w_{4}^{3 \times 2} & w_{4}^{3 \times 3} \\
\end{bmatrix}
\begin{bmatrix}
x_{0} \\
x_{1} \\
x_{2} \\
x_{3}
\end{bmatrix}
=
\begin{bmatrix}
w_{4}^{0} & w_{4}^{0} & w_{4}^{0} & w_{4}^{0} \\
w_{4}^{0} & w_{4}^{1} & w_{4}^{2} & w_{4}^{3} \\
w_{4}^{0} & w_{4}^{2} & w_{4}^{4} & w_{4}^{6} \\
w_{4}^{0} & w_{4}^{3} & w_{4}^{6} & w_{4}^{9} \\
\end{bmatrix}
\begin{bmatrix}
x_{0} \\
x_{1} \\
x_{2} \\
x_{3}
\end{bmatrix}
$$
现在假想，我在时域中采集了四个点 L = 4，但是只需要变换两个点，N = 2，矩阵表达式会发生什么？我们知道:
	事实上这在现实中是非常常见的情况，我有极高的采样频率，但是只需要变换出几个点就能获得我需要的信息
$$
w_{2}^{0} = w_{2}^{2}, w_{2}^{1} = w_{2}^{3}
$$
所以原来的矩阵表达式就变为了：
$$
\begin{bmatrix}
X_{0} \\
X_{1} \\
\end{bmatrix}
=
\begin{bmatrix}
w_{2}^{0} & w_{2}^{0} & w_{2}^{0} & w_{2}^{0} \\
w_{2}^{0} & w_{2}^{1} & w_{2}^{0} & w_{2}^{1} \\
\end{bmatrix}
\begin{bmatrix}
x_{0} \\
x_{1} \\
x_{2} \\
x_{3}
\end{bmatrix}
$$
我们将原来的采样序列进行一些奇偶交换，可以得到一个等价的，但是矩阵阶数更低的矩阵表达式：
$$
\begin{bmatrix}
X_{0} \\
X_{1} \\
\end{bmatrix}
=
\begin{bmatrix}
w_{2}^{0} & w_{2}^{0} \\
w_{2}^{0} & w_{2}^{1} \\
\end{bmatrix}
\begin{bmatrix}
x_{0} + x_{2} \\
x_{1} + x_{3} \\
\end{bmatrix}
$$
	这里就已经有一些 FFT 的味道在里面了
# Fast Fourier Transform
我们定义傅里叶矩阵如下：
$$
F_{n} =
\begin{bmatrix}
1 & 1 & 1 & \cdots & 1 \\
1 & w & w^{2} & \cdots & w^{n-1} \\
1 & w^{2} & w^{4} & \cdots & w^{2(n-1)} \\
\vdots \\
1 & w^{n-1} & w^{2(n-1)} & \cdots & w^{(n-1)^{2}} \\
\end{bmatrix},
w = e^{j\frac{2\pi}{n}}
$$
我们尝试将高阶傅里叶矩阵进行分解，用阶数更低的傅里叶矩阵来表示，这样可以大大的减少计算次数。结果如下，后面解释；
$$
\begin{bmatrix}
F_{64}
\end{bmatrix}
=
\begin{bmatrix}
I & D \\
I & -D
\end{bmatrix}
\begin{bmatrix}
F_{32} & 0 \\
0 & F_{32}
\end{bmatrix}
\begin{bmatrix}
1 & 0 & 0 & 0 & \cdots \\
0 & 0 & 1 & 0 & \cdots \\
\vdots \\
0 & 1 & 0 & 0 & \cdots \\
0 & 0 & 0 & 1 & \cdots \\
\end{bmatrix}
$$
最右侧的矩阵是一个置换矩阵，目的是通过交换傅里叶矩阵中的列，实现对输入列向量的奇偶项的分别处理：
$$
\begin{bmatrix}
F_{32} & 0 \\
0 & F_{32}
\end{bmatrix}
\begin{bmatrix}
1 & 0 & 0 & 0 & \cdots \\
0 & 0 & 1 & 0 & \cdots \\
\vdots \\
0 & 1 & 0 & 0 & \cdots \\
0 & 0 & 0 & 1 & \cdots \\
\end{bmatrix}=
\begin{bmatrix}
1 && 1 && 1 && \cdots \\
1 & 0 & w_{32} & 0 & w^{2}_{32} & 0 &\cdots\\
1 && w^{2}_{32} && w^{4}_{32} && \cdots \\
\vdots \\
& 1 && 1 && 1 & \cdots \\
0 & 1 & 0 & w_{32} & 0 & w^{2}_{32} & \cdots\\
& 1 && w^{2}_{32} && w^{4}_{32} & \cdots \\
\end{bmatrix}
$$
输入向量和处理后的向量分别是：
$$
X =
\begin{bmatrix}
x_{0} \\
x_{1} \\
x_{2} \\
\vdots \\
x_{32} \\
x_{33} \\
x_{34} \\
\vdots
\end{bmatrix},
X_{tmp} =
\begin{bmatrix}
x_{0} + x_{2} + \cdots + x_{62} \\
x_{0} + w_{32}x_{2} + \cdots + w^{31}_{32}x_{62} \\
x_{0} + w_{32}^{2}x_{2} + \cdots + w_{32}^{62}x_{62} \\
\vdots \\
x_{1} + x_{3} + \cdots + x_{63} \\
x_{1} + w_{32}x_{3} + \cdots + w_{32}^{31}x_{63} \\
x_{1} + w_{32}^{2}x_{3} + \cdots + w_{32}^{62}x_{63} \\
\vdots
\end{bmatrix}
=
\begin{bmatrix}
x_{0} + x_{2} + \cdots + x_{62} \\
x_{0} + w_{64}x_{4} + \cdots + w_{64}^{62}x_{62} \\
x_{0} + w_{64}^{4}x_{2} + \cdots + w_{64}^{124}x_{62} \\
\vdots \\
x_{1} + x_{3} + \cdots + x_{63} \\
x_{1} + w_{64}^{2}x_{6} + \cdots + w_{64}^{62}x_{63} \\
x_{1} + w_{64}^{4}x_{3} + \cdots + w_{64}^{124}x_{63} \\
\vdots
\end{bmatrix}
=
\begin{bmatrix}
X_{odd} \\
X_{even}
\end{bmatrix}
$$
这一步置换矩阵的运算在计算机中几乎不需要什么运算量。
最左侧的修正矩阵需要较多的运算量，目的是给原本输入向量偶数位上的元素补上 w 的阶数，然后加到奇数位的结果中，得到完整的结果。其中对角矩阵 D 的定义方式是：
$$
D = 
\begin{bmatrix}
1 \\
& w_{64} \\
&& w_{64}^{2} \\
&&& \ddots \\
&&&& w_{64}^{31}
\end{bmatrix}
$$
$$
\begin{bmatrix}
I & D \\
I & -D
\end{bmatrix}
\begin{bmatrix}
X_{odd} \\
X_{even}
\end{bmatrix}
=
\begin{bmatrix}
X_{odd} + DX_{even} \\
X_{even} - DX_{even}
\end{bmatrix}
$$
	下半部分变成负是因为提出了一个 w^{32} = -1.
我们看一下稍微具体的展示：
$$
DX_{even} = 
\begin{bmatrix}
x_{1} + x_{3} + \cdots + x_{63} \\
w_{64}x_{1} + w_{64}^{3}x_{3} + \cdots + w_{64}^{63}x_{63} \\
w_{64}^{2}x_{1} + w_{64}^{6}x_{3} + \cdots + w_{64}^{126}x_{63} \\
\vdots
\end{bmatrix}
$$
$$
X_{odd} + DX_{even}=
DX_{even} = 
\begin{bmatrix}
x_{0} + x_{2} + \cdots + x_{62} \\
x_{0} + w_{64}x_{4} + \cdots + w_{64}^{62}x_{62} \\
x_{0} + w_{64}^{4}x_{2} + \cdots + w_{64}^{124}x_{62} \\
\vdots \\
\end{bmatrix}
\begin{bmatrix}
x_{1} + x_{3} + \cdots + x_{63} \\
w_{64}x_{1} + w_{64}^{3}x_{3} + \cdots + w_{64}^{63}x_{63} \\
w_{64}^{2}x_{1} + w_{64}^{6}x_{3} + \cdots + w_{64}^{126}x_{63} \\
\vdots
\end{bmatrix}
=
result
$$
## 时间复杂度
$$
\mathcal{O}(n^{2}) \longrightarrow \mathcal{O}(n\log n)
$$
