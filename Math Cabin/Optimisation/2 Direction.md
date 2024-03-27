# Direction Réalisable
Soit $S\subseteq \mathbb{R}^{n},S \neq \emptyset$,. Un vecteur $d \in \mathbb{R}^{n}$ n'est appelé direction réalisable au point $x \in S$ si:
$$
\exists \lambda^{*} > 0,\forall \lambda \in ]0,\lambda^{*}], x + \lambda\cdot d \in S
$$
也就是说，可以沿这个方向射出一条有限长的线，都在集合内。
On notons:
$$
Z(x)
$$
# Direction de descente
比可行方向更严格，可行方向不一定是下降方向。可行方向中的一个方向 d 是下降方向如果是 x 点上的下降方向，需要满足：
$$
\exists \lambda^{*} > 0,\forall \lambda \in ]0,\lambda^{*}], f(x + \lambda \cdot d) \le f(x)
$$
如果是严格下降方向，需要满足：
$$
\exists \lambda^{*} > 0,\forall \lambda \in ]0,\lambda^{*}], f(x + \lambda \cdot d) < f(x)
$$
On notons:
$$
D(x)
$$
## Caractérisation
下降方向通常满足以下特征：
- $<\nabla f(x), d> \le 0$
- Direction de descente stricte:
$$
d = -\nabla f(x)
$$
# Direction admissible Lineaire
通常用在线性等式约束中：
On dit que $d \in \mathbb{R}^{n}$ est une direction admissible en $x \in C$ s'il existe $t > 0$ tel que:
$$
x + t \cdot d \in C
$$
## Caractérisation
$$
A \cdot (x +  t \cdot d) -  b  = t\cdot A \cdot d
$$
donc:
$$
A \cdot d = 0
$$
# Direction admissible non lineaire
为了定义这种情况下的可行方向，我们需要引入一个可行线的定义。
## Courbe Admissible
因为在非线性等式约束中，可能不存在 $t > 0$ tel que $x + t \cdot d \in C$.所以我们定义在 $x^{*}$ 上的一条可行线，considérons une courbe $x(t)$ définie pour $t \ge 0$ vérifiant:
$$
\begin{cases}
x(t) \in C ,\forall t \in [-\alpha,\alpha], \alpha > 0\\
x(0) = x^{*}
\end{cases}
$$
**Caractérisation**:
因为 $x(t) \in C$,所以 $h_{j}(x(t)) = 0$:
$$
\frac{d}{dt}h_{j}(x(t)) = 0 = <\frac{d}{dt}h_{j}(x(t)),x'(t)>
$$
On note $y = x'(0),t = 0$:
$$
<\frac{d}{dt}h_{j}(x'),y> = 0
$$
## Direction admissible
On dit que $d \in \mathbb{R}^{n}$ est une direction admissible en $x \in C$ si:
$$
\begin{cases}
x(t) \in C ,\forall t \in [-\alpha,\alpha], \alpha > 0\\
x(0) = x^{*} \\
x'(0) = d
\end{cases}
$$
换句话说，所有在 $x^{*}$ 切面上的向量都可以推出与该点梯度乘积为 0。
# Cone de Direction Admissible
