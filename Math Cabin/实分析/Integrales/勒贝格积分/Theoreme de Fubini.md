	前面讲的收敛允许我们在极限运算符和积分运算符之间做顺序调换。而Theoreme de Fubini则允许我们将不同积分运算符之间做顺序调换。
# 前置定义
## 有限测度
On dit que $\mu$ est une mesure $\sigma$-finie sur $\Omega$, s'il existe une famille denombrable $(A_{n})_{n\in \mathbb{N}}\in T^{\mathbb{N}}$:
$$
\forall n \in \mathbb{N},\mu(A_{n})\in \mathbb{R_{+}},et \ \Omega=\underset{n\in\mathbb{N}}\cup A_{n}
$$
	概率空间里的$\mathbb{P}$是一个很好的例子，概率空间$\Omega$是有限的，为1，每个测度必然都对应$[0,1]$之中的实数。


## Tribu Produit
$(\Omega_{1},\mathcal{T}_{1},\mu_{1}),(\Omega_{2},\mathcal{T}_{2},\mu_{2})$,
$$
\Omega = \Omega_{1} \times \Omega_{2}
$$
## Mesure Produit
	有限测度保证了这个测度存在的唯一性。

$(\Omega_{1},\mathcal{T}_{1},\mu_{1}),(\Omega_{2},\mathcal{T}_{2},\mu_{2})$ deux espaces mesures, ou $\mu_{1},\mu_{2}$ sont $\sigma$-finies,存在定义在$\mathcal{T}_{1}\otimes\mathcal{T}_{2}$上的测度:
$$
\forall (A_{1},A_{2})\in\mathcal{T}_{1} \times\mathcal{T}_{2},\mu(A_{1}\times\mu_{2}) = \mu_{1}(A_{1}) \times \mu_{2}(A_{2})
$$
on note:
$$
\mu = \mu_{1}\otimes\mu_{2}
$$
	1. $\mu$ est une mesure $\sigma$-finie
	2. 其中一项为零时，该测度为0.

# 两个定理
## Fubini-Tonelli
Soit $f:\Omega_{1}\times \Omega_{2} \longrightarrow [0,+\infty]$,une application mesurable:
$F_{1}$ est mesurable:
$$
F_{1}:
\begin{cases}
\Omega_{1} \longrightarrow [0,+\infty] \\
x \longrightarrow \int_{\Omega_{2}}f(x,\cdot)d\mu_{2}
\end{cases}
$$
$F_{2}$ est mesurable:
$$
F_{2}:
\begin{cases}
\Omega_{2} \longrightarrow [0,+\infty] \\
y \longrightarrow \int_{\Omega_{1}}f(\cdot,y)d\mu_{1}
\end{cases}
$$
并且:
$$
\int_{\Omega_{1}\times\Omega_{2}}fd(\mu_{2}\otimes\mu_{2}) = \int_{\Omega_{1}}F_{1}d\mu_{1} = \int_{\Omega_{2}}F_{2}d\mu_{2}
$$
	这个定理是针对正可测函数来说的。
	有些情况下，我们知道函数对于$\Omega_{1} \times \Omega_{2}$ 可测，我们并不能确定对于$\Omega_{1}$或者$\Omega_{2}$同样可测。
	在计算双重函数积分时，我们先给函数套上绝对值，然后用Tonelli定理判断函数的可积性。

    被点代替的变量说明我们需要取遍每个他可以取的值。
## Fubini-Lebesgue
Soit $f:\Omega_{1}\times \Omega_{2} \longrightarrow [-\infty,+\infty]$,une application mesurable:
$F_{1}$ est definie $\mu_{1}$-p.p. et integrable
$$
F_{1}:
\begin{cases}
\Omega_{1} \longrightarrow [-\infty,+\infty] \\
x \longrightarrow \int_{\Omega_{2}}f(x,\cdot)d\mu_{2}
\end{cases}
$$

$F_{2}$ est definie $\mu_{1}$-p.p. et integrable
$$
F_{2}:
\begin{cases}
\Omega_{2} \longrightarrow [-\infty,+\infty] \\
y \longrightarrow \int_{\Omega_{1}}f(\cdot,y)d\mu_{1}
\end{cases}
$$

并且:
$$
\int_{\Omega_{1}\times\Omega_{2}}fd(\mu_{2}\otimes\mu_{2}) = \int_{\Omega_{1}}F_{1}d\mu_{1} = \int_{\Omega_{2}}F_{2}d\mu_{2}
$$
	Fubini定理告诉了我们双重积分的计算方式。

### R.q.:
通过指定特定的空间和Tribu，我们可以将上面定理的结论推广到数列与级数上：
Soit $u_{n,p}$ une suite double de complexes, telle que:
1. $\forall n \in \mathbb{N},\sum_{p}|u_{n,p}|$ converge
2. $\sum_{n}\sum_{p=0}^{+\infty}|u_{n,p}|$ connverge
那么我们可以得到以下级数都是收敛的：
$$
\forall (n,p) \in \mathbb{N}^{2},\sum_{p}u_{n,p},\sum_{n}u_{n,p},\sum_{n}\sum_{p=0}^{+\infty}u_{n,p},\sum_{p}\sum_{n=0}^{+\infty}u_{n,p}
$$
并且为我们提供一种计算方式：
$$
\sum_{n=0}^{+\infty}\sum_{p=0}^{+\infty}u_{n,p} = \sum_{p=0}^{+\infty}\sum_{n=0}^{+\infty}u_{n,p}
$$

## 总结
我们可以总结双重积分的计算步骤
1. 给函数套上绝对值，套用Tonelli定理
2. 看积分值是不是小于$+\infty$,如果是，我们就可以判断函数可积
3. 然后套用Fubini定理对积分进行计算