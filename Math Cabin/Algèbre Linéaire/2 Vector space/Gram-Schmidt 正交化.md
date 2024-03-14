	该正交化的一大缺点，因为常常要归一化向量，所以会产生很多的根号。
# Q——标准正交基构成的矩阵
我们假设有一组正交归一的矩阵：
$$
q_{i}^{T} \ q_{j} = \delta_{i,j}
$$
令这些向量构成一个矩阵的各列，这个矩阵**不必须是一个方阵**：
$$
Q = 
\begin{bmatrix}
q_{1} & \cdots & q_{n}
\end{bmatrix}
$$
容易发现此性质：
$$
Q^{T}Q = 
\begin{bmatrix}
q_{1}^{T} \\
\vdots \\
q_{n}^{T}
\end{bmatrix}
\begin{bmatrix}
q_{1} & \cdots & q_{n}
\end{bmatrix}
= I_{n}
$$
	也就是非方阵时，转置只有左乘才得到单位矩阵。
并且如果 Q 是方阵的话，更甚：
$$
Q^{T} = Q^{-1}
$$
此时 Q 才被称为**正交矩阵**，也就是说正交矩阵前提为方阵。
## Exemple
$$
\text{Perm} \ Q = 
\begin{bmatrix}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0
\end{bmatrix}
\begin{bmatrix}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0
\end{bmatrix}
= I_{3}
$$
$$
Q = 
\begin{bmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{bmatrix}
,
Q = \frac{1}{\sqrt{2}}
\begin{bmatrix}
1 & -1 \\
1 & 1
\end{bmatrix}
,
\text{Adhemar Matrix}
$$
## 投影
在一般情况下，也就是包括了 Q 不是方阵的情况，它的各列正交归一且线性独立，我们有投影矩阵：
$$
P = Q(Q^{T}Q)^{-1}Q^{T} = QQ^{T}
$$
方阵时：
$$
P = QQ^{T} = I
$$
	非常的合理，因为此时 Q 就代表了整个向量空间，向整个向量空间投影，很自然的就得到了原本的向量。
## 优势
很多复杂的方程，只要用了标准正交基可以化的非常简单。
如之前的 normal equation:
$$
\begin{align}
A^{T}A\hat{x} &= A^{T}b \\
Q^{T}Q\hat{x} &= Q^{T}b \\
\hat{x} &= Q^{T}b
\end{align}
$$
由此得到了一个很基本的性质，一个向量在各个基向量上的投影得到的向量：
$$
\hat{x}_{i} = q_{i}^{T}b_{i}
$$

# Gram-Schmidt 正交化
基本流程：
$$
\text{vectors a,b} \longrightarrow \text{orthogal vectors A,B} \longrightarrow \text{orthonormal vectors} \ q_{1} = \frac{A}{\| A \|},q_{2} = \frac{B}{\| B \|}
$$
一般在一组向量 $a,b,\cdots,n$ 中，我们会直接选取第一个向量做开始：
$$
A = a
$$
然后将第二个向量减去它在第一个向量上的投影：
$$
B = b - \frac{A^{T}b}{A^{T}{A}}A
$$
之后的向量减去它在之前已正交化的各个向量上的投影，如：
$$
C = c - \frac{A^{T}c}{A^{T}{A}}A - \frac{B^{T}c}{B^{T}{B}}B
$$
## 矩阵表示
我们知道消元法存在矩阵表示：
$$
A = LU
$$
那么正交化是不是也存在一个矩阵表示呢：
$$
A = QR
$$
	R 为一个上三角矩阵，将两个矩阵 A Q 联系了起来。