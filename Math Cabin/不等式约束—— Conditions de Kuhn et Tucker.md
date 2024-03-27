在不等式约束中，我们关注形如下面的问题：
$$
(\mathcal{PCI})
\begin{cases}
\inf_{x\in C}f(x) \\
s.c. \ g(x) \le 0
\end{cases}
$$
假设有 n 个变量，有 p 条不等式约束。
解决不等式约束的主要思想是，在我们最终想要的极值点上，部分起到作用的约束，可以表示为：
$$
g_{i}(x^{*}) = 0
$$
我们把这些约束称为积极约束，Contrainte active，并记作：
$$
A(x^{*}) = \{ i \in [| 1,p |] \ | \ g_{i}(x^{*}) = 0 \}
$$
而没起到作用的约束就相当于不存在。
但是因为我们在求解问题的过程中并不知道哪些约束最终起作用哪些没有，因此实际问题通常没有这么简单。
# Conditions de Kuhn et Tucker
Soit $x \in C$ un point régulier solution du problème sous contraintes d’inégalité. Alors il existe un unique vecteur $\mu \in \mathbb{R}^{p}$ tel que:
$$
\nabla f(x^{*}) + \sum_{j = 1}^{q}\mu_{j}\nabla g_{j}(x^{*}) = 0
$$
其中：
$$
\mu_{i} \ge 0, i\in [| 1,\dots,p |]
$$
$$
\mu_{i}\cdot g_{i}(x^{*}) = 0, i\in [| 1,\dots,p |]
$$
**核心思想**：
这里的原理很 tricky，表现了数学对某种统一性的追求。
我们知道，对于一个约束来说，要么它是积极约束，这样我们用拉格朗日乘数法就可以解决它，得到：
$$
\lambda_{i} > 0, g_{i}(x^{*}) = 0 \Rightarrow \mu_{i}\cdot g_{i}(x^{*}) = 0
$$
要么这个约束压根没起作用，那么为了表达式的统一性，我们强制拉格朗日乘子为 0:
$$
\lambda_{i} = 0, g_{i}(x^{*}) < 0 \Rightarrow \mu_{i}\cdot g_{i}(x^{*}) = 0
$$
这样我们就得到了库恩塔克条件里的 $\lambda$
# Conditions de Karush, Kuhn et Tucker
KKT. 是对前面情况的推广，用于解决既有不等式约束又有等式约束的情况。
## 约束规范
Qualifications des contraintes。这是为了保证我们的约束不会约束过紧或者约束过松，导致我们最后得出的结果不是最优的结果。我们称 $\bar{x}$ 上的约束是规范的如果满足：
- 所有的向量 $\nabla h_{j}(x^{*})$ 是线性独立的。
- 存在方向 d，满足：
$$
<\nabla g_{j}(\bar{x})> \le 0,<\nabla h_{j}(\bar{x})> = 0
$$

## KKT