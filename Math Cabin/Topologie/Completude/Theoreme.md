以下这些定理都是建立在完备空间上的。
# Trois remarques importantes
1. La caracterisation sequentielle des applications continues.
	感觉是后面两条的基础
2. Soit $f:(E,d)\longrightarrow (E^{'},d^{'})$,si $f$ est uniformement continue,alors si $(x_{n})_{n \in \mathbb{N}} \in E^{\mathbb{N}}$ est une suite de Cauchy,alors:
$$
(f(x_{n}))_{n\in\mathbb{N}} \ est \ une \ suite \ de \ Cauchy \ de \ E^{'}
$$
3. 如果$f$仅仅是continue的，那么第二条就不一定成立了
e.g.:
$$
x_{n} = \frac{1}{n+1}
$$
$$
f:x\longmapsto \frac{1}{x}
$$

# Point fixe
Soit $(E,d)$ un espace complet et $f$ une application de E dans E contractante
$$
\exists k \in]0,1[,\forall(x,y) \in E^{2},d(f(x),f(y)) \le kd(x,y)
$$
	一个较直观的例子，导函数永远小于某个值。
alors:
$$
\exists! a\in E,f(a) = a
$$
	这个东西很有趣，他证明了很多数学上的结论
要是注意的是，这个是不动点存在的一个定理，而不是不动点的定义。我们可以拿函数contractante来判断一个函数的存不存在不动点。

# Fermes emboites, version complete
Soit $(E,d)$ un espace complet, $(F_{n})_{n \in \mathbb{N}}$ des fermes non vide de E,t.q.
$$
diam(F_{n})\underset{n\rightarrow +\infty}\longrightarrow 0 \ et \ \forall n \in \mathbb{N},F_{n+1}\subset F_{n}
$$
alors:
$$
\exists! \alpha\in E,\underset{n\in\mathbb{N}}\cap F_{n} = {\alpha}
$$
1. $F_{n}$ 的diam一定得趋向于0，不然就不成立了
$$
F_{n} = [n,+\infty[
$$
2. 即使满足了diam的条件，我们也能举出范例
$$
x = (x_{n})_{n\in\mathbb{N}} \ n'a \ pas \ de \ valeur \ d'adherence
$$
$$
F_{n} = \{x_{n},n\ge p\}
$$
因为x没有adh，所以我们知道$F_{n}$是ferme的，因为其中所有收敛的数列都是常数列。并且F很明显是emboite的。
$$
\underset{p\in\mathbb{N}}\cap F_{p} = Adh(x) = \emptyset
$$
我们发现他满足diam的定义，但是却不满足定理，因为这里espace不是complet的，而是离散的。

# Prolongement des applications uniformement continues
Soit $(E,d)$ et $(E',d')$ deux espaces metriques, tels que $E'$ est complet, soit $A\subset E$
$$
f:A\longrightarrow E' \text{uniformement continue sur A}
$$
Alors, il existe une unique fonction $\tilde{f}$ definie et continue sur $\bar{A}$ telle que:
$$
\forall a \in A,\tilde{f}(a) = f(a)
$$
On l'appelle prolongement de $f$ a $\bar{A}$.De plus, $\tilde{f}$ est uniformement continue sur $\bar{A}$.

	事实上，黎曼积分中用cpm的函数去逼近一个函数也是这种做法。