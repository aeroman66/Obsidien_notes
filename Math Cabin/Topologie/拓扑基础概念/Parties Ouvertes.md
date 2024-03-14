# Partie Ouverte
 一个集合在一个空间里可以既不是闭集也不是开集
	]0,1]在R上既不是闭集又不是开集
1. 定义
2. 对于开集的三个operations
	1. 空集和E永远是E中的开集（同时他们两个也是闭集）
	2. 开集的任意并集是开集
	3. 开集的有限交集是开集（如果是无限交集的话可能会交出E？）
3. 开集的特征
	这是开集最重要的一个性质，不仅好画，还允许我们直接利用这条性质而不用做其他的补充。
$$
[O ouvert dans E] \leftrightarrow [\forall x \in O,\exists \epsilon > 0,BO(x,\epsilon) \subset O]
$$
4. 如何证明一个集合是开集
	1. 利用开集的特征
	2. 注意每个x对应的$\epsilon$取值一定要跟x本身有关。

# 由开集衍生出的概念
## Interieur
1. 定义
2. notations
	1. $\overset{o}A$
	2. Int(A)
3. 特征
跟开集的特征几乎一模一样
4. Interieur d'une boule ferme
5. 三个基本性质
	1. $\overset{o}A \subset A$
	2. $[A = \overset{o}A] \leftrightarrow [A ouvert de E]$
	3. $\overset{\overset{o}o}A = \overset{o}A$
6. 四个propositions