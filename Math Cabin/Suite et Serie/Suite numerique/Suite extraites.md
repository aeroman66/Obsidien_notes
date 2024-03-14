	这部分主要的定义就是提取数列，还有个valeur d'adherence,其他都是杂乱的性质。
Soit $u = (u_{n})_{n\in \mathbb{N}}\in\mathbb{R}^{\mathbb{N}}$ une suite, 我们把所有以下形式的数列都叫做suite extraite de u:
$$
(U_{\phi(n)})_{n\in \mathbb{N}}, \ ou \ \phi:\mathbb{N}\rightarrow\mathbb{N} \ est \ strictement \ croissante
$$
	意思是只能按顺序抽取，不能来回反复横跳。

# Valeur d'adherence
Soit $u = (u_{n})_{n\in \mathbb{N}}\in\mathbb{R}^{\mathbb{N}}$ une suite, on dit que $\lambda$ est une valeur d'adherence de u, s'il existe une sous-suite de u quiconverge vers $\lambda$:
$$
x_{\phi(n)}\underset{n\rightarrow+\infty}\longrightarrow \lambda
$$
note:
$$
Adh(u)
$$
	如果一个数列收敛，那么它的valeur d'adherence只有一个值。
	但是这个命题的逆命题是错误的
# Proposition
- 在所有数列中，我们都可以提取出一个单调数列。
- 如果一个数列是收敛的，那么他所有的子数列都是收敛的，并且都趋向这个值
- 这条是关于提取数列的一些规则的。
	我们先取一个子数列$(u_{\phi(n)})_{n\in \mathbb{N}}\in\mathbb{R}^{\mathbb{N}}$,再取这个子数列的子数列$(u_{\theta(n)})_{n\in \mathbb{N}}\in\mathbb{R}^{\mathbb{N}}$,我们有以下两点
	$$
	\theta(\mathbb{N})\subset\phi(\mathbb{N})
	$$
	$$
	\theta = \phi \circ \psi
	$$
	我们要保证之前那个值域嵌套的关系，所以会有这个函数嵌套的关系。
- 我认为这一条可以归纳为，如果一个数列的所有子数列都趋向于一个值，那么这个数列就趋向于这个值。
- 用子数列来说明一个数列并不收敛。
$$
(u_{n})_{n\in \mathbb{N}} \ ne \ converge \ pas \ vers \ \lambda\Rightarrow\left[\exists\epsilon>0,\exists(u_{\phi(n)})_{n\in \mathbb{N}} \ extraite \ de \ u,\forall n\in\mathbb{N},|u_{\phi(n)}-\lambda|>\epsilon\right]
$$

# Theoreme（IMPORTANTE）
bolzano-weierstraß：
对于所有的有界数列，我们可以从中抽取一个收敛的子数列。
	很好证，结合前面的所有数列我们可以抽取一个单调子数列，有界的单调数列必收敛，所以我们就可以得到这个定理了。