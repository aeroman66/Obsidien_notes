看内容主要都是大二内容，等后面复习的还需要补充
# Definition
我们把形如下式的级数称作 serie entiere.
我们发现它的每一项其实都是一个关于 $z$ 的函数，所以说跟我们前面学习的 convergence 的内容贯穿起来了。
$$
\sum_{n \in \mathbb{N}} a_{n} z^{n}
$$
# Rayon de convergence
在本章中，这个数列最让我们关心的就是它收敛时的情况，而对于一个 serie entiere 来说，对于收敛，我们有 RCV 这个对象来研究。
## Lemme d'Abel
这个引理告诉了我们为什么 RCV 存在，因为我们发现当 z 的取值小于某个值时，整个数列必然是绝对收敛的。
Si la suite $(a_{n}r^{n})_{n \in \mathbb{N}}$ est bornee, alors:
$$
\forall z \in \mathbb{C},|z|<r,\sum_{n \in \mathbb{N}}a_{n}z^{n} \text{est absolument convergente}
$$
## Formalisme
这个理论告诉了我们这个区间的形状是怎么样的，也就是收敛区间的几种可能性。
$$
E_{1} = \{ \rho\in \mathbb{R}_{+},(a_{n}\rho^{n}) \ \text{borne} \}
$$
cet ensemble est un intervalle de la forme:
$$
[0,R],[0,R[,R = +\infty
$$
## Definition
Soit $\sum_{n \in \mathbb{N}} a_{n} z^{n}$ un serie entiere, on appelle rayon de convergence de la serie entiere:
$$
R = \sup\{ \rho \in \mathbb{R}_{+},(a_{n}\rho^{n}) \ \text{bornee} \}
$$
d'apres la formalisme, il y a deux cas:
$$
R \in \mathbb{R}_{+},R = +\infty
$$
### Definitions equivalentes
$$
\begin{align}
E_{1} &= \{ \rho \in \mathbb{R}_{+},(a_{n}\rho^{n}) \ \text{borne} \} \\
E_{2} &= \{ \rho \in \mathbb{R}_{+},(a_{n}\rho^{n}) \ \text{tend vers 0} \} \\
E_{3} &= \{ \rho \in \mathbb{R}_{+},(a_{n}\rho^{n}) \ \text{converge} \} \\
E_{4} &= \{ \rho \in \mathbb{R}_{+},(a_{n}\rho^{n}) \ \text{converge absolument} \}
\end{align}
$$
Alors $[0,R[\subset E_{1} \subset E_{2} \subset E_{3} \subset E_{4} \subset [0,R]$ ou R est le rayon de convergence de la serie

# Propriete
1. Trois cas
	- $|z|<R$,absolument convergence 
	- $|z|>R$, grossierement divergente
	- $|z|=R$, on ne sait pas ce qui se passe
2. Comparaison
Soit $R_{a},R_{b}$ les rayons de convergences des series entieres $\sum a_{n}z^{n},\sum b_{n}z^{n}$,alors:
- $|a_{n}|\le|b_{n}|$ ou $a_{n} = o(b_{n})$ ou $a_{n} = O(b_{n})$,alors $R_{a}\ge R_{b}$
- $a_{n} \sim b_{n}$, alors $R_{a} = R_{b}$
- Les serie $\sum a_{n}z^{n},\sum na_{n}z^{n}$ ont le meme RCV.
- Regel de D'Alembert
Soit $\sum_{n \in \mathbb{N}} a_{n} z^{n}$ un serie entiere telle qu'a partir d'un certain rang $a_{n} \ne 0$, on suppose qu'il existe $l \in \mathbb{R}_{+}\cup \{ +\infty \}$ tel que:
$$
\lim_{n\rightarrow +\infty} |\frac{a_{n+1}}{a_{n}}| = l
$$
Alors le RCV est:
- $\frac{1}{l}$ si $l \in ]0,+\infty[$
- $+\infty$ si $l = 0$
- 0 si $l = +\infty$

# Theoreme
Soit $\sum_{n \in \mathbb{N}} a_{n} z^{n}$ un serie entiere definie sur $\mathbb{R}$. Notons R son RCV,alors:
1. $\sum_{n \in \mathbb{N}} a_{n} z^{n}$ CVS sur $]-R,R[$
2. $\sum_{n \in \mathbb{N}} a_{n} z^{n}$ CVU sur tout segment de $]-R,R[$
