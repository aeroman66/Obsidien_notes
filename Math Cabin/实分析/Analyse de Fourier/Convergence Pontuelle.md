	逐点收敛，是最严格的收敛
# Deux proprietes
这两个 proprietes 从傅里叶级数系数出发，来判断一个傅立叶级数是否收敛。
- $f \in E$
$$
\sum |a_{n}(f)|,\sum |b_{n}(f)| \ convergent \Rightarrow S(f) \ CVU \ f
$$
- $f \in E$
$$
(c_{n}(f))_{n \in \mathbb{Z}} \ sommable \Rightarrow (c_{n}(f)\cdot e_{n})_{n \in \mathbb{Z}} \ sommable \ et \ S(f) \ CVU \ f
$$
事实上:
$$
(c_{n}(f))_{n \in \mathbb{Z}} \ sommable \Rightarrow \sum |a_{n}(f)|,\sum |b_{n}(f)| \ convergent
$$
# Theos de Convergence
这些定理从函数本身的性质出发，来判断这个函数的傅立叶级数的收敛情况。
## CVN des $\mathcal{C}^{1}_{p.m.}$
Si $f \in E$ est continue, de classe $\mathcal{C}^{1}_{p.m.}$, alors(CVU):
$$
S_{n}(f) \underset{n \rightarrow +\infty}\longrightarrow f \ sur \ \mathbb{R}
$$
## Dirichlet
Si $f \in E$ est de classe $\mathcal{C}^{1}_{p.m.}$, alors $S_{n}(f)$ converge simplement（CVS） vers la fonction:
$$
S(f):x \longmapsto \frac{f(x^{+}) + f(x^{-})}{2}
$$
这里的函数不一定要是连续的，并且 convergence 是 simple 而非 uniforme，这造成了一种吉布斯现象。
**Phenomene de Gibbs**
假设
$$
S_{N} = \sum_{-N}^{+N}
$$
那么 N 就决定了逼近程度，N 越大，越近似。傅里叶级数的最大值会逐渐去向不连续点，但是峰值不会下降，大约有 9% 的跳变值。
## Fejer
Si $f \in E$ est continue, alors(CVU):
$$
\sigma_{n}(f) = \frac{S_{0}(f) + \cdots + S_{n}(f)}{n + 1} \underset{n \rightarrow +\infty}\longrightarrow f \ sur \ \mathbb{R}
$$
$S_{n}(f)$ designe la somme partielle de la serie de Fourier de $f$
### Theoreme d'approximation de Weierstrab trigonometrique
- Origine
Soit $f \in \mathcal{C}^{0}([a,b], \mathbb{K})$, alors il existe une suite de fonctions polynomiales $(P_{n})_{n \in \mathbb{N}} \in \mathbb{K}[X]^{\mathbb{N}}$ t.q.
$$
\| P_{n} - f \|_{\infty,[a,b]}\underset{n \rightarrow +\infty}\longrightarrow 0 
$$
- Approcimation
所有 $2\pi$ 连续周期函数都是一个三角多项式的 limite uniforme.
$$
\sigma_{n}(f) = \sum_{(k,p)\in \bigtriangleup}\alpha_{k,p,n}\sin^{k}\cos^{p}
$$