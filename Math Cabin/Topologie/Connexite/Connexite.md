有两个重要定义。
# Connexite
On a trois assertions equivalentes pour dire que un espace topologie A est connexe:
1. Si $B\subset A$ est un ouvert et ferme de A, alors $B = \emptyset$ ou $B = A$
2. $\forall (O_{1},O_{2})$ ouverts de A, $A = O_{1} \cup O_{2}$ et $O_{1} \cap O_{2} = \emptyset \Rightarrow O_{1} = \emptyset \ ou \ O_{2} = \emptyset$
	这条好像是更通用的定义
3. Toute fonction continue $f:A \longrightarrow \{0,1\}$ est constante.
	其中{0,1}是一个离散集合
事实上，我们发现每条断言都是在表述一个事实，那就是我们不能把拓扑空间A切分成两个相离部分。

我们还要注意其中开闭集这个概念。
	根据定义，我们很容易发现$\emptyset$和$A$本身是$A$空间中的开闭集。

### E.g.
Soit $A\subset \mathbb{R}$,如果$A$是连通集，那么一定满足以下四种形式之一：
1. $[a,b]$
2. $[a,b)$
3. $(a,b]$
4. $(a,b)$

# Propriete 
- 强弱关系
$$
[Connexe \ par \ arcs]\Rightarrow[Connexe]
$$
1. pas reciproque.
	看上去弧连通要更强一点
2. 但是在赋范线性空间中，这两个是等价的。

- 连通空间的连续像是连通的。
- 联通空间和闭包的关系
A est connexe,$\overset{-}A$ l'est aussi, ainsi pour tout ensemble B t.q.$A\subset B \subset \overset{-}A$

- 交集不为空的Connexes的并集是Connexe
	比较好证，我们用第三种断言，对每个连通集构造常值函数就可以证明
两两交集不为空也有这个性质。

- 对第三个assertion有一段小拓展，将值域变成一个离散的空间，函数依旧是constante的。

- 连通空间的有限个直积和直积
Soit $X_{1},\cdots,X_{n}$ connexes:
$$
X_{1}\times X_{2}\times \cdots \times X_{n}
$$
也是连通的
Soit $\{X_{\lambda}|\lambda \in I\}$是一族连通空间，则:
$$
\Pi_{\lambda \in I}X_{\lambda}
$$
也连通。

# Composante connexe
Composante connexe de a, le plus grand connexe de A contenant a.
$$
C_{A}(a)
$$
我们也可以将其定义为，含有x的所有连通集的并集。
### Remarque
$C_{A}(a)$ est toujours ferme dans A.

$$
[x\mathcal{R}y]\Longleftrightarrow[x\in C_{A}(y)]
$$
这也向我们说明了所有E的子空间A是reunion disjointe de ses composantes connexes

# Propriete
- 连通分支的基本性质：
1. 包含x的连通分支是包含x的连通集中最大的一个
2. 对于任意$x,y\in X$,如果他俩的连通分支交集不为空，那么他俩的连通分支相同。
3. 对于任意$x\in X,C_{A}(x)$都是闭集

- 连通分支有且仅有一个
$$
[\text{连通分支有且仅有一个}]\Leftrightarrow [Connexe]
$$
- Soit $\{X_{\lambda}|\lambda \in I\}$是X中的一族连通空间，满足$X = \cup_{\lambda \in I}A_{\lambda}$并且disjointes 2 a 2,那么我们可以知道这个partition里的每个元素就是X的各个连通分支。