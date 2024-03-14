# 前置定义
Soit $(\Omega,\mathcal{T},\mu)$ un espace mesure et$f:\Omega \longrightarrow [-\infty,+\infty]$,
## Fonction mesurable
$$
\forall A \in \mathcal{BO}(\mathbb{R}),f^{-1}(A)\in \mathcal{T}
$$
	A是属于博雷尔集的
	拿博雷尔集来做定义是不是因为，我们在拿值域进行划分的时候，所有的intervalle都是开集，而我们要确保开集所对应的定义域集合是可测的，所以有了这个定义。
我认为这样定义就保证了每次拿这个函数计算，我们都有一个可测的集合来计算。
## Fonction etagee
Si $f$ est mesurable, a valeurs reelles et:
$$
card(f(\Omega)) \ est \ fini
$$
## Fonction positive
$$
f(\Omega) \subset [0,+\infty]
$$
## Proposition importante
Toute fonction positive et mesurable est limite croissante d'une suite de fonctions etagee positives.
$$
f(positive, \ mesurable) = \lim_{n\rightarrow+\infty}\uparrow f_{n}(positive, \ etagee)
$$
	是不是某种prolongement.


## Image reciproque
	需要理解这个概念，因为这与勒贝格可测这个概念之间有关系。

$$
f^{-1}(B) = \{ x \in X,f(x) \in B \}
$$
还有原像的各种性质，包含、交、并、差、补等。

	黎曼积分是定义域划分的做法，把定义域划分成一样的一个个小截。而勒贝格积分则是一种值域划分方法，通过值域来获取这段定义域区间的长度。

# 勒贝格积分
	我们先定义了一个etagee的fonction的积分，再将其推广到所有可测函数的积分上。
Soit $f$ une fonction etagee, positive sur $\Omega$, on pose alors:
$$
\int_{\Omega}fd\mu \overset{Def} = \sum_{\alpha\in f(\Omega)}\alpha\mu\left(f^{-1}(\{ \alpha \})\right) \in [0,+\infty]
$$
这里就已经提现了拿值域进行划分的思想，与传统的黎曼积分不同。
Soit $f$ une fonction positive, mesurable sur $\Omega$, on pose alors:
$$
\int_{\Omega}fd\mu \overset{Def} =\sup_{g \in \Gamma_{f}}\left(\int_{\Omega}gd\mu\right)\in[0,+\infty]
$$
ou
$$
\Gamma_{f} = \{g:\Omega\rightarrow[0,+\infty],g \ etagee \ et \ g\le f\}
$$
## integrable
	我们将f分为了正函数和不是正函数两种情况
	注意啦，可积性一定要求我们所有的函数值都是正的才可以，这样后面才出现了函数可积与函数积分值存在不能划等号的情况。
Si $f$ est positive et verifie:
$$
\int_{\Omega}f d\mu < +\infty
$$
on dit que $f$ est integrable sur $\Omega$

Si $f$ verifie:
$$
\int_{\Omega}|f| d\mu < +\infty
$$
On dit aussi que $f$ est integrable sur $\Omega$, et on pose
$$
\int_{\Omega}f d\mu \overset{Not}= \\
\int_{\Omega}f^{+} d\mu - \int_{\Omega}f^{-} d\mu
$$

	还没想通为什么可积性要求函数一定要是正的。
## Propriete
前三条Propriete与黎曼积分的三条一样
1. Linearite
2. Croissance
3. Relation de Chasles
4. 多了一条：Restriction
Soit $f$ est integrable sur $\Omega$, alors $f_{|A}$ est integrable sur A et
$$
\int_{A}f_{|A}d\mu_{|A} = \int_{\Omega}\mathbb{1}_{A}fd\mu
$$