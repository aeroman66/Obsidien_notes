# Continuite
## Continuite sous le signe somme
Soit $(f_{n})$ une suite de fonctions telles que $f_{n}:I \longrightarrow \mathbb{K}$.
- **H1** $\forall n \in \mathbb{N},f_{n}$ est continue sur $I$
- **H2** $\sum f_{n}$ CVU vers $S$
- **C1** $S$ est continue en $x_{0}$

## Interversion limite et somme infinie
- **H1** $\sum f_{n}$ CVU vers S au voisinage de a
- **H2** $\forall n \in \mathbb{N},\lim_{x\rightarrow a}f_{n}(x) = b_{n}$
- **C1** $\sum b_{n}$ converge
- **C2** $\lim_{x\rightarrow a}S(x) = \sum_{k=0}^{+\infty}b_{n}$
以上 C2 可以翻译成：
$$
\lim_{x\rightarrow a}\sum_{k=0}^{+\infty}f_{k}(x) = \sum_{k=0}^{+\infty}\lim_{x\rightarrow a}f_{k}(x)
$$
	极限和求和可以交换位置。

# Integrale
## Interversion serie integrale sur un compact
Soit $(f_{n})$ une suite de fonctions telles que $f_{n}:[a,b] \longrightarrow \mathbb{K}$.
- **H1** $\forall n \in \mathbb{N},f_{n} \in \mathcal{C}^{0}([a,b],\mathbb{R})$
- **H2** $\sum f_{n}$ CVU ver $S$ sur $[a,b]$
- **C1** $S \in \mathcal{C}^{0}([a,b],\mathbb{R})$
- **C2** $\sum \int_{a}^{b}f_{n}(t)dt$ est convergente
- **C3** $\sum_{n=0}^{+\infty}\int_{a}^{b}f_{n}(t)dt = \int_{a}^{b}\sum_{n=0}^{+\infty}f_{n}$

## Theoreme de Fubini

# Derivabilite
## Permutation derivation et serie
Soit $\sum f_{n}$ une serie de fonctions.
- **H1** $\forall n \in \mathbb{N},f_{n} \in \mathcal{C}^{1}(I,\mathbb{K})$
- **H2** $\forall x \in I, \sum f_{n}(x) \ CVS \ vers \ S(x)$
- **H3** $\sum f_{n}^{'} \ CVU \ vers \ h$
- **C1** $S \in \mathcal{C}^{1}(I,\mathbb{K})$
- **C2** $S^{'} = h$ et $\left( \sum_{n=0}^{+\infty} f_{n} \right)^{'} = \sum_{n=0}^{+\infty} f^{'}_{n}$
- **C3** $\sum f_{n}$ CVU vers $S$

## K-ieme 参考前面的关系