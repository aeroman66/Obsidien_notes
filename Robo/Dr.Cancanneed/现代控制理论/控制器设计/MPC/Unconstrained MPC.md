# 描述与定义
- LTI system
一个线性时不变可控的离散系统：
	这里的限定条件很多
$$
x[k + 1] = Ax[k] + Bu[k], x \in \mathbb{R}^{n}, u \in \mathbb{R}^{p}
$$
- Notation define
在 k 时刻往后预测的 i 步。也就是说当 i=0 时，就是 k 时刻的系统状态量：
$$
x[i|k], u[i|k]
$$
# 计算有限时域 MPC
## 序列预测
我们利用上面定义好的 notation，来预测 k 时刻以后的系统状态：
$$
\begin{align}
x[1|k] &= Ax[0|k] + Bu[0|k] \\
x[2|k] &= Ax[1|k] + Bu[1|k] \\
&= A^{2}x[0|k] + ABu[0|k] + Bu[1|k] \\
&\vdots \\
x[i|k] &= A^{i}x[0|k] + A^{i-2}Bu[0|k] + A^{i-3}B^{2}u[1|k] + \cdots + Bu[i-1|k]
\end{align}
$$
将以上的式子写成更加紧凑的矩阵的形式：
	N: predictive horizon
$$
X(k) \overset{\text{def}}=
\begin{bmatrix}
x[1|k] \\
x[2|k] \\
\vdots \\
x[N|k]
\end{bmatrix}
,
U(k) \overset{\text{def}}=
\begin{bmatrix}
u[0|k] \\
u[1|k] \\
\vdots \\
u[N-1|k]
\end{bmatrix}
$$
因为我们需要确定当前的最佳的控制量，所以 $u[0|k]$ 也在我们的预测序列当中，和 X 的不同之处。
将原式写作矩阵形式：
$$
X(k) = Fx[0|k] + \Phi U(k)
$$
其中：
$$
F = 
\begin{bmatrix}
A \\
A^{2} \\
\vdots \\
A^{N}
\end{bmatrix}
,
\Phi =
\begin{bmatrix}
B & \\
AB & B & \\
\vdots \\
A^{N-1}B & A^{N-2}B & \cdots & AB & B
\end{bmatrix}
$$
## 代价函数
	最优化，这种算法叫：predictive cost function
代价函数需要根据自己的需求定义，这里如此定义代价函数我暂时无法解释其中的意义：
$$
J(k) = \sum_{i=1}^{N}\| x[i|k] \|_{Q}^{2} + \| u[i-1|k] \|_{R}^{2} = X(k)^{T}\mathcal{Q}X(k) + U(k)^{T}\mathcal{R}U(k)
$$
U, R 都是权值矩阵，建议看《Optimisation》
通过上面的矩阵表达式对 X 进行代换：
	二次型
$$
\begin{align}
J(k) &= (Fx[k] + \Phi U(k))^{T}\mathcal{Q}(Fx[k] + \Phi U(k)) + U(k)^{T}\mathcal{R}U(k) \\
&= x^{T}[k]F^{T}\mathcal{Q}Fx[k] + 2x^{T}[k]F^{T}\mathcal{Q}\Phi U(k) + U^{T}(k)(\Phi^{T}\mathcal{Q}\Phi + \mathcal{R})U(k)
\end{align}
$$
我们需要对控制序列来最小化这个代价函数，因为我们要预测的是控制序列：
	$*$ 上标代表最优
$$
\frac{\partial J}{\partial U}\Big|_{U=U^{*}} = 0
$$
$$
2x^{T}[k]F^{T}\mathcal{Q}\Phi + 2U^{T}(k)(\Phi^{T}\mathcal{Q}\Phi + \mathcal{R})\Big|_{U=U^{*}} = 0
$$
在矩阵满足一些情况下的时候，我们可以直接解出 U：
$$
U^{*}(k) = -(\Phi^{T}\mathcal{Q}\Phi + \mathcal{R})^{-1}\Phi^{T}\mathcal{Q}Fx[k]
$$
只取序列第一个
$$
u^{*}[k] = -
\begin{bmatrix}
I_{p} & 0 & \cdots & 0
\end{bmatrix}
(\Phi^{T}\mathcal{Q}\Phi + \mathcal{R})^{-1}\Phi^{T}\mathcal{Q}Fx[k] = -K_{mpc}x[k]
$$
前面那个矩阵是对角线部分元素为 0 的对角矩阵
我们发现 unconstrained MPC 得到的就是一个状态线性反馈。

## 验证系统稳定性
根据：
$$
u^{*}[k] = -K_{mpc}x[k]
$$
我们有系统状态空间方程：
$$
x[k+1] = (A - BK_{mpc})x[k]
$$
用李雅普诺夫稳定性判据。
### 验证的必要性
代价函数最优性并不保证系统是稳定的。
直观来理解，因为我们上面优化的是有限时间内的代价函数，所以有可能在过了这段最优化的区间后，x 又开始发散了。（其实不是很懂，他解释的原因）
若 predictive horizon 太短，预测的区间并不能真正反映系统变化的趋势，所以也不能保证系统的稳定性。

### 保证稳定性机制
避免每次计算都要验证系统稳定性。
预测未来无限长的时间，这样预测一定是反映系统行为的：
$$
N = \infty
$$
- 证明
 当预测时域为无穷长时，我们会至少得到一组可行解 $U^{*}(k)$，若系统采用这组解运行下去：
 $$
u[i|k+1] = u^{*}[i+1|k], t.q. x[i|k+1] = x^{*}[i+1|k] 
$$
也就是说我们至少都会有一组可行解。如果后面时刻的最优解跟当前时刻的最优解不一样，那么，我们用代价函数来看：
$$
J^{*}(k+1) - J^{*}(k) \le J(k+1) - J^{*}(k) = -\| x[1|k] \|_{Q}^{2}- \| u[0|k] \|_{R}^{2} < 0
$$
$J(k+1)$ 是采用上一时刻最优解的代价函数，这样我们就证明了只要当前有可行解，未来的所有时刻都是可控的。

# 计算无限时域 MPC
还不懂原理，可能需要精进李雅普诺夫
$$
J(k) = \sum_{i=1}^{\infty}\| x[i|k] \|_{Q}^{2} + \| u[i-1|k] \|_{R}^{2} = \| x[0|k] \|_{P}^{2} - \| x[0|k] \|_{Q}^{2}
$$