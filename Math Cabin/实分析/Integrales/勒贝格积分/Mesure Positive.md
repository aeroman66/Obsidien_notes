# 前置定义
## Topologie
	事实上，这里更应该叫Topologie ouvert,因为他是一个开集系，但是我们这里把它笼统地称作Topologie.
Topologie sur $\Omega$ , la donne d'une partie $\mathcal{T}\mathcal{O}$ de $\mathcal{P}(\Omega)$:
	是所有子集构成的集合的子集，我们只能选取子集中的开集来组成拓扑。
1. $\emptyset \in \mathcal{T}\mathcal{O}$ et $\Omega \in \mathcal{T}\mathcal{O}$  
	这个构成了我们能构造的最简单的$\mathcal{T}\mathcal{O}$
2. $\forall (O_{i})_{i \in I} \in \mathcal{T}\mathcal{O}^{I},\underset{i\in I}\cup O_{i} \in \mathcal{T}\mathcal{O}$
	reunion quelconque
3. $\forall n \in \mathbb{N} \forall (O_{1},\dots,O_{n}) \in \mathcal{T}\mathcal{O}^{n}, \underset{k=1}\cap^{n} O_{k}\in \mathcal{T}\mathcal{O}$
	intersection finie
	联系开集的性质我们就可以知道，如果允许无限个开集相交，是可以获得闭集的。

## $\sigma$-algebre
	Tribu
La donne d'un sous-ensemble $\mathcal{T}$ de $\mathcal{P}(\Omega)$:
1. $\emptyset \in \mathcal{T}$
2. $\forall A\in \mathcal{T},A^{C} = \Omega \textbackslash A \in \mathcal{T}$
	Stabilite par passage au complementaire.
3. $\forall (A_{n})_{n\in\mathbb{N}} \in \mathcal{T}^{\mathbb{N}},\underset{n\in\mathbb{N}}\cup A_{n} \in \mathcal{T}$
	Stabilite par reunion denombrable.

	$(\Omega,\mathcal{T})$ est dit espace mesurable.
	Les parties de $\mathcal{T}$ sont dites parties mesurables.

### Tribu Borelienne--一个很重要的例子
	tribu borelienne是一个topologie
最小的包含了所有开集的tribu。
$\mathcal{BO}(\Omega)$

### Tribu Produit
	$\sigma$-代数积

$(\Omega_{1},\mathcal{T}_{1}),(\Omega_{2},\mathcal{T}_{2})$, On a tribu produit sur $\Omega_{1} \times \Omega_{2}$,$\mathcal{T}_{1}\bigotimes\mathcal{T}_{2}$ la plus petite tribu contenant les $T_{1} \times T_{2}$, ou $T_{1} \in \mathcal{T}_{1},T_{2} \in \mathcal{T}_{2}$

## 完备$\sigma$-代数
	Tribu $\mu$-completee de T
	让我们 从Borel可测集进入了Lesbegue可测集，勒贝格可测集都是完备的。
Soit $(\Omega,\mathcal{T},\mu)$ un espace mesure, on pose:
$$
\mathcal{N} = \{N\subset\Omega,N \ \mu-negligeable\}
$$
On appelle tribu $\mu$-negligeable de $\mathcal{T}$ la tribu definie par:
$$
\mathcal{T}^{*}\overset{Not}=\{T\cup N,T\in\mathcal{T},N\in\mathcal{N}\}
$$
La mesure $\mu$ se prolonge a $\mathcal{T}^{*}$ par
$$
\forall A\in \mathcal{T}^{*},\mu^{*}(A) = \mu(T) \ ou \ A = T \cup N,T\in\mathcal{T},N\in\mathcal{N}
$$
	可以发现，就是把那些零测集加了进去，让这个tribu显得更加的完备

# Mesure Positive
	测度！

Toute application $\mu$ de $\mathcal{T}$ dans $\mathbb{R}_{+} \cup \{+\infty\}$
1. $\mu(\emptyset) = 0$
2. si $(A_{n})_{n\in\mathbb{N}}\in \mathcal{T}^{N}$ est une famille de parties mesurables 2 a 2 disjointes, alors
$$
\mu\left(\underset{n\in\mathbb{N}}\cup A_{n}\right) = \underset{n\in\mathbb{N}} \sum \mu(A_{n})
$$
	注意对A的要求！！！
	Le triplet $(\Omega,\mathcal{T},\mu)$ est appele espace mesure.

	因为这里定义了测量方法，所以所以用词从mesurable变成了mesure。

## Remarque
Lorsque l'un des $A_{n}$ est de mesure infinie ou lorsque la serie $\sum \mu(A_{n})$ diverge, nous conviendrons que:
$$
\underset{n\in\mathbb{N}} \sum \mu(A_{n}) = +\infty
$$
sinon,nous poserons:
$$
\underset{n\in\mathbb{N}} \sum \mu(A_{n}) = \sum_{n=0}^{+\infty} \mu(A_{n})
$$
## Propriete
	一些测度的性质
1. la croissance
$$
\forall(A,B)\in\mathcal{T}^{2},[A\subset B]\Rightarrow[\mu(A)\le\mu(B)]
$$
2. de plus
$$
\forall(A,B)\in\mathcal{T}^{2},\mu(A)+\mu(B) = \mu(A\cup B) + \mu(A\cap B)
$$
	交的部分要算两次
3. limite croissante
$$
\forall(A_{n})_{n\in\mathbb{N}} \in \mathcal{T}^{\mathbb{N}},[\forall n\in\mathbb{N},A_{n}\subset A_{n+1}] \Rightarrow \left[ \mu \left( \underset{n\in\mathbb{N}}\cup A_{n} \right) = \lim_{n\rightarrow +\infty}\mu(A_{n})\overset{Not}=\lim_{n\rightarrow +\infty}\uparrow\mu(A_{n}) \right]
$$
4. limite decroissante
$$
\forall(A_{n})_{n\in\mathbb{N}} \in \mathcal{T}^{\mathbb{N}},[\forall n\in\mathbb{N},A_{n+1}\subset A_{n} \ et \ \mu(A_{0})\ne +\infty ]\Rightarrow \left[ \mu \left( \underset{n\in\mathbb{N}}\cap A_{n} \right) = \lim_{n\rightarrow +\infty}\mu(A_{n})\overset{Not}=\lim_{n\rightarrow +\infty}\downarrow\mu(A_{n}) \right]
$$
5. Sous-additivite
$$
\forall(A_{n})_{n\in\mathbb{N}} \in \mathcal{T}^{\mathbb{N}},\mu\left(\underset{n\in\mathbb{N}}\cap A_{n}\right)\le\sum_{k\in\mathbb{N}}\mu(A_{k})
$$
	个人对最后一条的理解，两个A之间的交集可能不为空

## Exemple
$(\Omega,\mathcal{T},\mu)$:
$\Omega$:样本
$\mathcal{T}$:事件集合
$\mu$:概率

## 勒贝格测度——例子
	我们将这个测度记为$\lambda$
Mesure de Lebesgue sur la tribu borelienne de $\mathbb{R}$
$$
\forall (a,b) \in \mathbb{R}^{2},[a\le b] \Rightarrow \left[ \lambda(]a,b[)\overset{Def} = b-a \right]
$$
Mesure de Lebesgue sur la tribu borelienne de $\mathbb{R}^{n}$
$$
\lambda\left(\prod_{k=1}^{n}]a_{k},b_{k}[\right)\overset{Def}=\prod_{k=1}^{n}(b_{k}-a_{k})
$$

# 由测度引申出的概念
## $\mu$-negligeable
On dit que A est $\mu$-negligeable,si:
$$
\exists T\in\mathcal{T},A\subset T \ et \ \mu(T)=0
$$
	T本身也是$\mu$-negligeable的
### Exemple
1. $\mathbb{Q}$ est un ensemble $\lambda$-negligeable de $\mathbb{R}$

### *p.p.*
P est vraie ($\mu$-)presque partout si
$$
\{\omega\in\Omega,P(\omega) fausse\} \ est \ \mu-negligeable
$$ 