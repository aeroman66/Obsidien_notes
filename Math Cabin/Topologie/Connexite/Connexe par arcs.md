在connexe的基础上加了形容词，所以要求比连通性更高。所以通过弧连通是可以推出道路联通的。所以感觉书上的顺序其实不是很好，反过来了。

弧连通，还搜到了道路联通这种叫法
# Connexe par arcs
## Chemin－很重要的前置定义
$(x,y) \in (E,d)^{2}$, toute application $p:[0,1]\longrightarrow E$ ,t.q.:
$$
p(0) = x,p(1) = y
$$
## Connexe par arcs
On dit que A est connexe par arcs, si 
$$
\forall (x,y)\in A^{2},\exists \ \text{un chemin de x a y dans A}
$$
	事实上，在连通性的定义里，没有这种类似的概念，我们只是专注于整个空间会不会被分成几小块，而在弧连通中对每个元素之间的关系做了更加细化。

# Propriete
连通的一部分性质也对道路连通成立，我们发现道路联通蕴含了连通。
- 弧连通部分经过连续的映射映射后还是弧连通的。
- 具有公共点的道路连通集之并也是道路联通的。
	$\{X_{\lambda}|\lambda \in I\}$为X中的一族道路连通集。若$\cap_{\lambda \in I}A_{\lambda} \ne \emptyset$,则$\cup_{\lambda \in I} A_{\lambda}$也是道路联通的
- $\mathbb{R}$ 上所有的开集是所有两两交集为空的，可列的开区间的reunion

# Exemples
1. $\mathbb{R}$:les intervalles
2. $M_{n}(\mathbb{C})$:$GL_{n}(\mathbb{C})$
3. $M_{n}(\mathbb{R})$:$GL_{n}^{+}(\mathbb{R}),GL_{n}^{-}(\mathbb{R})$
4. 欧式空间$\mathbb{R}^{n}$中的子集：非空凸集。

- 连通但不弧连通的例子。

# Composante connexe par arcs
On definit une relation $\mathcal{R}$ :
$$
\forall(x,y)\in A\times A.\left[ x\mathcal{R}y\right]\overset{Def}\Longleftrightarrow\left[x \ est \ relie \ a \ y\right]
$$
$\mathcal{R}$ est une relation equivalence sur A.这些等价的部分就是我们所谓的“弧连通部分”

能利用道路连接的关系为等价关系。用此可以帮助定义道路连通空间
$$
P(x) = \{y \in X|x\~y\Leftrightarrow\text{x,y之间存在一条chemin}\}
$$
## Propriete
- 有且仅有一个弧连通分支，那么是弧连通的。
- 一个点的连通分支大于等于弧连通分支