Definie sur $]0,+\infty[$:
$$
\Gamma(x) = \int_{0}^{+\infty}u^{x-1}e^{-u}du
$$
# 推导
On sait que:
$$
\sum_{n=0}^{+\infty}n^{p}x^{n} \underset{x\rightarrow1^{-}}\sim \frac{p!}{(1-x)^{p+1}}
$$
并且根据 Comparaison de serie-integrale:
(Rappel):
- 单调递增函数，对所有的 $n \ge 1$
$$
\int_{n-1}^{n}f(t)dt \le f(n) \times 1 \le \int_{n}^{n+1}f(t)dt
$$
- 单调递减函数，对所有的 $n \ge 1$
$$
\int_{n}^{n+1}f(t)dt \le f(n) \times 1 \le \int_{n-1}^{n}f(t)dt
$$
	可以从图像面积的角度来理解
我们发现我们要研究的函数是一个单调递增的函数，利用第一个关系，将 n 从 1 到正无穷累加起来，我们就可以得到以下近似：
$$
\sum_{n=0}^{+\infty}n^{p}x^{n} \underset{x\rightarrow1^{-}}\sim \int_{0}^{+\infty}t^{p}x^{t}dt = \int_{0}^{+\infty}t^{p}e^{t\ln x}dt
$$
	之所以趋向于1的左极限是因为右极限往右不收敛，故级数没有定义。
我们再进行一次换元，令：
$$
u = t \ln x
$$
得到：
$$
\int_{0}^{+\infty}t^{p}x^{t}dt = \frac{1}{(\ln x)^{p+1}}\int_{0}^{+\infty}u^{p}e^{-u}du
$$
又因为：
$$
\ln x \underset{x\rightarrow1^{-}}\sim x-1
$$
所以根据待定系数法，我们得到：
$$
p! = \int_{0}^{+\infty}u^{p}e^{-u}du
$$
p 的定义范围是 $]-1,+\infty[$ 的，所以我们如下定义Gamma函数，令它的定义域为 $]0,+\infty[$:
$$
\Gamma(x) = \int_{0}^{+\infty}u^{x-1}e^{-u}du
$$
# Propriete
## 求导
设以下函数，对 Gamma 函数求导就是对它积分内求导：
$$
g(x) = u^{x-1}e^{-u}
$$
alors on a:
$$
g'(x) = \ln u \cdot u^{x-1}e^{-u}
$$
通过recurrance，我们还可以求解它的 j 阶导函数：
$$
g^{(j)}(x) = (\ln u)^{j} \cdot u^{x-1}e^{-u}
$$
也由此，我们证明了：
$$
\Gamma \in \mathcal{C}^{\infty}
$$
### Convexe
$$
g^{(2)}(x) = (\ln u)^{2} \cdot u^{x-1}e^{-u} \ge 0
$$
因为恒大于零，所以 convex

# 复数域

$\Gamma$ definie sur 
$$
]0,+\infty[ + i\cdot \mathbb{R} = \{ a+ib , a>0, b \in \mathbb{R}\} = \wedge
$$
sont de la meme forme:
$$
\Gamma(x) = \int_{0}^{+\infty}u^{x-1}e^{-u}du
$$
# Propriete
## Continue
**H1** Mesurabilite sur $\Omega$
Soit $\alpha \in \wedge,f(\alpha,\cdot)$ est mesurable sur $\Omega$, car elle est continue sur $\Omega$.
	1. 我们固定一个alpha，所以这里我们的变量其实是后面那个点
	2. 因为最后是对 t 积分的，所以这里我们要证明对 t 的可积性。
**H2** Continuite sur $\wedge$
Soit $t \in ]0,+\infty[, f(\cdot,t)$ est continue sur $\wedge$
**H3** Domination uniforme
Soit $t \in ]0,+\infty[, \alpha = a + ib$,我们有：
$$
|t^{\alpha-1}e^{-t}| = t^{a-1}e^{-t}
$$
如果$a\rightarrow 0^{+},t\rightarrow 0^{+}$,那我们发现这个东西趋向于正无穷，这样我们就找不到一个有效的domination了。
所以我们令：
$$
\alpha = a + ib \in [\gamma,\delta] + i\mathbb{R}, (\gamma,\delta)\subset ]0,+\infty[
$$
$$
|t^{\alpha-1}e^{-t}| = t^{a-1}e^{-t} \le \phi:
\begin{cases}
t^{\gamma-1}e^{-t} &\ t \in ]0,1]\\
t^{\delta-1}e^{-t} &\ t \in ]1,+\infty]
\end{cases}
$$
On a:
- $\phi$ mesurable sur $]0,+\infty[$,comme $\mathcal{C}^{0}_{p.m}$
- $\phi(t)\underset{0^{+}}\sim t^{\gamma -1}$ integrable comme $\gamma-1>-1$
- $\phi(t) = o_{+\infty}(\frac{1}{t^{2}})$ integrable

所以gamma函数在复数域上是连续的。

# Des formules
1. En posant $\wedge = ]0, +\infty[ + i\mathbb{R}$
$$
\forall z \in \wedge , \Gamma(z + 1) = z\Gamma(z)
$$
2. $\forall n \in \mathbb{N}$
$$
\Gamma(n + 1) = n!
$$
3. Formule de Stirling(阶乘近似)
$$
\Gamma( x + 1 )\underset{+\infty}\sim \left( \frac{x}{e} \right)^{x}\sqrt{2 \pi x}
$$
4. On a:
$$
\Gamma(\frac{1}{2}) = \sqrt{\pi}
$$
$\forall n \in \mathbb{N}$
$$
\Gamma(n + \frac{1}{2}) = \frac{(2n)!}{2^{2n}n!}\sqrt{\pi}
$$