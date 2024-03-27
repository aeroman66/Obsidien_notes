运动学的部分比较简单，更多的是矩阵操作。接下来我们进入动力学范畴。尽管我们已经研究了静力和速度，用一个雅可比矩阵将关节空间和足端空间联系起来。但是我们还没有考虑过引起运动所需的力，也就是**动态**情况下的动力学问题。
我们在这里主要研究两个问题：
1. 已知一个轨迹点 $\Theta,\dot{\Theta},\ddot{\Theta}$ ,求出期望的关节力矩矢量 $\tau$
	类似于逆运动学
2. 计算施加一组关节力矩情况下足端将如何运动
	这个主要用于仿真器的计算。更加类似于正运动学。
# 一种很 Confusing 的 Notation
我们把要与后面向量做叉积的向量记作某种矩阵形式，并给它赋予某种并不是很简洁的符号：
$$
[ \ \vec{p} \ ]_{\times} = 
\begin{bmatrix}
0 & -p_{z} & p_{y} \\
p_{z} & 0 & -p_{x} \\
-p_{y} & p_{x} & 0
\end{bmatrix}
$$
假设 $\vec{p}$ 与 $[x \ y \ z]^{T}$ 做叉积：
$$
\begin{bmatrix}
p_{x} \\
p_{y} \\
p_{z}
\end{bmatrix}
\times
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
=
\begin{bmatrix}
p_{y}z - p_{z}y \\
p_{z}x - p_{x}z \\
p_{x}y - p_{y}x
\end{bmatrix}
=
\begin{bmatrix}
0 & -p_{z} & p_{y} \\
p_{z} & 0 & -p_{x} \\
-p_{y} & p_{x} & 0
\end{bmatrix}
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
$$
借助这种表达式，我们成功把叉乘符号换成了矩阵乘法。