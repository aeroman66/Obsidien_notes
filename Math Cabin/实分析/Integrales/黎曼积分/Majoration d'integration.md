	这部分讲到的各种性质都更侧重于各部分的大小关系。
# Majoration
1. Si $f:[a,b] \rightarrow \mathbb{R}(a<b)$ et si $f$ et $|f|$ sont integrables sur $[a,b]$ ,alors:
$$
\left|\int_{a}^{b}f(x)dx\right| \le \int_{a}^{b}|f(x)|dx
$$

2. $f$ est integrable sur $[a,b]$ et bornee, alors:
$$
\left|\int_{a}^{b}f(x)dx\right| \le \
(b-a)\underset{x\in[a,b]}{sup}|f(x)|
$$
3. Soit $f$ continue, positive,alors:
$$
\left[ \int_{a}^{b}f(x)dx = 0 \right] \leftrightarrow [f = 0]
$$
4. Inegalite de Cauchy-Schwarz:
$$
\left|\int_{a}^{b}f(x)g(x)dx\right| \le \
\sqrt{\int_{a}^{b}f(x)^{2}dx} \
\sqrt{\int_{a}^{b}g(x)^{2}dx}
$$

	在积分之前一定要说明这个东西是不是integrable的，就像大部分enonce里面那样。

