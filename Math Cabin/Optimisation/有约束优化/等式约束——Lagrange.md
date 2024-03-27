# Contraintes d’égalité linéaires
我们先关注形如下面的问题：
$$
(\mathcal{PCE})
\begin{cases}
\inf_{x\in C}f(x) \\
s.c. \ Ax - b = 0
\end{cases}
$$
可以看出，这里的等式约束是一种线性约束，因为它们被表示成了线性方程组的形式。
## Existence des multiplicateurs de Lagrange
假设我们有 q 条等式约束，并且我们已经找出了一个极值点 $x^{*}$ ，那么一定存在一个向量拉格朗日乘子 $\lambda \in \mathbb{R}^{q}$:
$$
\nabla f(x^{*}) - A^{\top} \cdot \lambda = 0
$$
**Demonstration**:
Soit d un direction admissible en $x^{*}$,
$$
f(x^{*}) \le f(x^{*} + t\cdot d) = f(x^{*}) + <\nabla f(x^{*}),t\cdot d> + o(\|x^{*}\|)
$$
因为 $x^{*}$ 是最小值，所以：
$$
<\nabla f(x^{*}),t\cdot d> = 0
$$
comme:
$$
A \cdot d = 0, d\in Ker(A)
$$
on a:
$$
\nabla f(x^{*}) \in (Ker(A))^{\top} = Im(A^{\top})
$$
所以存在 $\lambda \in \mathbb{R}^{q}$：
$$
\nabla f(x^{*}) = -A^{\top}\cdot \lambda
$$
## 原理
将等式约束看作一个函数：
$$
g(x) = Ax - b
$$
事实上，拉格朗日乘子想要我们求解的是目标函数和等式约束函数的梯度共线的时候的解：
$$
\nabla g = A 
$$
	这里梯度的解释存疑。线性情况下应该不是用梯度来解释。
见视频![https://www.bilibili.com/video/BV15T411f7DY/?spm_id_from=333.337.search-card.all.click&vd_source=d53a375084b7127af1236ed8b485b543]
# Contraintes d’égalité non linéaires
在非线性约束中，我们关注形如下面的问题：
$$
(\mathcal{PCE})
\begin{cases}
\inf_{x\in C}f(x) \\
s.c. \ h(x) = 0
\end{cases}
$$
假设有 n 个变量，有 q 条等式约束。
**Point Régulier**:
我们说 $x^{*}$ 是一个 $h(x) = 0$ 约束下的 point régulier 如果他满足以下性质：
- $h(x^{*}) = 0$
- 所有的向量 $\nabla h_{j}(x^{*})$ 是线性独立的。
## Theoreme de Lagrange
我们已经找出了一个极值点 $x^{*}$ 是一个 point régulier ，那么一定存在一个向量拉格朗日乘子 $\lambda \in \mathbb{R}^{q}$:
$$
\nabla f(x^{*}) + J_{h}^{\top}(x^{*}) \cdot \lambda = 0
$$
也即：
$$
\nabla f(x^{*}) + \sum_{j = 1}^{q}\lambda_{j}\nabla h_{j}(x^{*}) = 0
$$
原理同上面解释的，梯度共线时在约束条件下取到最小值。
# Conclusion
我们构造一个拉格朗日函数如下：
$$
L(\vec{x}) = f(\vec{x}) - \lambda h(\vec{x})
$$
我们有：
$$
\nabla L = 0 \Leftrightarrow 
\begin{cases}
\nabla f(\vec{x}) = \lambda \nabla h(\vec{x}) \\
h(\vec{x}) = 0
\end{cases}
$$
**利用拉格朗日乘数法的条件**：
与隐函数定理有关。