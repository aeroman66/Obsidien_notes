	裴蜀定理，怪不得很耳熟
Soient $(a,b)\in \mathbb{Z}^{2}$ non tous nuls, alors:
$$
\exists (u,v) \in \mathbb{Z}^{2}, au + bv = PGCD(a,b)
$$
重要推论：
$$
[\text{a,b sont premiers entre eux}]\Leftrightarrow \exists (u,v) \in \mathbb{Z}^{2}, au + bv = 1
$$
	demo: a z + b z = PGCD(a,b)
# Comment calculer u et v
On prend l'exemple suivante:
$$
a = 143,b = 23 , PGCD(143,23) = 1
$$
On sait deja:
$$
\begin{align}
143 &= 6 \times 23 + 5 \\
23 &= 4 \times 5 + 3 \\
5 &= 1 \times 3 + 2 \\
3 &= 1 \times 2 + 1 \\
2 &= 2 \times 1 + 0 \\
\end{align}
$$
这样，我们只要把每行写成 a,b 的线性组合形式，就能获得我们想要的结果了:
$$
\begin{align}
5 &= 143 - 6 \times 23 \\
3 &= 23 - 4 \times 5  = -4 \times 143 + 25 \times 23\\
2 &= 5 - 1 \times 3 = 5 \times 143 - 31 \times 23\\
(PGCD) \ 1 &= 3 - 1 \times 2 = -9 \times 143 + 56 \times 23\\
\end{align}
$$
	不断的把上一行带入下一行。
我们还可以得到一个二阶的递推公式：
$$
\begin{cases}
u_{n+2} = u_{n} + q_{n+1}u_{n+1} \\
v_{n+2} = v_{n} + q_{n+1}v_{n+1}
\end{cases}
$$