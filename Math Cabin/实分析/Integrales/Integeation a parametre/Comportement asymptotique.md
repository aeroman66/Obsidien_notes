我们想要研究的都是一个含参积分在他的参数（也就是自变量而不是积分变量）趋向于正无穷或者 0 的时候，函数趋向于什么函数。
以下列举几种常用的方法。
1. Estimation de l'ordre de l'equivalent et utilistion des theoremes de convergence
$$
f(x) = \int_{0}^{+\infty}\frac{dt}{(1 + t^{2})\sqrt{(x^{2} + t^{2})}} \underset{x \rightarrow +\infty}\sim \int_{0}^{+\infty}\frac{dt}{(1 + t^{2})x} = \frac{\pi}{2x}
$$
2. Localisation de la masse et comparaison au comportement dominant
$$
f(x) = \int_{0}^{+\infty}\frac{dt}{\sqrt{(1 + t^{2})(x^{2} + t^{2})}} \underset{x \rightarrow 0^{+}}\sim \int_{0}^{+\infty}\frac{dt}{\sqrt{x^{2} + t^{2}}} \underset{x \rightarrow 0^{+}}\sim -\ln(x)
$$
3. Fixation des bornes(把积分上下界固定为常数)
$$
\int_{0}^{x}\sqrt{\frac{1 + t^{2}}{x^{2} - t^{2}}}dt = \int_{0}^{1}\sqrt{\frac{1 + x^{2}u^{2}}{1 - u^{2}}}du \underset{x \rightarrow 0^{+}}\longrightarrow \frac{\pi}{2}
$$
3. 1. A contrario(跟上面相反，把积分上下阶变为变量)
$$
\int_{1}^{+\infty}\frac{e^{-x^{2}t^{2}}}{t}dt = \int_{x}^{+\infty}\frac{e^{-u^{2}}}{u}du \underset{x \rightarrow +\infty}\sim \frac{e^{-x^{2}}}{2x^{2}}
$$
4. Methode de Laplace
对于特定的函数形式：
$$
F(x) = \int_{a}^{b}\phi(t)e^{x f(t)}dt
$$
在参数 $x$ 较大时候的渐进估值或者说是当 $x \rightarrow +\infty$ 时的渐近展开。其主要思想是，如果 $f$ 在区间 $[a, b]$ 中某个点  $t_{0}$ 达到绝对最大，则对于较大或者极速增长的 $x$ 而言， $e^{xf(t)}$ 在 $t_{0}$ 的取值会远大于其他点的取值，从而 $t_{0}$ 的邻域对于整个积分占据绝大部分贡献，其余部分的积分几乎是非实质的。
$$
\int_{0}^{+\infty} \frac{e^{-t}}{(t^{2} + t + 1)^{x}} dt
$$
- Cas academique