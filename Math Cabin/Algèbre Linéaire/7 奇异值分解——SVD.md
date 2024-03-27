	Single Value Decomposition
奇异值是矩阵里的概念，一般通过奇异值分解定理求得。设A为 $m \times n$ 阶矩阵，$q = \min(m,n)$ $A^{T}A$(这部分有问题) 的 q 个非负特征值的算术平方根叫作A的奇异值。
在[[5.2 Eigen Applications]]中我们已经知道了，对于满足特定条件的方阵，我们有以下分解方式：
$$
A = S\Lambda S^{-1}
$$
尤其对于对称矩阵来说：
$$
A = Q\Lambda Q^{T}
$$
现在，我们想把这种分解方法扩展到任意矩阵，甚至不一定是方阵上。
# SVD
我们将原矩阵分解为正交矩阵、对角矩阵、正交矩阵的形式，其中两个正交矩阵不一定要是同一个：
$$
A = U\Sigma V^{T}
$$
我们取一个 $m \times n$ 的矩阵 A ，并假设 $rank(A) = r$，我们取以下四组正交基：
- Row Space: $v_{1},v_{2},\cdots,v_{r}$
- Column Space: $u_{1},u_{2},\cdots,u_{r}$
- Null Space: $v_{r+1},\cdots,v_{n}$
- 左零空间: $u_{r+1},\cdots,u_{m}$
我们想要：
$$
\forall i \in [|1,r|], Av_{i} = \sigma_{i}u_{i}
$$
$$
\forall i \in [|r+1,n|], Av_{i} = 0
$$
所以我们有：
$$
\begin{align}
A
\begin{bmatrix}
v_{1} & v_{2} & \cdots & v_{n}
\end{bmatrix}
&=
\begin{bmatrix}
\sigma_{1}u_{1} & \sigma_{2}u_{2} & \cdots & \sigma_{r}u_{r} & 0 & \cdots & 0
\end{bmatrix}
\\
&=
\begin{bmatrix}
u_{1} & u_{2} & \cdots & u_{r} & 0 & \cdots & 0
\end{bmatrix}
\begin{bmatrix}
\sigma_{1} & & \\
& \sigma_{2} &&&& 0\\
&&\ddots &  \\
&&&\sigma_{r} \\
&&&& 0 \\
&0&&&&\ddots \\
&&&&&& 0
\end{bmatrix}
\end{align}
$$
把上面的矩阵表达形式化简，得到：
$$
AV = U\Sigma
$$
即：
$$
A = U\Sigma V^{T}
$$
这就是我们一般所说的奇异值分解。之所以叫这个名字，是因为中间对角矩阵对角线上元素都被称作奇异值。
# 求解方法
通常情况下，分别求解 $U,V,\Sigma$ 比较的困难，因此我们希望将其转化为某个矩阵的特征向量，将奇异值与某个矩阵的特征值进行挂钩来求解。
方法如下：
- 求解 V 和奇异值：
$$
A^{T}A = V\Sigma^{T} U^{T}U\Sigma V^{T}
$$
因为 U 是一个正交矩阵，所以我们有：
$$
\begin{align}
A^{T}A &= V\Sigma^{T} I\Sigma V^{T} \\
&= V
\begin{bmatrix}
\sigma_{1}^{2} & & \\
& \sigma_{2}^{2} &&&& 0\\
&&\ddots &  \\
&&&\sigma_{r}^{2} \\
&&&& 0 \\
&0&&&&\ddots \\
&&&&&& 0
\end{bmatrix}V^{T}
\end{align}
$$
我们惊奇地发现这就是某个对称矩阵的分解，其中 $A^{T}A$ 矩阵的特征向量构成矩阵 V，特征值分别对应奇异值的平方。
- 求解 U
我们约定奇异值都为非负数，但是 $A^{T}A$ 矩阵的正交归一基却无法确定正负。这种情况下，我们只能人为选择一个正负，然后通过：
$$
Av_{i} = \sigma_{i}u_{i}
$$
来求解 U 矩阵。

# Exemples
1. 满秩情况
取：
$$
A = 
\begin{bmatrix}
4 & 4 \\
-3 & 3
\end{bmatrix}
$$
- 求解 V 和奇异值：
$$
A^{T}A = 
\begin{bmatrix}
4 & -3 \\
4 & 3
\end{bmatrix}
\begin{bmatrix}
4 & 4 \\
-3 & 3
\end{bmatrix}
=
\begin{bmatrix}
25 & 7 \\
7 & 25
\end{bmatrix}
$$
可得：
$$
\sigma_{1} = \sqrt{32}, v_{1} =
\begin{bmatrix}
\frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} \\
\end{bmatrix};
\sigma_{2} = \sqrt{18}, v_{2} =
\begin{bmatrix}
\frac{1}{\sqrt{2}} \\
-\frac{1}{\sqrt{2}} \\
\end{bmatrix}
$$
	这里特征向量的正负号就已经是我们选定的了
- 求解 U
$$
Av_{1} = \sigma_{1}u_{1}
$$
$$
u_{1} = 
\begin{bmatrix}
1 \\
0
\end{bmatrix}
$$
同理：
$$
Av_{2} = \sigma_{2}u_{2},
u_{2} = 
\begin{bmatrix}
0 \\
-1
\end{bmatrix}
$$
- 结果
$$
A = U\Sigma V^{T} = 
\begin{bmatrix}
1 & 0\\
0 & -1
\end{bmatrix}
\begin{bmatrix}
\sqrt{32} & 0\\
0 & \sqrt{18}
\end{bmatrix}
\begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}}\\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}
$$
2. 不满秩情况
$$
A = 
\begin{bmatrix}
4 & 3 \\
8 & 6
\end{bmatrix}
$$
- 求 V 和奇异值
为了构建完整的 V ，我们需要行空间的基和零空间的基。但是因为这两个空间是正交的，所以到时候只需要取于行空间基正交的向量就是零空间的基了。
$$
A^{T}A = 
\begin{bmatrix}
4 & 8 \\
3 & 6
\end{bmatrix}
\begin{bmatrix}
4 & 3 \\
8 & 6
\end{bmatrix}
=
\begin{bmatrix}
80 & 60 \\
60 & 45
\end{bmatrix}
$$
得到：
$$
\sigma_{1} = \sqrt{125}, v_{1} =
\begin{bmatrix}
0.8 \\
0.6 \\
\end{bmatrix};
\sigma_{2} = 0, v_{2} =
\begin{bmatrix}
-0.6 \\
0.8 \\
\end{bmatrix}
$$
- 求解 U
步骤跟上个例子一样，得到：
$$
u_{1} = 
\begin{bmatrix}
\frac{1}{\sqrt{5}} \\
\frac{2}{\sqrt{5}}
\end{bmatrix},
u_{2} = 
\begin{bmatrix}
\frac{2}{\sqrt{5}} \\
-\frac{1}{\sqrt{5}}
\end{bmatrix}
$$
- 结果
$$
A = U\Sigma V^{T} = 
\begin{bmatrix}
\frac{1}{\sqrt{5}} & \frac{2}{\sqrt{5}}\\
\frac{2}{\sqrt{5}} & -\frac{1}{\sqrt{5}}
\end{bmatrix}
\begin{bmatrix}
\sqrt{125} & 0\\
0 & 0
\end{bmatrix}
\begin{bmatrix}
0.8 & 0.6\\
-0.6 & 0.8
\end{bmatrix}
$$