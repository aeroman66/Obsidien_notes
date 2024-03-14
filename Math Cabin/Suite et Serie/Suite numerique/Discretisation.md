之前研究的函数的性质都是连续的，而数列是一个离散的对象。我们可以把函数中的很多性质通过数列表现为离散形式，并且还是成立的。我们把这一过程称作离散化。

# Limite
$$
f(x)\underset{x\rightarrow a}\longrightarrow \lambda \Leftrightarrow\left[\forall(x_{n})_{n\in\mathbb{N}}\in I^{\mathbb{N}},x_{n}\underset{n\rightarrow +\infty}\longrightarrow a \Rightarrow f(x_{n})\underset{n\rightarrow +\infty}\longrightarrow \lambda\right]
$$

# Continuite
$$
f(x) \ continue \ en \ a \Leftrightarrow\left[\forall(x_{n})_{n\in\mathbb{N}}\in I^{\mathbb{N}},x_{n}\underset{n\rightarrow +\infty}\longrightarrow a \Rightarrow f(x_{n})\underset{n\rightarrow +\infty}\longrightarrow f(a)\right]
$$
# u-continue
$$
f(x) \ u-continue \ sur \ I \ \Leftrightarrow\left[\forall((x_{n})_{n\in\mathbb{N}},(y_{n})_{n\in\mathbb{N}})\in (I^{\mathbb{N}})^{2},x_{n}-y_{n}\underset{n\rightarrow +\infty}\longrightarrow 0 \Rightarrow f(x_{n}) - f(y_{n})\underset{n\rightarrow +\infty}\longrightarrow 0\right]
$$
	注意u-continue的定义噢,他保证了一个函数的光滑性：
	$$
	\forall \epsilon>0,\exists\eta>0,\forall(x,y)\in I^{2},|x-y|\le\eta\Rightarrow |f(x)-f(y)|\le \epsilon
	$$

	后面我们继续对函数的连续性做拓展
	不清楚这些拓展的应用是什么，而且是在不动点中讲得这些概念。