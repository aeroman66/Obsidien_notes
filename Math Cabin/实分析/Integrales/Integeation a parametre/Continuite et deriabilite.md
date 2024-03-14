# Continuite
	Continuite sous le signe \int
Soit $(\Omega, \mathcal{T}, \mu)$ un espace mesure, $(\wedge, d)$ un espace metrique (espace de parametre) et $\lambda_{0} \in \wedge$.soit $f : \Omega \times \wedge \rightarrow \mathbb{K}$, 满足以下三个 hypotheses:
**H1**：Mesurabilite
$$
\forall \lambda \in \wedge,f(\cdot, \lambda) \ \text{est mesurable sur} \ \Omega
$$
	这里变化的是 x ,固定的是 $\lambda$，函数是对 x 的积分，所以要求对于 x 来说是 mesurable 的。
**H2**：Continuite
$$
f(x, \cdot) \text{ est comtinue en } \lambda_{0},\mu-p.p.
$$
	函数的自变量 (parametr) 是 $\lambda$，所以要对于 $\lambda$ 来说函数是连续的
**H3**：Domination uniforme
Il existe une fonction $\phi \in \mathcal{L}^{1}(\Omega, \mathcal{T},\mu;\mathbb{R}_{+})$,t.q.
$$
\forall \lambda \in \wedge, |f(x, \lambda)| \le \phi(x),\mu-p.p.
$$
**C1**：Alors，la fonction suivante est definie sur $\wedge$ et est continue en $\lambda_{0}$ 
$$
F:
\begin{cases}
\wedge \rightarrow \mathbb{K} \\
\lambda \mapsto \int_{\Omega}f(\cdot, \lambda)d\mu
\end{cases}
$$
	注意我们在函数的定义中加了积分这一因素，这跟我们三个假设里的 f 是有很大不同的。

## Remarque importante
以上定理有一个更加常用的版本。
Soit $I,J$ deux intervalles de $\mathbb{R}$ et $f:J \times I \rightarrow \mathbb{R}$ verifiant:
**H1**:$\forall t \in I,f(\cdot, t)$ est cpm sur $J$
	是不是在实数域上，cpm 就意味着黎曼可积
**H2**:$\forall x \in J,f(x, \cdot)$ est continue sur $I$
**H3**:il existe une fonction $\phi$ positive et integrable sur $J$ t.q.（T.C.D）
$$
\forall (x, t) \in J \times I, |f(x, t)| \le \phi(x)
$$
**C1**:我们依旧可以得到目标的积分函数连续

# Derivabilite
	Derivation sous le signe \int
 Soit $\wedge = I$ un intervalle de $\mathbb{R}$, muni de sa tribu borelienne et de la mesure Lebesgue, soit $(\Omega, \mathcal{T}, \mu)$ un espace mesure et $f:\Omega \times I\rightarrow \mathbb{K}$ une fonction mesurable. Soit, de plus, $\lambda_{0} \in I$.
**H1**:Integrabilite
$$
\forall \lambda \in I, f(\cdot, \lambda) \ \text{est integrable sur} \ \Omega
$$
**H2**:Derive partielle
L'application $f(x, \cdot)$ est $\mu-p.p.$ derivable en $\lambda_{0}$, nous notons:
$$
\frac{\partial f}{\partial \lambda}(x,\lambda_{0})
$$
	这单单指这一点上的变化率
**H3**：Domination
Il existe une fonction $\phi \in \mathcal{L}^{1}(\Omega, \mathcal{T},\mu;\mathbb{R}_{+})$,t.q.
$$
|f(x, \lambda) - f(x, \lambda_{0})| \le \phi(x)|\lambda - \lambda_{0}| \ \mu-p.p.
$$
**C1**:La fonction suivante est definie sur I et derivable en $\lambda_{0}$:
$$
F:
\begin{cases}
I \rightarrow \mathbb{K} \\
\lambda \mapsto \int_{\Omega}f(\cdot, \lambda)d\mu
\end{cases}
$$
**C2**:sa derivee
$$
F'(\lambda_{0}) = \int_{\Omega} \frac{\partial f}{\partial \lambda}(x,\lambda_{0}) d\mu
$$
## Dans la pratique
在我们平时使用的过程中，定理的条件通常会更简单一点，会比较符合我们的直觉，如下：
**H1**:$\forall \lambda \in I, f(\cdot, \lambda) \ \text{est integrable sur} \ \Omega$
**H2**:L'application $f(x, \cdot)$ est $\mu-p.p.$ derivable sur $I$, nous notons:
$$
\frac{\partial f}{\partial \lambda}(x,\lambda)
$$
	与上面只代表一个点处的变化率不同，这个类似于导函数，对于这段区域上的 $\lambda$ 都成立
**H3**:Il existe une fonction $\phi \in \mathcal{L}^{1}(\Omega, \mathcal{T},\mu;\mathbb{R}_{+})$,t.q.
$$
|\frac{\partial f}{\partial \lambda}(x,\lambda)| \le \phi(x) \ \mu-p.p.
$$
**C1**:同理，我们得到函数是连续的
**C2**：导函数表达式为：
$$
F'(\lambda_{0}) = \int_{\Omega} \frac{\partial f}{\partial \lambda}(x,\lambda) d\mu
$$
## Remarque importante
以上仅仅是 derivabilite，我们也可以用类似的定理来证明 $\mathcal{C}^{1}$,是在实数域上的，平时我们用的大多数都是实数域。
Soit $I,J$ deux intervalles de $\mathbb{R}$ et $f:J \times I \rightarrow \mathbb{R}$ verifiant:
**H1**:$\forall t \in I,f(\cdot, t)$ est integrable sur $J$
	积分变量
**H2**:$\forall x \in J,f(x, \cdot)$ est de classe $\mathcal{C}^{1}$ sur $I$
	参数
**H3**:il existe une fonction $\phi$ positive et integrable sur $J$ t.q.
$$
\forall (x, t) \in J \times I, |\partial_{2} f(x, t)| \le \phi(x)
$$
**C1**:$F:t \mapsto \int_{J}f(x, t)dx$ est de classe $\mathcal{C}^{1}$ sur $I$ et $F':t \mapsto \int_{J}\partial_{2}f(x, t)dx$
- Pour montrer la regularite $\mathcal{C}^{k}$ ou $\mathcal{C}^{\infty}$ , on utilise une recurrence(见上课笔记有，但是过程十分的混乱)