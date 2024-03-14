我们可以有
$$
f_{n}\underset{n\rightarrow+\infty}\longrightarrow f
$$
但这样我们就会面临两个问题，我们想知道下面这两件事是否成立：
$$
\int_{\Omega}f_{n}\underset{n\rightarrow+\infty}\longrightarrow\int_{\Omega}f
$$
$$
f_{n} \ integrable \ \longrightarrow \ f \ integrable
$$
	课件中就有两个例子说明这两种情况并不是任何时候都是成立的。

# Convergence monotone
	注意，这里用到的函数都得是正的并且可测的。在证明过程中应该证明以上两点。
Soit $(\Omega,\mathcal{T},\mu)$ un espace mesure et $(f_{n})_{n\in\mathbb{N}}$ une suite croissante de fonctions positives, mesurables sur $\Omega$
$$
\forall n \in \mathbb{N},\forall\omega\in\Omega,f_{n}(\omega)\le f_{n+1}(\omega)
$$
Alors:
1. 存在一个正的可测函数
$$
\forall \omega\in\Omega,f(\omega) = \lim_{n\rightarrow+\infty}\uparrow f_{n}(\omega)
$$
2. On a:
$$
\int_{\Omega}fd\mu = \lim_{n\rightarrow+\infty}\uparrow \left(\int_{\Omega}f_{n}d\mu\right)
$$
我们这里只是求出了$f$的积分值，但是他不一定是可积的，事实上，积分值小于正无穷和是否可积并不一定。

	事实上，单调收敛定理允许我们将积分号与极限号运算符的位置进行互换。

## 离散点的函数极限
	在这样由函数构成的数列中很可能用到
La discretisation de la limite d'une fonction en un point
$$
\left[f(x)\underset{x\rightarrow a}\lambda\right]\Leftrightarrow\left[\forall(x_{n})_{n\in\mathbb{N}}\in I^{\mathbb{N}},\left[x_{n}\underset{n\rightarrow+\infty}\longrightarrow a\right]\Rightarrow\left[f(x_{n})\underset{n\rightarrow +\infty}\longrightarrow \lambda\right]\right]
$$
我们可以令上面x的数列是单调的，还可以得到相同的结果。这叫做discretisation monotone.

## Limite superieur/inferieur
$$
\lim_{n\rightarrow +\infty}\sup u_{n} \overset{Not}= \max(Adh(u)) \in [-\infty,+\infty]
$$
$$
\lim_{n\rightarrow +\infty} \inf u_{n} \overset{Not}= \min(Adh(u)) \in [-\infty,+\infty]
$$
	这两个是两个完整的概念，但是我们书上没有介绍他们
以数列下极限为例：
$$
\lim_{n\rightarrow +\infty} \inf u_{n} = \lim_{k\rightarrow +\infty}\inf_{n \ge k} u_{n}
$$
	因为我们要取的是无穷远处的最小值，所以只能取子列趋向极限的最小值。
Transformer une limite inferieur en limite croissante,en remarquant que:
$$
\lim \inf u_{n} = \lim_{n\rightarrow+\infty}\uparrow\left(\inf_{k\ge n}u_{k}\right)
$$
我们可以得出几个结果：
1. 所有可测函数列的limite inferieur是可测的
2. 所有可测函数列的limite superieur是可测的
3. 所有可测函数列极限的函数是可测的。

### Lemme de Fatou
	说明一个函数列的下极限的积分和这个函数列的积分的下极限存在不等关系。
	法图引理事实上是单调收敛定理的一种推广。
所有函数必须的positive, mesurable的
事实上在我们处理问题的时候，我们并不是总能很理想的获得一串单调递增的函数列。因此，根据上面lim inf的构造，我们可以在这样一个不单调的函数列中构造出一个单调的函数列。通过这个做法，我们可以把单调收敛中的croissante条件去掉,但是，由此得到的是一个不等关系。
对于$k \ge 1$,令$g_{k} = \inf\limits_{n\ge k}f_{n}\le f_{k}$满足:
1. $g_{k} \ge 0$
2. $\{g_{k}\}$单调增
3. $\lim\limits_{n\rightarrow +\infty} \inf u_{n} = \lim\limits_{k\rightarrow +\infty}\inf_{n \ge k} u_{n} = \lim\limits_{k\rightarrow +\infty}g_{k}$

$$
\int_{\Omega}\lim\inf f_{n}d\mu \le \lim \inf \int_{\Omega}f_{n}d\mu
$$
Version inverse:
$$
\int_{\Omega}\lim\sup f_{n}d\mu \ge \lim \sup \int_{\Omega}f_{n}d\mu
$$
# Convergence dominee
	单调收敛的条件太强了，只有有些时候这个定理适用。我们需要一个更强的定理，这样它的条件可以弱一点。
一群可测函数如果满足以下两条假设：
1. Convergence simple de la suite
$$
f_{n}(\omega)\underset{n\rightarrow +\infty}\longrightarrow f(\omega) \  p.p.
$$
2. Domination uniforme,存在一个可积函数，注意一定要是可积的，我们称之为**控制函数**：
$$
\forall n \in \mathbb{N}, |f_{n}(\omega)|\le \phi(\omega) \ p.p.
$$
Alors, on a:
1. 所有$f_{n}$都是可积的
2. $f$是可积的
3. 并且
$$
\int_{\Omega}f_{n}d\mu\underset{n\rightarrow+\infty}\longrightarrow\int_{\Omega}fd\mu
$$
	这里我们已经将积分号和极限号的位置进行了互换。

	单调收敛是可以用控制收敛推出来的。只要我们令控制函数为数列最后趋向的极限值就好了。
	尽管说单调收敛是极限收敛的一种特殊情况，但是单调收敛还可以用于$f$不可积的情况，这是控制收敛做不到的，因为控制收敛一定需要一个可积的控制函数。