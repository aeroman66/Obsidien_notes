	其实这部分内容很接近高中的求导类似内容
# Definition
Soit $f$ une fonction definie sur un intervalle $I \subset \mathbb{R}$, on dit que F est une primitive de $f$, si F est derivable sur I et si:
$$
\forall x\in I, F^{'}(x) = f(x)
$$
## incertitude
每个primitive后面都可以加一个常数，所以就不是唯一的了
	做个拓展，如果$f$ 的定义域可以被分成很多段的话，那么F在每一段上后面加的常数都可以不同

## Theoreme fondamental de l'analyse(TFA)
Soit $f:[a,b]\rightarrow \mathbb{R}(a<b)$,continue sur $[a,b]$,alors la formation:
$$
F:x\longrightarrow \int_{a}^{x}f(t)dt
$$
est la primitive de $f$ sur $[a,b]$, qui s'annule en a.

### Notation
Une primitive quelconque F de f
$$
\forall x \in [a,b], F(x) \overset{Not}= \int f(x)dx
$$
	千万要小心primitive这个表达，因为他指向任意原函数，而这些原函数之间其实并不相等，会搞错的。

# 几种积分的方法
	有了primitive的概念事实上我们就可以开始求解积分了。
	在这里我们给出了几种计算积分的办法。

## Integration par parties
$$
\int_{a}^{b}f^{'}(x)g(x)dx = [f(x)g{x}]_{x=a}^{x=b} - \int_{a}^{b}f(x)g^{'}(x)dx
$$
	Propriete,une primitive de f'g:
	$$
	\int f^{'}(x)g(x)dx = f(x)g(x) -\int f(x)g^{'}(x)dx
	$$

## Changement de variable
$$
\int_{a}^{b}f(\phi(x))\phi^{'}(x)dx = \int_{\phi(a)}^{\phi(b)}f(t)dt
$$

	要注意计算积分与计算原函数之间的区别。计算积分最后给出的是一个实数或复数。而计算原函数最后的结果是一个函数，并且函数后面还有一个常数。

## 对称和周期性的利用
1. 奇函数，cpm sur $[-a,+a]$
$$
\int_{-a}^{+a}f(x)dx= 0
$$
2. 偶函数，cpm sur $[-a,+a]$
$$
\int_{-a}^{+a}f(x)dx = 2\int_{0}^{+a}f(x)dx
$$
3. T-periodique
$$
\forall a \in \mathbb{R},\int_{a}^{a+T}f(x)dx = \int_{0}^{T}f(x)dx
$$