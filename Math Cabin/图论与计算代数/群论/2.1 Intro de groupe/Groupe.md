	也像是引子的作用，主要介绍了群论的主题和一些重要的概念和操作。分成了三部分。
# Groupe
	群，那应该是群论的研究对象了
定义：
Un groupe est la donne de $(G,*)$ ou:
1. G est un ensemble
2. \* est une application de 
$$
\begin{cases}
G\times G \longrightarrow G \\
(a,b) \longrightarrow a*b
\end{cases}
$$
	Loi de composition interne
	这个定义里还隐含了stabilite par composition interne.
tels que:
- element neutre
	$\exists e \in G,\forall x \in G,e*x = x*e = x$
	一定要两个方向都满足
- symetrique
	$\forall x \in G,\exists \bar{x}\in G,x*\bar{x} = \bar{x}*x = e$
	同样也需要两个方向都满足
- associativite(结合律)
	$\forall(x,y,z)\in G^{3},x*(y*z) = (x*y)*z$
	通常我们把这个记作$x*y*z$
## E.g.
- $(\mathbb{N},+)$
	不是一个groupe，因为尽管有EN，但是对于任何非零元素，都不存在symetrie,应该是个负数，但负数不属于自然数范围。
- $(\mathbb{Z},+)$
	是groupe
- $(\mathbb{Z},\times)$
	不是，因为symetrie可能不是整数
- $(\mathbb{Q},\times)$
	不是，因为0没有symetrie，怎么乘都得不到1
- $(\mathbb{Q}^{*},\times),(\mathbb{R},+),(\mathbb{R}^{*},\times),(\mathbb{R}^{*}_{+},\times),(\mathbb{C},+),(\mathbb{C}^{*},\times)$
	是的
	而且看上去涉及乘法的要把0剔除掉。

	以上这些还是很好判断的，有一个概念就行
## 拓展概念
## 阿贝尔群（交换群）
groupe commutatif,groupe abelien 定义：
$$
\forall (x,y)\in G^{2},x*y = y*x
$$
## 有限群
groupe fini 定义：
$$
\text{G est un ensemble fini}
$$
On appelle l'ordre de groupe sa cardinal:
$$
|G| = \text{card(G)}
$$
	与后文 element 的 ordre 要做区分
## E.g.
Les racines n-iemes de l'unite
$$
\mathbb{U}_{n} = \{z \in \mathbb{C}|z^{n}=1\} = \{e^{i\frac{2k\pi}{n}}|k\in ([0,n-1]\cap \mathbb{Z})\}
$$
$(\mathbb{U}_{n},\times)$est un groupe commutatif fini d'ordre n