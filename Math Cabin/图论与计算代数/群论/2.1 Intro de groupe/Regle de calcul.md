为了更好地进行计算，我们需要知道两个前提。
Soit $(G,*)$ un groupe:
1. L'element neutre est unique
2. Chaque element de G admet un unique symetrie
	如果没有这两个结论，有些结论我们无法得到，有时候会发生奇怪的事情。
	很好证的，是比较奇妙的证法。
# Regle de calcul
- $\forall x \in G,\bar{\bar{x}} = x$
- $\forall (x,y)\in G^{2},\bar{x*y} = \bar{y}*\bar{x}$
	细节交换顺序。但如果是commutatif就不用在意了
- $\forall (a,b) \in G^{2}$:
$$
\begin{cases}
a*x = b \Leftrightarrow x = \bar{a}*b \\
x*a = b \Leftrightarrow x = b*\bar{a}
\end{cases}
$$
	依赖 associative
- $\forall (a,b,c) \in G^{3}$:
$$
\begin{cases}
a*b = c*b \Leftrightarrow a = c \\
a*b = a*c \Leftrightarrow b = c
\end{cases}
$$
- N-ieme itere:
	我们需要分别定义 itere 次数为 0、正数、负数的情况
On peut definir le n-ieme itere de $x$ pour tout $n\in \mathbb{N}$ a l'aide de la recurrence:
$$
x^{*0} = e
$$
$$
\forall n \in \mathbb{N}, x^{*(n+1)} = x^{*(n)} * x = x * x^{*(n)}
$$
c-a-d:
$$
\forall n \in \mathbb{N}, x^{*n} = x * x * x * \cdots* x
$$
En posant:
$$
x^{*(-1)} = \bar{x}
$$
on peut definir:
$$
\forall n \in \mathbb{Z}\backslash\mathbb{N},x^{*n} = \bar{x^{*(-n)}} = \bar{x} * \bar{x} * \bar{x} \cdots * \bar{x} 
$$
#### Propriete
des calculs usuels:
- $\bar{x^{*n}} = x^{*(-n)} = \bar{x}^{*n}$
- $x^{*(p+q)} = x^{*p} * x^{*q}$
- $(x^{*n})^{*p} = x^{*np}$
## Dans la pratique
事实上，这个 composition interne 的概念是一些我们一直在使用的运算符的抽象。像是我们经常使用的实数范围内的加法乘法，就是两种 composition interne.

在现实中，我们会经常使用以下两种 composition interne :
- la notation additive
	$* = +$
- la notation multiplicative:
	$* = \times$
这两个概念都不局限于实数范围内的加减法的，后面会给出例子。

| |additive|multiplicative|
|---|---|---|
|element neutre|e = $0_{G}$|e = $1_{G}$|
|symetrie|$\bar{x} = -x$|$\bar{x} = x^{-1}$|
|loi de composition interne|$x * y = x + y$|$x * y = xy$|
|iteres|$x^{*n} = nx$|$x^{*n} = x^{n}$|
### Exemples
**Groupes additif**：
- $\mathcal{M}_{n,p}(\mathbb{R})$
- $\mathcal{T}_{n}(\mathbb{R}) = \{M \in \mathcal{M}_{n}(\mathbb{R})|^{t}M = M\}$
**Groupes multiplicatif**：
- $\mathcal{GL}_{n}(\mathbb{R})$
- $\mathcal{O}_{n}(\mathbb{R}) = \{M \in \mathcal{GL}_{n}(\mathbb{R})|^{t}M = M^{-1}\}$
#### Autres lois de composition interne
- La composition des fonctions
	这些函数值域和定义域得是相同的集合，且必须得是 bijective.