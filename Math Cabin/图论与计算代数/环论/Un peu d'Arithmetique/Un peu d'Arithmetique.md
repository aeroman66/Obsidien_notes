# Congrus
	同余
- Congrus
Deux entiers relatifs $(a,b)\in\mathbb{Z}^{2}$ sont dits ***condrus module n***（这个包含n的东西是一个完整的关系，n是不能从中割裂出来的）,lorsqu'ils ont le meme reste par la division euclidienne:
$$
\exists (q,q^{'},r) \in \mathbb{Z}^{2}\times [0,|n|-1]\cap \mathbb{Z},
\begin{cases}
a = qn+r \\
b = q^{'}n+r
\end{cases}
$$
On note:
$$
a \equiv b[n]
$$
	不要先入为主，后面括号内的是除数而不是余数。
**Propriete**：
1. $\forall (a,b) \in \mathbb{Z}^{2},a \equiv b[n] \Leftrightarrow a-b \in n\mathbb{Z}$
2. La relation de congruence module n est une relation d'equivalence.
**demonstration de 2**:
- reflexive
$$
x \equiv x \ [n]
$$
- symetrie
$$
x \equiv y \ [n] \Rightarrow y \equiv x \ [n]
$$
- transtive(要用欧式除法展开证明，这里只是简写)
$$
x \equiv y \ [n], y \equiv z \ [n] \Rightarrow x \equiv z \ [n]
$$
1. La classe d'equivalence de a,notee $\dot{a}$:
$$
\dot{a} = \{ b \in \mathbb{Z}|a \equiv b[n] \} = \{ a +qn |q \in \mathbb{Z} \} = a +n\mathbb{Z}
$$
	在 a 的基础上加上余数的整数倍。
4. $\dot{a} = \dot{r}$, $r$ est le reste de la division euclidienne de a par n.
	on a $a \equiv r [n]$, donc $\dot{a} = \dot{r}$ comme relation de congruence module n est une relation d'equivalence.
5. $\forall (a,b)\in \mathbb{Z}^{2}$, la classe d'equivalence de $a+b,\dot{\widehat{a+b}}$ depend seulement de $\dot{a},\dot{b}$
	Il suffit de montrer que si $(a_{1}, a_{2}) \in \mathbb{Z}^{2}$ et $(b_{1}, b_{2}) \in \mathbb{Z}^{2}$ sont tels que $\dot{a}_{1} = \dot{a}_{2}$ et $\dot{b}_{1} = \dot{b}_{2}$, alors $\dot{\widehat{a_{1}+b_{1}}} = \dot{\widehat{a_{2}+b_{2}}}$
**demonstration de 5**:
On suppose que $\dot{a}_{1} = \dot{a}_{2}$, donc que:
$$
a_{1} \equiv a_{2} \ [n], a_{1} - a_{2} \in n\mathbb{Z}
$$
et que $\dot{b}_{1} = \dot{b}_{2}$:
$$
b_{1} \equiv b_{2} \ [n], b_{1} - b_{2} \in n\mathbb{Z}
$$
Alors:
$$
(a_{1} + b_{1}) - (a_{2} + b_{2}) = (a_{1} - a_{2}) + (b_{1} - b_{2}) \in n\mathbb{Z}
$$
On en deduit que:
$$
a_{1} + b_{1} \equiv a_{2} + b_{2} \ [n], \dot{\widehat{a_{1}+b_{1}}} = \dot{\widehat{a_{2}+b_{2}}}
$$
# 倍数与因数
## Commun diviseur
Soit $(a,b) \in \mathbb{Z}^{2}$,on pose:
$$
a\mathbb{Z} + b\mathbb{Z} = \{ ka+lb|(k,l)\in \mathbb{Z}^{2} \}
$$
on remarque que $a\mathbb{Z} + b\mathbb{Z}$ est un sous-groupe de $\mathbb{Z}$, donc:
$$
\exists ! d \in \mathbb{N},a\mathbb{Z} + b\mathbb{Z} = d\mathbb{N}
$$
on remarque que:
$$
a\mathbb{Z} \subset d\mathbb{Z},b\mathbb{Z} \subset d\mathbb{Z}
$$
donc d est un diviseur commun de a et b.
	***PGCD*** : Plus Grand Commun Diviseur
### Premiers
Un nombre $p \in \mathbb{N}\backslash \{ 0,1 \}$ est premier loraque ses seuls diviseurs positifs sont 1 et p.
On dit que deux entiers relatifs a et b sont premiers entre eux loraque:
$$
PGCD = (a,b) = 1
$$
## Commun multiple
Soit $(a,b) \in \mathbb{Z}^{2}$,on pose:
$$
d\mathbb{Z} \subset a\mathbb{Z},d\mathbb{Z} \subset a\mathbb{Z}
$$
donc d est un multiple commun de a et b.
	***PPCM*** : Plus Petit Commun Multiple
## Propriete
- Soient $(a,b) \in \mathbb{Z}$ non tous nulls, alors :
$$
PGCD(a,b) \times PPCM(a,b) = |ab|
$$
- $\forall (a,b) \in \mathbb{Z}^{2}$
1. $a\mathbb{Z} \cap b\mathbb{Z} = PPCM(a,b)\mathbb{Z}$
2. $a\mathbb{Z} + b\mathbb{Z} = PGCD(a,b)\mathbb{Z}$
# Indicatrice d'Euler
$$
\Phi:
\begin{cases}
\mathbb{N}^{*} \longrightarrow \mathbb{N}^{*} \\
n \longmapsto card\{r \in [|0,n-1|]|n\wedge r = 1 \}
\end{cases}
$$
它的函数值就是 nombre de generateurs de $(\mathbb{Z}/n\mathbb{Z},+)$
我们可以手动计算他值域的前几个值：

|n|1|2|3|4|5|6|7|8|9|10|
|---|---|---|---|---|---|---|---|---|---|---|
|$\Phi(n)$|1|1|2|2|4|2|6|4|6|4|
我们目前还没有算法可以计算出它的所有值。
## Proprietes
- p un nombre premier
$$
\Phi(p) = p-1
$$
- $\forall n \in \mathbb{N}^{*}$, on a:
$$
n = \sum_{d \in [|1,n|],\text{d diviseur de n}}\Phi(d)
$$