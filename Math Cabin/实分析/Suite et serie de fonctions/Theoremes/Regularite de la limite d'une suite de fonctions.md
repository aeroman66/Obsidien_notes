主要讲函数列与极限有关的部分性质。
在前面一斤介绍了三种 convergence 的基础上，我们在这里做出总结，看在满足哪些 hypothese 的情况下可以得出什么相似的结论。
# Continuite et limite
极限与连续性相关的theo
## Limite uniformes
Soit $(f_{n})$ une suite de fonctions telles que $f_{n}:I \longrightarrow \mathbb{K}$
- **H1** $\forall n \in \mathbb{N}$, la fonction $f_{n}$ est continue sur $I$
- **H2** $(f_{n})$ converge uniformement vers $f$ sur $I$ ou sur tout segment de $I$
- **C1** $f$ est continue sur $I$
	说白了就是简单地得到了一条 CVU

## La double limites ou intervertion des limites
Soit $(f_{n})$ une suite de fonctions telles que $f_{n}:I \longrightarrow \mathbb{K}$ et $f:I \longrightarrow \mathbb{K}$. Soit $(b_{n}) \in \mathbb{K}^{\mathbb{N}}$ et $a \in \bar{I}$
- **H1** $(f_{n})$ CVU ver $f$ au voisinage de a
- **H2** $\forall n \in \mathbb{N},\lim_{x\rightarrow a}f_{n}(x) = b_{n}$
- **C1** $\lim_{n\rightarrow +\infty}b_{n} = b$（说明bn这个数列是收敛的）
- **C2** $\lim_{x\rightarrow a}f(x) = b$
	用 CVU 推极限的极限,两个极限可以交换位置。
	$$
	\lim_{x\rightarrow a}\left( \lim_{n\rightarrow +\infty} f_{n}(x)\right) = \lim_{n\rightarrow +\infty}\left( \lim_{x\rightarrow a} f_{n}(x)\right)
	$$

	当 a 是区间的一个端点时，事情就不好说了
	这条定理可以用来证明没有CVU
# Integration sur un segment
## Interversion limite et integrales
- **H1** $\forall n \in \mathbb{N},f_{n} \in \mathcal{C}^{0}([a,b],\mathbb{R})$
- **H2** $(f_{n})$ CVU ver $f$ sur $[a,b]$
- **C1** $f \in \mathcal{C}^{0}([a,b],\mathbb{R})$
- **C2** $\lim_{n\rightarrow +\infty}\int_{a}^{b}f_{n}(t)dt = \int_{a}^{b}\lim_{n\rightarrow +\infty}f_{n} = \int_{a}^{b}f(t)dt$
	用 CVU 推出极限和积分的交换
## Convergence monotone

## Convergence dominee

# Derivabilite
## Interversion limite et derivee
Soit $(f_{n})$ une suite de fonctions telles que $f_{n}:I \longrightarrow \mathbb{K}$ et $f:I \longrightarrow \mathbb{K}$.
- **H1** $\forall n \in \mathbb{N},f_{n} \in \mathcal{C}^{1}(I,\mathbb{K})$
- **H2** $f_{n} \ CVS \ vers \ f$
- **H3** $(f_{n}^{'}) \ CVU \ vers \ h$
- **C1** $f \in \mathcal{C}^{1}(I,\mathbb{K})$
- **C2** $f^{'} = h$ et $\left( \lim_{n\rightarrow +\infty}f_{n} \right)^{'} = \lim_{n\rightarrow +\infty}f^{'}_{n}$
- **C3** $(f_{n})$ CVU vers $f$
## derivee k-iemes
Soit $(f_{n})$ une suite de fonctions telles que $f_{n}:I \longrightarrow \mathbb{K}$ et $f:I \longrightarrow \mathbb{K}$.
- **H1** $\forall n \in \mathbb{N},f_{n} \in \mathcal{C}^{k}(I,\mathbb{K})$
- **H2** $\forall i \in [0,k-1]\cap \mathbb{Z}, f_{n}^{(i)} \ CVS \ vers \ h_{i}$
- **H3** $(f_{n}^{(k)}) \ CVU \ vers \ h_{k}$
- **C1** $f \in \mathcal{C}^{k}(I,\mathbb{K})$
- **C2** $\forall i \in [0,k-1]\cap \mathbb{Z},f^{(i)} = h_{i}$ et $\left( \lim_{n\rightarrow +\infty}f_{n} \right)^{'} = \lim_{n\rightarrow +\infty}f^{'}_{n}$
- **C3** $\forall i \in [0,k-1]\cap \mathbb{Z},(f_{n}^{(i)})$ CVU vers $h_{i}$
	比前一个关系多推出好多层