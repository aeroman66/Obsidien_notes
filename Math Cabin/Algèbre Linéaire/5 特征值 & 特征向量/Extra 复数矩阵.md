我们先来了解复数在线性代数中所需要的与实数不同的运算。
# 复数
- 向量内积
有一个复数向量：
$$
z =
\begin{bmatrix}
z_{1} \\
z_{2} \\
\vdots \\
z_{n}
\end{bmatrix}
\in \mathbb{C}^{n}
$$
如果我们还按照实数向量的方法求向量模长，也就是让他自己和自己做内积，我们会发现结果不一定是正的。这与模长的定义矛盾。所以在向量做内积时，我们定义对向量做转置的同时取共轭处理。
$$
\|z\|^{2} = \bar{z}^{T}z = 
\begin{bmatrix}
\bar{z}_{1} & \bar{z}_{2} & \cdots & \bar{z}_{n}
\end{bmatrix}
\begin{bmatrix}
z_{1} \\
z_{2} \\
\vdots \\
z_{n}
\end{bmatrix}
$$
同理，对于两个复数向量 $x,y$ :
$$
<x,y> = \bar{y}^{T}x
$$
- 矩阵运算
对于复数矩阵来说，一个性质优良的矩阵就不仅仅是转置等于自身了，而需要：
$$
A = \bar{A}^{T} = 
\begin{bmatrix}
2 & 3+i \\
3-i & 5
\end{bmatrix}
$$
	主对角线上必须是实数这种情况下。
- 正交矩阵
$$
\bar{Q}^{T}Q = I = Q^{H}Q
$$
## Hermitian
我们把转置和取共轭的符号记作一个，把它看作一个形容词：
$$
\text{Hermitian}:H
$$
- Hermitian Produit
$$
<x,y> = \bar{y}^{T}x = y^{H}x
$$
- Hermitian Matrix
$$
A = \bar{A}^{T} = A^{H}
$$
