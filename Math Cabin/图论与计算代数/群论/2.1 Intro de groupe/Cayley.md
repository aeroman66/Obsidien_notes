	听说有个叫Cayley定理的东西，尽请期待
# Tableau de Cayley
为了清晰地展示loi de composition interne,我们引入了Cayley表，他是专门用来描述有限群的结构的。
以下以$(\mathbb{U}_{4},\times)$为例

| |1|i|-1|-i|
|-----|-----|-----|-----|-----|
|1|1|i|-1|-i|
|i|i|-1|-i|1|
|-1|-1|-i|1|i|
|-i|-i|1|i|-1|

- 我们发现如果一张表是对称的话，那么说明这个 composition 是 commutatif 的。
- 根据 TP ，一张表要确实反应一个 groupe fini ，那么这张表就必须 满足 associative（要求见 TP）
$$
m_{m_{i,j},k} = m_{i,m_{j,k}}
$$
## Remarque
根据两个化简法则：
$$
a * b = c * b \Leftrightarrow a = c
$$
$$
a * b = a * c \Leftrightarrow b = c
$$
我们可以得知，在一个 tableau de Cayley 中，G 中的元素在每行或者每列中只会出现一次。因为如果你出现了两次，即我们可以假设 $a * b = a * c$ , 那么我们可以推断 $b = c$, 但是b, c分属于表中的不同两列，所以他们应该是不一样的。这样就矛盾了。所以各个元素在每行每列中都只能出现一次。
### Exemples
Soit $(G, *)$ un groupe:
1. D'ordre 1, $G = \{e\}$

| |e|
|---|---|
|e|e|
2. D'ordre 2, $G = \{e, a\}$

| |e|a|
|--------|-------|-------|
|e|e|a|
|a|a|e|
3. D'ordre 3, $G = \{e, a, b\}$
	这种情况照样只存在一种情况。

| |e|a|b|
|---|---|---|---|
|e|e|a|b|
|a|a|b|e|
|b|b|e|a|

4. D'ordre 4, $G = \{e, a, b, c\}$

| |e|a|b|c|
|---|---|---|---|---|
|e|e|a|b|c|
|a|a|c|e|b|
|b|b|e|c|a|
|c|c|b|a|e|

| |e|a|b|c|
|---|---|---|---|---|
|e|e|a|b|c|
|a|a|b|c|e|
|b|b|c|e|a|
|c|c|e|a|b|

| |e|a|b|c|
|---|---|---|---|---|
|e|e|a|b|c|
|a|a|e|c|b|
|b|b|c|a|e|
|c|c|b|e|a|

| |e|a|b|c|
|---|---|---|---|---|
|e|e|a|b|c|
|a|a|e|c|b|
|b|b|c|e|a|
|c|c|b|a|e|
当 G 的 ordre 是 4 的时候，我们可以写出上面四张 tableau de Cayley. 但是事实上，前三张在我们的眼里是等价的， 而第四张才是与前三张有所不同的，因为第四张的对角线上全是 element neutre.

而我们以前两张为例，展示如何在等价的 tableau de Cayley 之间进行转化。
我们可以通过一个 permutation 将表一变成表二：
$$
\phi:
\begin{cases}
G\longrightarrow G \\
x \longmapsto 
\begin{cases}
\phi(a) = c \\
\phi(b) = a \\
\phi(c) = b \\
\end{cases}
\end{cases}
$$
我们取一中的某一项进行示例变换：
$$
a * c = b
$$
通过映射 $\phi$ 我们可以得到：
$$
\phi(a) * \phi(c) = \phi(b) = \phi(a * c)
$$
$$
c * b = a
$$
所以这种情况下我们只有两种 tableau de Cayley.
On remarque qu'un isomorphisme entre deux groupes finis d'ordre $n$ représentées par des sudokus associatifs $M=(m_{i,j})_{0\leqslant i,j\leqslant n-1}$ et $M'=(m'_{i,j})_{0\leqslant i,j\leqslant n-1}$ correspond à une permutation $\sigma$ de $\{0,1,\dots,n-1\}$ telle que :
$$
\sigma(0)=0\quad\text{et}\quad\forall(i,j)\in\{0,1,\dots,n-1\}^2,\ \sigma(m_{i,j})=m'_{\sigma(i),\sigma(j)}
$$
	先运算再映射和先映射再运算的结果是一样的
如果两个 tableau de Cayley 间存在这样一个 permutation， 那么我们叫这两个 groupes finis à isomorphisme près，换言之，他们其实是等价的。

	以上情况我们发现 tableau 都是对称的。所以这些 groupe 都是 commutatifs 的。
	那我们是不是可以发现有限群都是交换群啊。