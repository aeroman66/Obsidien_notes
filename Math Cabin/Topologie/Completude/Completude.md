# Suite de Cauchy
Soit $(E,d)$ un espace metrique,:
$$
\forall \epsilon \in \mathbb{R}_{+}^{*},\exists N \in \mathbb{N},\forall p \ge N,\forall q \ge N,d(u_{p},u_{q})\le \epsilon
$$
	这样一个数列，最后越缩越紧，你不论圈多大一个圈，都可以把一定下标后的无数个元素给圈出来。
	他叫一个集的基本点列。
	柯西数列的定义是依靠distance的定义的，而很多的distance的定义都是跟norme有关的（具体见Topologie）

## Propriete
1. 所有柯西数列都是有界的
2. 所有收敛数列都是柯西数列
3. 对于一个柯西数列来说，收敛的充要条件是，$Adh(u) \ne \emptyset$
	bornee,applique le theoreme de Bolzano-Weierstrab
4. 所有元素是实数的柯西数列都是收敛的（必须得是全体实数）

## Exemples（不是柯西数列）
	通常来说，一个柯西数列应该是收敛的，但是它的极限会在我们所研究的空间之外，他就变得不收敛了。
1. 在有理数集中（前面说过了得是全体实数集）
$$
u_{n} = \frac{\lfloor10^{n}\sqrt{2}\rfloor}{10^{n}}
$$
	最后的极限是$\sqrt{2}$,不在有理数 范围内
2. Dans $Vect(\{x\longrightarrow x^{k}\},k\in\mathbb{K})$,muni de la norme $\|P\|_{\infty} = max(|a_{k}|,k\in\mathbb{N})$
$$
P_{n} = \sum_{k=0}^{n}\frac{1}{k!}(x\longrightarrow x^{k})
$$
	无论多小我们都能构造出来，但是x取值不定，最后这个多项式是不收敛的。

事实上，一个柯西数列通常是收敛的，但是它的极限会不在我们研究的空间内。同理，如果我们想要构造一个不收敛的柯西数列，我们可以选取空间外的一个值作为极限值，然后构造数列去趋近他。
# Espace Complet
Un espace est dit complet, ou toute suite de Cauchy converge.
	所有柯西数列的极限都在这个空间内，以一种抽象的方法说明，这个空间上不存在洞。
	一个完备的赋范向量空间，称作巴拿赫空间。

## Pour montrer qu'un espace est complet
我们首先取一个柯西数列
1. 在一个更大的空间中构建一个极限
2. 我们证明这个柯西数列趋向这个极限
3. 我们证明这个极限在我们所在的空间中

## Propriete
1. 一个完备空间的闭子集是一个完备空间
2. 两个巴拿赫空间之间的线性映射也是一个巴那赫空间
3. 所有有限维的赋范向量空间是完备的
	在有限维的线性空间中，我们更多的使用紧致性这个性质。完备性更多的是让我们像处理有限维线性空间一样去处理无限维线性空间。
