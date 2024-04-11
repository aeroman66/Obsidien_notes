Méthode de gradient，这是解决最优化问题中最常用的方法。
这里我们感兴趣的目标函数是凸函数，所以根据前面讲到的凸优化充要条件，这样的最优化问题就变成了寻找目标函数梯度为 0 的点。
$$
\nabla f(x) =
\begin{bmatrix}
\frac{\partial f}{\partial x_{1}}(x_{1},\dots,x_{n}) \\
\vdots \\
\frac{\partial f}{\partial x_{n}}(x_{1},\dots,x_{n}) \\
\end{bmatrix}
=
\begin{bmatrix}
0 \\
\vdots \\
0 \\
\end{bmatrix}
$$
# 决定步长
三种通用的梯度下降方法，适用于函数光滑、变量简单和梯度好算的情况。
## 固定步长
Un pas fixe:
$$
\forall k \in \mathbb{N}, \delta_{k} = \delta
$$
## Pas de Descente Optimale
On definie:
$$
\arg \min f \overset{\text{def}}= \left\{ x \in \mathbb{R}^{n}| \forall x' \in \mathbb{R}^{n}, f(x')\ge f(x) \right\}
$$
我们有最优步长为：
$$
\delta* = \arg \min_{\delta > 0} f (x + \delta \cdot d)
$$
在我看来这个方法几乎没有现实可行性，如果能知道最优步长为什么我们还需要梯度下降
## Pas de Descente par Rebroussement
在我们无法求解出最优步长的时候，我们就可以用这种方法。
我们想要保证每步下降有着充足的下降量。具体的做法是，先取一个足够大的步长，然后慢慢的将其缩小，直至下降量令我们满意为止。
- Condition d'Armijo
这个条件让我们判断一步下降的下降量是否足够大，其数学表示形式为：
$$
f(x_{k+1}) = f(x_{k} + \alpha d_{k}) \le f(x_{k}) + c \alpha \nabla f(x_{k})^{\top}d_{k}
$$
这个式子有及其显著的几何意义，那就是，我们以步长 $\alpha$ 为自变量，我们要新取得下降点必须在直线
$$
l(\alpha) = f(x_{k}) + c \nabla f(x_{k})^{\top}d_{k} \ \alpha 
$$
以下。该直线斜率与 $x_{k}$ 处的梯度有关，是被 $c \in [0,1[$ 放缩后的结果，可以根据我们的需要进行调节。
- Pas de Armijo
某种使 Condition d'Armijo 成立的最大的步长, soit $c \in [0,1[, \beta \in [0,1[$：
$$
\tau = \max\{ b^{n},n \in \mathbb{N}, f(x_{k} + b^{n} d_{k}) \le f(x_{k}) + c b^{n} \nabla f(x_{k})^{\top}d_{k}\}
$$
- Pas de Descente par Rebroussement
基本就是取 Pas de Armijo。
$$
\delta^{*} = b^{N}
$$
# 决定下降方向
Algorithme de descente de gradient:
$$
d_{k} = -\nabla f(x)
$$
# Convergence