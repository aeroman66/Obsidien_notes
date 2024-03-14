	每个概念在suite 和serie中有各自的不同的内涵。
# Convergence simple
保留奇偶性、单调性和周期性。
## Suite
Pour une suite de fonctions qui converge simplement vers f:
$$
\forall x \in X,\lim_{n\rightarrow+\infty}f_{n}(x) = f(x)
$$
	CVS
## Serie
La serie de fonctions converge simplement vers S:
$$
\lim_{n\rightarrow+\infty}S_{n} = S
$$
	1. la fonction $S:x\rightarrow \sum_{k=0}^{+\infty}f_{k}(x)$ est la somme de la serie $\sum f_{n}$
	2. Soit $n \in \mathbb{N}$, $R_{n} = S-S_{n}$ le reste d'ordre n.
R.q.:
$$
\sum f_{n} \ \text{converge} \Rightarrow (f_{n})_{n \in \mathbb{N}^{*}} \ \text{CVS ver 0}
$$

## Propriete
	以下条目都是对函数数列来说的，而不是级数
	第一条注重数列间性质
1. Conservation des inegalite
Soit  qui CVS vers :
$$
\text{Si} \ \forall n \in \mathbb{N},f_{n}\le g_{n} \ \Rightarrow f\le g
$$
	后三条讲得是数列内性质
2. Conservation de la monotonie
	所有$f_{n}$是递增的，那么$f$也是递增的
3. Conservation de la parite
4. Conservation de la periodicite

	很遗憾的是CVS完全不保留连续性和可导性

# Convergence uniforme
## Suite
1. 前置定义：
- 有界函数
$$
\mathcal{B}(X,\mathbb{K}) \ \text{L'ensemble des fonctions} \ f:X\rightarrow \mathbb{K}
$$
- 一种模长，对于有界函数来说
$$
N_{\infty} = sup_{x \in X}|f(x)|
$$
2. 定义
对于一个函数数列来说，如果converge uniformement vers f:
$$
\lim_{n\rightarrow +\infty}\|f_{n}-f\|_{\infty,I} = 0
$$
	CVU
### Propriete
1. 保留了函数的有界性
2. 在函数CVU的所有子区间上都CVU
3. 同时数列CVS
## Serie
La serie $\sum f_{n}$ converge uniformement vers $S$:
$$
\|S_{n}-S\|_{\infty} \underset{n\rightarrow +\infty}\rightarrow 0
$$
	说是级数CVU，其实就是$(S_{n})$这个数列CVU vers S，这样就跟数列的定义统一起来了。

## Propriete
- $CVU \Rightarrow CVS$
- S'il existe $(a_{n})\in \mathbb{R}^{\mathbb{N}}$ tel que:
	- $\forall x \in I,|S_{n}(x)-S(x)|\le a_{n}$
	- $\lim_{n\rightarrow +\infty} a_{n} = 0$
- $[\sum f_{n} \text{CVU vers S}] \Leftrightarrow [(R_{n}) \text{CVU vers 0}]$
- $[\sum f_{n} \text{CVU vers S}] \Leftrightarrow [(f_{n}) \text{CVU vers 0}]$

# Convergence normale-Serie seul
	这个概念仅仅针对函数级数。
尽管这是靠后才出现的概念，但是确是一个比较好证的概念，并且可以拿来推 CVU 。在实际研究中，我们经常先证明这个更加严格却好证的概念，再反过去证明 CVU。
La serie $\sum f_{n}$ converge normalment vers $S$:
- $\forall n \in \mathbb{N},f_{n}$ est bornee sur $I$
- La serie $\sum\| f_{n} \|_{\infty}$ est convergente
	通常在这里，我们需要构造出一个不取决于 x 的最大值。
## Methode pour etudier
On cherche une suite:
- $\forall n\in \mathbb{N},|f_{n}(x)| \le a_{n}$
- $\sum a_{n}$ est convergente.

## Propriete
- La serie $\sum f_{n}$ CVU
- $\forall x \in I$,La serie $\sum f_{n}$  converge absolument.
- $\exists (a_{n})_{n \in \mathbb{N}},\sum_{n \ge 0}f_{n}(a_{n})$ ne converge pas absolument, alors la serie $\sum f_{n}$ ne converge pas normalement.