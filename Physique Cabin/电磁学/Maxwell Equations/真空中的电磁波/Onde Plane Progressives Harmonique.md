	不知道为什么我们经常会研究正弦形式的物理量。
所有跟波有关的物理量都可以写成以下形式：
$$
\psi(M,t) = A\cos(\omega t-\vec{k}\vec{OM}+\phi)
$$
On introduit le vecteur unitaire parallele a $\vec{k}$:
$$
\vec{u} = \frac{\vec{k}}{||\vec{k}||}
$$
## Double periodicite
$$
T = \frac{2\pi}{\omega}
$$
$$
\lambda \overset{def}= \frac{2\pi}{k}
$$
## VItesse de phase
尽管叫这个名字，但是它描述的是波的传播速度？
$$
\psi(M,t) = A\cos(\omega t-kz+\phi) = A\cos(\omega\times(t-\frac{z}{\frac{\omega}{k}}))
$$
donc:
$$
\psi(z,t) = \psi(0,t-\frac{z}{\frac{\omega}{k}})
$$
on a:
$$
v_{\phi} = \frac{\omega}{k}
$$
## 复数表达
$$
E_{x} = E_{0x}\cos(\omega t-kz+\phi_{x})
$$
$$
\underline{\vec{E}} = E_{0x}e^{\phi_{x}}\exp[j(\omega t-kz)]
$$
remplace $\vec{\bigtriangledown}$ par $-j\vec{k}$ et $\frac{\partial}{\partial t}$ par $j\omega$
	从物理量的函数表达式中就可以一眼看出。
## Relation de dispersion
$$
(-k^{2} + \frac{\omega^{2}}{c^{2}})\times \underline{\vec{E}} = \vec{0}
$$
为了求的 E 的非零解，我们需要满足：
$$
\omega = ck
$$
在此基础上，我们还可以推出：
$$
\lambda = c\times T,v_{\phi} = \frac{\omega}{k} = c
$$
# Polarisation
电磁波电场的方向决定了polarisation的方向。
	$(\vec{u},\vec{E},\vec{B})$ est une base directe.我们在先前的计算看过了，他们两两之间是由向量积得到的于是互相正交。
## Convention Observateur
放在波传播方向的轴上，看着波向它传播。
- $\phi>0$: Droite
- $\phi<0$: Gauche
	这里的相位定义得跟椭圆中的定义相同。
	结合那两个图像记忆。
## Polarisation elliptique
我们先规定波向量 $\vec{k} = k\vec{e}_{z}$, 我们有：
$$
\vec{E}(M,t) = 
\begin{cases}
E_{0x}\cos(\omega t^{'}-kz+\phi_{x}) \\
E_{0y}\cos(\omega t^{'}-kz+\phi_{y}) \\
0
\end{cases}
$$
在一个 z 固定的截面上， $\vec{E}$ 在平面 $\{ \vec{e}_{x}, \vec{e}_{y} \}$ 上跑一个椭圆，我们称之为椭圆极化。
$$
\phi = \phi_{y}-\phi_{x}
$$
- $\phi>0$: La composante selon y est en avance
- $\phi<0$: La composante selon y est en retard
	要保证状态相同的情况下比较，相位越大，则时间越小，说明出现的越早，故avance。
	这是相对于 y 来说的，如果将相位的定义换了，说法也就不一样了。
## Polarisation Circulaire
$\phi = \frac{\pi}{2}$:Gauche
$\phi = -\frac{\pi}{2}$:Droite
	因为$\phi_{y}$在定义的时候前面是减号。
	事实上convention还是一样的，看谁avance，然后判断。PPT上的很乱，还是现场判断的好。
## Polarisation Rectiligne
- $\phi = 0$：一三象限
- $\phi = \pi$：二四象限

## Decomposition
- 一束电磁波可以拆分成x,y方向上的两个Polarisation rectiligne
$$
\vec{E} == e^{j(\omega t-kz)}
\begin{cases}
E_{0x} \\
E_{0y}e^{j\phi}
\end{cases} = 
e^{j(\omega t-kz)``}
\begin{cases}
E_{0x} \\
0
\end{cases} +
e^{j(\omega t-kz)}
\begin{cases}
0 \\
E_{0y}e^{j\phi}
\end{cases}
$$
这种分解方法在后面的实验分析中非常有用。
- 一束电磁波可以拆分成方向相反的的两个Polarisation circulaire
$$
\vec{E} == e^{j(\omega t-kz)}
\begin{cases}
E_{0x} \\
E_{0y}e^{j\phi}
\end{cases} = 
$$

## Polarisation de la lumiere
我们在这里研究特定电磁波的 polarisation ，那就是光。
	为什么要单单研究光的偏振呢。
### Lumiere naturelle
- non polarisee
- trains d'onde incoherents
### Obtention de lumiere polarisee
任意光通过一个 polariseur 就可以得到偏振光，式子如下：
$$
\vec{E_{0}}\vec{u_{p}} = 
\left(
\begin{matrix}
E_{x} \\
E_{y}
\end{matrix}
\right)
\left(
\begin{matrix}
1 \\
0
\end{matrix}
\right) =
E_{x}
$$
这样就变成了 x 方向上的偏振光。
### Loi de Malus
$$
I_{ap} = I_{0}\cos^{2}\alpha
$$

## Lame a retard
Un cristal birefringent: 可以改变穿过它的光的偏振状态。
	双折射晶体是会产生双折射现象的晶体，作用相当于两个透振方向相互垂直的起偏器。更细节的内容就很高深了。
双折射晶体会有快轴和慢轴，两个轴的方向会有不同大小的折射率，光在其中的传播速度并不一样。因此最后同时从晶体出射的两个光之间的相位差和一开始相比就不一样了：
$$
\bigtriangleup\phi = \frac{2\pi}{\lambda_{0}}(n_{L}-n_{R})e
$$
再详细点说，由于慢轴上的光传播速度更慢，因此在晶体里传播的时间更长，某种意义上，相当于它的相位被快轴赶上了一部分。

### Lame demi-onde $\frac{\lambda}{2}$
$$
\bigtriangleup n \times e = \frac{\lambda}{2}
\Rightarrow \bigtriangleup\phi = \pm\pi
$$


### Lame quart d'onde $\frac{\lambda}{4}$
$$
\bigtriangleup n \times e = \frac{\lambda}{4}
\Rightarrow \bigtriangleup\phi = \pm\frac{\pi}{2}
$$