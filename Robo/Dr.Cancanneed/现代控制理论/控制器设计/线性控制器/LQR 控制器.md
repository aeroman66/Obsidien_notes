Linear Quadratic Regulator，是一种调节器。
我们在这里暂时只引入代价函数(Cost function)的概念，但是还不对其求最小值，只是大致知道代价函数是个什么存在。
# LQR 与直接线性控制的区别
根据上一讲，我们知道了线性控制的整个过程：
$$
\text{选择} K(k_{1}, k_{2},\cdots)\overset{\text{改变}}\longrightarrow A_{cl}\text{的特征值}\overset{\text{控制}}\longrightarrow\text{系统表现}
$$
但是在这个过程中，我们面临着一个很核心的问题：
- 如何确定特征值 $\lambda$ ？怎么样的特征值才是好的？
# Cost Function
为了解答以上问题，我们引入了代价函数（aka 目标函数，能量函数）
$$
J = \int_{0}^{\infty} (X^{T}QX + U^{T}RU)dt
$$
其中，Q R 都是对角矩阵：
$$
\begin{bmatrix}
a & & & \\
& b & & \\
& & c & \\
& & & \ddots
\end{bmatrix}
$$
# Exemple
![[倒立摆 lqr1.png]]
![[倒立摆 lqr2.png]]
![[倒立摆 lqr3.png]]
![[倒立摆 lqr4.png]]
![[倒立摆 lqr5.png]]
# Remarque Importante
LQR 本质上是一个利用最优化理论选取反馈增益的比例控制器。
所以在 Dr.can 的视频里，因为他默认的目标状态是系统的初始状态，所以说我们在控制量里没有看到做差的痕迹，因为：
$$
u = - k(x - x_{des}) = - k(x - 0) = - kx
$$
而在 b 站倒立摆教程中，只是把这个做差显性的写出来了，尽管目标值也为 0，所以看上去不一样。
![[lqr 比例控制器.png]]