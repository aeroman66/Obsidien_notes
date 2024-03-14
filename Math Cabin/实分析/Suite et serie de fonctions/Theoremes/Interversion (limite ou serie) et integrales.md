前面研究了极限函数数列和级数中的各种表现，包括取极限后可以保留函数或者级数的连续性，保持积分结果相等，以及保留可微性。
在这一部分，我们再着重研究极限与积分之间的互动。
	第三章这部分的架构好乱，我实在不知道整个顺序是什么。
# Suite de fonctions
在最一般的情况下，我们需要 CVU 来推出极限和积分号之间的互换关系。
***Interversion limite et integrales***
- **H1** $\forall n \in \mathbb{N},f_{n} \in \mathcal{C}^{0}([a,b],\mathbb{R})$
- **H2** $(f_{n})$ CVU ver $f$ sur $[a,b]$
- **C1** $f \in \mathcal{C}^{0}([a,b],\mathbb{R})$
- **C2** $\lim_{n \rightarrow +\infty} \int_{a}^{b}f_{n}(t)dt = \int_{a}^{b} \lim_{n\rightarrow +\infty} f_{n} = \int_{a}^{b}f(t)dt$
	用 CVU 推出极限和积分的交换

但是在一些情况下，我们用更弱的条件就可以推出这些等价关系：
***Convergence monotone***
- **H1** $\forall n\in \mathbb{N},f_{n}$ est mesurable et positive
- **H2** $(f_{n}(x))$ est croissante $\mu-p.p.$
- **H3** $(f_{n})$ CVS vers une fonction $f \ \mu-p.p.$ sur $I$
- **C1** $\lim_{n \rightarrow +\infty} \int_{I}f_{n}(t)dt = \int_{I} \lim_{n\rightarrow +\infty} f_{n}$
这里不再要求 CVU ，而是要求递增函数列的 CVS

***Convergence dominee***
- **H1** $\forall n\in \mathbb{N},f_{n}$ est mesurable(不一定得是正函数)
- **H2** $f_{n}$ CVS vers $f$ une fonction mesurable sur $I$
- **H3** $\exists \phi \in \mathcal{L}^{1}(I,\mathbb{K})$ telle que:
$$
\forall n \in \mathbb{N},\mu-p.p. \ sur \ I,|f_{n}(x)|\le \phi(x)
$$
- **C1** $\forall n \in \mathbb{N},f_{n}\in \mathcal{L}^{1}(I,\mathbb{K})$ et $f\in \mathcal{L}^{1}(I,\mathbb{K})$
	表明函数列的每个函数以及极限都是可积的。
- **C2** $\lim_{n \rightarrow +\infty} \int_{I}f_{n}(t)dt = \int_{I} \lim_{n\rightarrow +\infty} f_{n}$
这个定理中我们甚至丢掉了单调的条件，以上的过程是一个慢慢剥离条件的过程。

# Serie de fonction
***Interversion serie integrale sur un compact***
Soit $(f_{n})$ une suite de fonctions telles que $f_{n}:[a,b] \longrightarrow \mathbb{K}$.
- **H1** $\forall n \in \mathbb{N},f_{n} \in \mathcal{C}^{0}([a,b],\mathbb{R})$
- **H2** $\sum f_{n}$ CVU ver $S$ sur $[a,b]$
- **C1** $S \in \mathcal{C}^{0}([a,b],\mathbb{R})$
- **C2** $\sum \int_{a}^{b}f_{n}(t)dt$ est convergente
- **C3** $\sum_{n=0}^{+\infty}\int_{a}^{b}f_{n}(t)dt = \int_{a}^{b}\sum_{n=0}^{+\infty}f_{n}$
级数和积分号的顺序调换之间与Fubini定理之间是有关系的，连接他们之间的桥梁是我们接下来要讲到的 ***Mesure Comptage***
## Mesure Comptage
Soit $\mathcal{M} = (\mathbb{N},\mathcal{P}(\mathbb{N}))$ un ensemble muni de sa tribu. La mesure comptage est definit par:
$$
\forall A \in \mathcal{P}(\mathbb{N}),\mu_{c}(A) = 
\begin{cases}
card(A) &\ \text{A est fini} \\
+\infty &\ \text{sinon}
\end{cases}
$$
我们来证明 mesure comptage 与积分号之间的关系，一个很重要的结论，需要分四步进行
- etape 1:证明在函数值为正，从某一自然数之后函数值恒为正的情况：
Soit $f:\mathbb{N}\longrightarrow \mathbb{R}^{+}$ (a support compact),c-a-d:
$$
\exists N\in \mathbb{N},\forall n > N,f(n) = 0
$$
donc, on note:
$$
\Omega = [| 1,N |],f(\Omega) = \{ y_{1},\cdots,y_{k} \}
(y_{i}\ne y_{j} \ si \ i \ne j)
$$
$$
E_{k} = \{ x \in \Omega,f(x) = y_{k} \}(\text{某一函数值对应的定义域})
$$
根据函数定义的特性，我们有：
$$
\forall i,j \in [| 1,k |],E_{i}\cap E_{j} = \emptyset
$$
$$
\Omega = \cup_{j=1}^{k}E_{j}
$$
	这个式子证明略，可看上课笔记

于是我们有：
$$
f(x) = \sum_{j=1}^{k}y_{j}\mathbb{1}_{E_{j}}(x)
$$
donc:
$$
\begin{align}
\int f d\mu_{c} &= \sum_{j=1}^{k}y_{j}\int\mathbb{1}_{E_{j}}d\mu_{c} \\
&= \sum_{j=1}^{k}y_{j}\mu_{c}(E_{j}) \\
&= \sum_{j=1}^{k}y_{j}card(E_{j}) \\
&= \sum_{j=1}^{k}f(x)card(E_{j}) \ si \ x\in E_{j} \\
&= \sum_{n=1}^{N}f(n)
\end{align}
$$
积分的性质，对每一项分别积分不影响结果
我们如果把后面全为 0 的项加上，那么我们就会得到：
$$
\int f d\mu_{c} = \sum_{n=1}^{+\infty}f(n)
$$

- etape 2:不一定是 a support compact ，我们把后面几项补上。
Soit $f_{n} = f \times \mathbb{1}_{[0,n]}$, alors
1. $f_{n}$ est mesurable positive.
2. $f_{n}\le f_{n+1}$, $(f_{n})$ est croissante.
3. $f_{n}$ CVS vers $f$
根据 theo de ***Convergence monotone***，我们可以交换积分号和极限的位置，有：
$$
\sum_{k=1}^{+\infty}f(k) = 
\lim_{n\rightarrow +\infty} \int f_{n}d\mu_{c} = 
\int \lim_{n\rightarrow +\infty}  f_{n}d\mu_{c} = 
\int f d\mu_{c}
$$
这行不等式是从中间往外发展的，这样这步我们就成功了。
- etape 3：将值域扩展到负数。我们正在越来越接近一般函数了
根据以前学的函数可积性的定义，我们有：
$$
[f \ \text{integrable pour la mesure de comptage}] 
\Leftrightarrow [\int |f|d\mu_{c} < +\infty]
$$
	可积性要求我们对函数取绝对值
Donc $\sum f(n)$ est ACV et sommable.
On pose:
$$
f_{+} = \max(f,0)
$$
$$
f_{-} = -\min(f,0) = \min(-f,0)
$$
	f-这样定义，里面的元素就变成正的了，要注意这点
Alors:
$$
\begin{cases}
f = f_{+} - f_{-} \\
|f| = f_{+} + f_{-}
\end{cases}
$$
comme $|f|$ est integrable et $f_{+},f_{-}\le |f|$,alors:
$$
f_{+},f_{-} \text{sont integrables pour} \ \mu_{c}
$$
于是我们有：
$$
\begin{align}
\int f d\mu_{c} &= \int f_{+} - f_{-} d\mu_{c} \\
&= \int f_{+}d\mu_{c} - \int f_{-}d\mu_{c} \\
&= \sum_{n=1}^{+\infty}f_{+}(n)-\sum_{n=1}^{+\infty}f_{-}(n) \\
&= \sum_{n=1}^{+\infty} f_{+}(n)-f_{-}(n) \\
&= \sum_{n=1}^{+\infty} f(n)
\end{align}
$$
- etape 4：这是一个应用环节，我们用 mesure de comptage 来证明级数中的求和号和积分号可以互换位置。
On considere $E = I \times \mathbb{N}$
on munit $E$ de la mesure produit $d\lambda\otimes d\mu_{c}$
我们将一个函数列转化为双变量函数，这是这一步中最妙的部分,因为一旦这么转化，再结合 mesure comptage，我们就可以应用fubini定理了：
$$
f(t,n) = f_{n}(t)
$$
1. Fubini-Tonelli
$$
\begin{align}
\int |f(t,n)|d\lambda\otimes d\mu_{c} 
&= \int_{I}\left( \int_{\mathbb{N}}|f(t,n)|d\mu_{c} \right)d\lambda \\
&= \int_{\mathbb{N}}\left( \int_{I}|f(t,n)|d\lambda \right)d\mu_{c} \\
\end{align}
$$
于是，很自然的，我们就有：
$$
\int_{I} \sum_{n \in \mathbb{N}}|f(t,n)| d\lambda
= \sum_{n \in \mathbb{N}}\int_{I}|f(t,n)| d\lambda
$$
同理，我们进行替换：
$$
\int_{I} \sum_{n \in \mathbb{N}}|f_{n}(t)| d\lambda
= \sum_{n \in \mathbb{N}}\int_{I}|f_{n}(t)| d\lambda
$$
2. Fubini-Lebesgue:
与上面一样的，带进去，但是少了绝对值符号：
$$
\int_{I} \sum_{n \in \mathbb{N}}f_{n}(t) d\lambda
= \sum_{n \in \mathbb{N}}\int_{I}f_{n}(t) d\lambda
$$

