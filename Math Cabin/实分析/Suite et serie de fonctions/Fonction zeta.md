$$
\zeta(x) = \sum_{n=1}^{+\infty}\frac{1}{n^{x}}
$$
# Domaine de definition
Par critere de Riemann $\zeta$ est definie pour:
$$
x \in ]1,+\infty[
$$
在 1 以内，这个级数是不收敛的，所以是没有定义的。

# 前置研究
知道了定义域，我们可以进行一些前置研究
- **H1** $\mathcal{C}^{k}$ de  $\frac{1}{n^{x}}$
Soit $k \in \mathbb{N},x\longmapsto f_{n}(x) = \frac{1}{n^{x}}$ est $\mathcal{C}^{k}$ sur $]1,+\infty[$
On demontre par recurrence que:
$$
\forall j \in [| A,+\infty |],
f^{(j)}(x) = (-\ln n)^{j}\frac{1}{n^{x}}
$$
我们证明了这个函数是 k 次可导的。
- **H2** 导函数级数收敛
Soit $A>0,x\in [A,+\infty]$, 我们有：
$$
\forall j \in [| 0,k |],
|f^{(j)}(x)| \le \frac{1}{n^{A}(\ln n)^{-j}}
$$
我们有了一个 serie de Bartrand avec $\alpha = A >1$,donc:
$$
\sum f^{(j)}(x) \ \text{CVN sur}[A,+\infty[
$$
所以说这个时候，$\zeta$ 也是有定义的因为级数收敛。
- **C1** $\zeta$ est $\mathcal{C}^{k}$ sur $[A,+\infty[$
- **C2** $\forall j \in [| 0,k |],\zeta^{(j)}(x) = \sum_{n=1}^{+\infty}\frac{(\ln n)^{j}}{n^{x}}$
通过以上的推导，我们才得出我们最终想要的结论：
$$
\zeta \ \text{est} \ \mathcal{C}^{k} \ \text{sur} \ \cup_{A>1}[A,+\infty[ = ]1,+\infty[
$$
# Monotonie
On sait que:
$$
\zeta^{'}(x) = \sum_{n=1}^{+\infty}-\frac{\ln n}{n^{x}} \le 0
$$
所以说在 $]1,+\infty[$ 上是递减的

# Convexe
On sait que:
$$
\zeta^{'}(x) = \sum_{n=1}^{+\infty}\frac{(\ln n)^{2}}{n^{x}} \ge 0
$$
所以说在定义域上是 Convexe 的。

# Inegalite
Finalement:
$$
\frac{1}{x-1} \le \zeta(x) \le 1+\frac{1}{x-1}
$$
并且在 x 趋向于 1 的时候：
$$
1+\frac{1}{x-1} \underset{1^{+}}\sim \frac{1}{x-1}
$$
donc:
$$
\zeta(x)\underset{1^{+}}\sim \frac{1}{x-1}
$$
	夹逼定理吧