	我们在这门课中研究实数或者复数数列。
	大三研究函数数列？
Les ensembles suivants sont naturellement en bijection:
$$
\mathbb{K}^{\mathbb{N}} \ et \ \mathcal{F}(\mathbb{N},\mathbb{K})
$$
每一个数列都对应一个从自然数集到数列元素的映射。
也就是我们可以拿一个函数来表示一个数列
$$
u_{n} = \psi(n)
$$
# 几个重要的基础定义
## Suite monotone
Une suite $u = (u_{n})_{n\in \mathbb{N}}\in\mathbb{R}^{\mathbb{N}}$ est dite monotone, si la fonction associee:
$$
\begin{cases}
\mathbb{N}\rightarrow\mathbb{K}    \\
n\rightarrow u_{n}
\end{cases}
 \ est \ monotone
$$
R.q.:$f:\mathbb{R_{+}}\rightarrow\mathbb{R}$ est croissantes,$(f(n))_{n\in\mathbb{N}}$ est croissante.$(f(\frac{1}{n}))_{n\in\mathbb{N^{*}}}$ est decroissante

## Convergence
si:
$$
\exists\lambda\in\mathbb{K},\forall\epsilon>0,\exists N\in \mathbb{N},\forall n\in \mathbb{N},n\ge N \Rightarrow |u_{n}-\lambda|\le\epsilon
$$
根据定义，limite是唯一的。
不converge得数列我们叫它divergente

对于一个向量数列来说，我们也可以这样定义极限，假如converge vers $\vec{\lambda}$ si
$$
\forall\epsilon>0,\exists N\in \mathbb{N},\forall n\in \mathbb{N},n\ge N \Rightarrow \|\vec{x_{n}}-\vec{\lambda}\|\le\epsilon
$$
1. 我们用距离来定义极限，跟多元函数里很像。
2. 收敛数列构成的空间是一个向量空间
3. 很多函数里的性质都可以拓展到数列上（夹逼定理）

## Relations de comparaisons
$$
u_{n} = 0_{+\infty}(v_{n})
$$
$$
u_{n} = O_{+\infty}(v_{n})
$$
$$
u_{n} \underset{+\infty} \sim v_{n}
$$
并且通常，我们可以把$+\infty$省去，因为我们默认这些关系在$+\infty$上成立。

## Suites adjacentes
Soit $a = (a_{n})_{n\in \mathbb{N}}\in\mathbb{R}^{\mathbb{N}}$ et $b = (b_{n})_{n\in\mathbb{N}}\in\mathbb{R}^{\mathbb{N}}$ deux suites reelles. On dit que ces suites sont adjacentes, sielles verifient:
1. a croissante et b decroissante
2. $(b_{n}-a_{n})_{n\in\mathbb{N}}$ est une suite convergente vers 0

# Proposition
1. Soit $u = (u_{n})_{n\in \mathbb{N}}\in\mathbb{R}^{\mathbb{N}}$ une suite monotone, alors:
$$
u \ converge \Leftrightarrow \{u_{n},n\in\mathbb{N}\} \ est \ bornee
$$
	为什么这里数列一定要是monotone的呢
	事实上从converge推导bornee并不需要monotone这一个条件。
	从bornee推导converge才需要这个条件。

2. Si a et b sont deux suites adjacents, alors elles convergent vers une meme limite.