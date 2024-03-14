	跟以前讲得换元不同，这里不是把dx,dy什么的换掉，而是一种测度换元
	啥意思啊，完全没听明白啊
# 前置定义
Soit $(\Omega, \mathcal{T},\mu)$ un espace mesure, $\Omega^{'}$ un ensemble et $f:\Omega\rightarrow \Omega'$,on a tribu image de $\Omega'$ par $f$ la tribu definie par:
$$
\mathcal{T}_{f}'\overset{Not}= \left\{A' \subset \Omega', f^{-1}(A') \in \mathcal{T} \right\}
$$
	是依靠$\Omega$ 的tribu定义的
mesure de $\mu$ par $f$:
$$
\forall A' \in \mathcal{T}_{f}', \mu'_{f}(A') \overset{Not}= \mu (f^{-1}(A'))
$$
# Changement de Variable
1. cas positif
Si $f:\Omega'\rightarrow[0,+\infty]$ est une application mesurable, positive,alors:
$$
\int_{\Omega'}fd(\mu'_{\phi}) = \int_{\Omega}f\circ\phi d\mu
$$
2. cas general
Si $f:\Omega'\rightarrow[-\infty,+\infty]$ est une application mesurable alors:
$$
\left[f \ est \ \mu_{\phi}'-integrable \ sur \ \Omega'\right] \Leftrightarrow[f\circ \phi \ est \ \mu -integrable \ sur \ \Omega]
$$
如果函数还是可积的，那么我们还有:
$$
\int_{\Omega'}fd(\mu'_{\phi}) = \int_{\Omega}f\circ\phi d\mu
$$
	这个定理很理论，没有很大的实践操作的意义。但是加入我们取一种更加准确的情况，比如$\Omega = \Omega' = \mathbb{R}^{n}$, munis des trubus borelienne,avec un changement de variable de type particulier$(\mathcal{C}^{1}-diffeomorphisme)$,那么是可以指导我们进行实际计算的。

# Changement de Variable $\mathcal{C}^{1}$
## Diffeomorphisme
Soit $f \in \mathcal{k}(\bigtriangleup,\mathbb{R}^{p})$,ou $\bigtriangleup$ est un ouvert de $\mathbb{R}^{n}$ et $k \in \mathbb{N}^{*}\cup \{\infty\}$, on dit que f est un $\mathcal{C}^{1}-diffeomorphisme$ de $\bigtriangleup$ si on a:
1. $f$ est injective
2. $f(\bigtriangleup)$ est un ouvert de $\mathbb{R}^{p}$
3. $f^{-1}$ de classe $\mathcacl{C}^{k}$

Propriete:
1. n = p
	通俗解释，因为是微分同胚的，所前后两个空间从拓扑学上来讲是一样的。那么他们的纬度理论上也是一样的
2. 我们可以定义$f$在点$\mathop{x}\limits_{-} \in \mathbb{R}^{n}$上的雅可比矩阵：
$$
J_{f}(\mathop{x}\limits_{-}) = [\partial_{j}f_{i}(\mathop{x}\limits_{-})]_{(i,j)\in [1,n]^{2}\cap\mathbb{Z}}
$$

### Caracterisation globale des diffeomorphisme
$$
f \text{est un $\mathcal{C}^{1}-diffeomorphisme$} \Leftrightarrow 
\begin{cases}
\text{f est injective} \\
et \\
\forall \vec{x}\in\bigtriangleup,J_{f}(\mathop{x}\limits_{-})\in GL_{n}(\mathbb{R})
\end{cases}
$$
	用这个特征可以更好地判断f是不是微分同胚的。

## Changement de Variable $\mathcal{C}^{1}$
Soit U un ouvert de $\mathbb{R}^{n}$ et $\phi:U\longrightarrow \mathbb{R}^{n}$ un $\mathcal{C}^{1}$-diffeomorphisme.Soit de plus une fonction $f:\phi(U)\rightarrow [-\infty,+\infty]$ une fonction mesurable(pour les tribus boreliennes) et integrables sur $\phi(U)$ (pour les mesures de Lebesgue),alors $|det(J_{\phi})|\cdot(f\circ \phi)$ est integrable sur U et :
$$
\int_{\phi(U)} f d\lambda = \int_{U}|det(J_{\phi})|\cdot (f\circ g)d\lambda
$$
	将g(x)当做积分变量，所以自然积分范围是g的值域。
	有时候，一些零测集会给我们造成问题，而我们需要把这些零测集给去掉。