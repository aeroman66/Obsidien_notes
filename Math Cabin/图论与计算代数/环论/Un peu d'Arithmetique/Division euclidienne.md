# Division euclidienne
	辗转相除法
- Theo de Division euclidienne
Soient $a\in \mathbb{Z}$ et $n \in \mathbb{Z}^{*}$ deux entiers relatifs avec $n \ne 0$
$$
\exists ! (q,r)\in \mathbb{Z} \times [|0,|n|-1|],a = nq+r
$$
On dit que q est le quotient et r le reste de la devision euclidienne de a par n.
- Corollaire:
$$
PGCD(a,b) = PGCD(b,r)
$$
**Convergence de cet algorithme**:既然 $r \in [| 0,|b|-1 |]$，那么如果我们重复执行上面的除法运算，我们能得到一个严格递减的 r 数列，直到最后它会减到 0 。然后我们再用一个定义的关系（注意，这个跟 0 的最大公约数是定义出来的）：
$$
PGCD(b,0) = b
$$
**Correction de l'algorithme**:
$$
r_{N-1} = PGCD(r_{N-1},0) = PGCD(r_{N-2},r_{N-1}) = \cdots = PGCD(r_{0},r_{1}) = PGCD(a,b)
$$
## Algorithme d'Euclide
```
1. On pose r0 = a, r1 = b et n = 0
2. tant que rn+1 != 0:
	3. Effectuer la division euclidienne de rn par rn+1
	rn = qn rn+1 + rn+2
	4. n =n + 1
	5. revenir a 2
6. retourner rn
```
# Division euclidienne des polynomes
Soit $\mathbb{K}$ un corp commutatif, alors:
$$
\forall A \in \mathbb{K}[x], \forall B \in \mathbb{K}[x],\exists! R,Q \in \mathbb{K}[x]^{2},A = BQ + R,\deg(R) < \deg(B)
$$
**demonstration**:
- unicite
- existence:
1 cas: Si $\deg(A) < \deg(B)$, alors on pose:
$$
A = B \times 0 + A
$$
2 cas: Si $\deg(A) \ge \deg(B)$, on pose:
$$
A = \sum_{k=0}^{n}a_{k}x^{k},(a_{0},\cdots, a_{n}) \in \mathbb{K}^{n+1},n = \deg(A),a_{n} \ne 0
$$
$$
B = \sum_{k=0}^{n}b_{k}x^{k},(b_{0},\cdots, b_{n}) \in \mathbb{K}^{n+1},n = \deg(B),b_{n} \ne 0
$$
On remarque que 
$$
A - \frac{a_{n}}{b_{p}}x^{n-p}B
$$
est degre $\le n-1 < \deg(A)$, et si $\deg\left( A - \frac{a_{n}}{b_{p}}x^{n-p}B \right) < \deg(B)$, donc on prend:
$$
A = B \times \frac{a_{n}}{b_{p}}x^{n-p} + \left( A - \frac{a_{n}}{b_{p}}x^{n-p}B \right)
$$
Sinon on ietre l'algorithme, 不断去消除新获得的 $A_{i}$ 的最高项：
$$
\begin{align}
A_{0} &= A \\
A_{1} &= A - \frac{a_{n}}{b_{n}}x^{n-p}B \\
A_{i + 1} &= A_{i} - \alpha_{i}x^{\deg(A_{i}) - p}B
\end{align}
$$
Par construction, on obtient une suite $(\deg(A_{i}))_{i \ge 0}$ strictement decroissante. donc:
$$
\exists j \ge 0, \deg(A_{j})< \deg(B)
$$
De plus:
$$
A_{j} = A_{0} - \left(\sum_{i = 0}^{j - 1}\alpha_{i}x^{\deg(A_{i}) - p}\right)B
$$
Donc:
$$
A = B \times Q + R, \deg(R) < \deg(B)
$$
## Theo
- Si $\mathbb{K}$ est un corp commutatif, alors $\mathbb{K}[x]$ est principal (参考 ideal 的 principal 的定义)
**demonstration**:
Soit $I$ un ideal de $\mathbb{K}[x]$,
1 cas: Si $I = \{ 0 \}$, alors $I = 0\mathbb{K}[x]$
2 cas: Si $I \ne \{ 0 \}$ alors $I$ contient des polynomes non null.
On pose:
$$
d = \min\{ \deg(p) | p \in I\backslash \{ 0 \} \}
$$
On choisit $P \in I, \deg(P) = d$. Comme $I$ est un ideal, on a:
$$
P \mathbb{K}[x] \subset I
$$
On fixe $A \in I$, par division euclidienne de $A$ par $P$, on a:
$$
\exists ! (Q,R) \in \mathbb{K}[x]^{2},A = PQ + R, \deg(R) < \deg(P)
$$
donc:
$$
R = A  - PQ \in I, \deg(R) < \min \{ \deg(P) | P \in I\backslash \{ 0 \} \}
$$
On en deduit que:
$$
R = 0
$$
donc:
$$
A = PQ \in P\mathbb{K}[x], I \subset P\mathbb{K}[x]
$$

**Remarque**:?
Il suffit qu'un anneau commutatif admettre une division euclidienne pour etre principal.
	只要交换环中的元素可以做 division euclidienne ,那么他就是 principal 的。

**Exemple**:
Pour l'anneau des entiers de Gauss
$$
\mathbb{Z}[i] = \{ a + ib | (a, b) \in \mathbb{Z}^{2} \}
$$
我们要证明这些复数每一个都可以被欧氏除法分解：
$$
\forall z = a + ib \in \mathbb{Z}[i], \forall w = c + id\in \mathbb{Z}[i]\backslash \{ 0 \}, \exists!(q, r) \in \mathbb{Z}[i]^{2},z = qw + r
$$
$$
N(r) < N(w)
$$
On peut alors montrer que $\mathbb{Z}[i]$ est principal.