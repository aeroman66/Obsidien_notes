# Boule
Boule ferme (de centre a et de rayon r)
1. $BF(a,r)$
Boule ouverte
1. $BO(a,r)$
Sphere
1. $S(a.r)$

	Remarque:以上三个定义与距离有关，通常我们会在右下角表上定义它的距离。

# Partie bornee
	在这里我们讲了三种bornee的形式。
Une partie d'un espace metrique est bornee
1. 
	Une propriete,3 assertions suivantes sont equivalentes
	1. A est bornee
	2. $\forall x \in E, \exists r \in \mathbb{R}^{*}_{+},A \subset BO(x,r)$
	3. $diam(A) <+\infty$
Une suite est bornee
1. 
Une fonction est bornee
1. 

# Ferme
	我们还需要一个前置定义
## Suite convergente
1. 

## Ferme
定义
	On dit que F est un ferme de E (dans E)

Pour montrer qu'une partie F est ferme dans E
1. 
2. 
	Remarque importante:
	E est importante pour dire si F est ferme ou non.
	ex:

## Operations sur ferme
1. $\emptyset$,E 永远是E上的闭集
2. 闭集的交集是闭集
3. 闭集的有限并集是闭集

## Propriete
ferme et distance nulle
1. 

# 由ferme延伸出的概念
## Adherence
定义：
	Le plus petit ferme de E contenant A.
性质：
1. 包含于所有包含了A的闭集中。
2. Adherence de A 是所有由A元素构成的数列的极限组成的。
3. 这个概念也跟E有关，不同的E可能会有不同的Adherence
4. $[x \in \overline{A}] \leftrightarrow [\forall \epsilon > 0,\exists a \in A,a\in BO(x,\epsilon)]$
5. Adherence d'une boule ouverte. P62
6. 三个基本性质
	1. $A \in \overline{A}$
	2. $[A = \overline{A}] \leftrightarrow [A est ferme dans F]$
	3. $\overline{\overline{A}} = \overline{A}$
7. 三个集合运算与之相关的基本性质
	1. $[A \in B] \rightarrow [\overline{A} \in \overline{B}]$
	2. $\overline{A\cup B} = \overline{A} \cup \overline{B}$
	3. $\overline{A \cap B} \subset \overline{A} \cap \overline{B}$

## Partie dense
	On dit que A est dense dans E.
定义
1. 
一些例子
1. 
