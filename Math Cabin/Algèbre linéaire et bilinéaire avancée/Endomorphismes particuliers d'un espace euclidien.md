# Adjoint d'un endomorphisme
	Utilisation
	- Physique:mécannique quantique
	- Analyse des données
	- Tous les outiles actuels
## Théorème de représentation des formes linéaires
Soit $E$ un espace euclidien(donc de dimension finie):
$$
\forall \phi \in E^{*},\exists!a \in E, \forall x \in E,\phi(x) = <a,x>
$$
	On dit que a représente $\phi$
*Démonstration*
## L'adjoint de u
### Définition 
Soit E euclidien, soit $u \in L(E)$,il existe un unique $u^{*} \in L(E)$,
$$
\forall (x,y) \in E^{2},<u(x),y> = <x,u^{*}(y)>
$$
### propriétés
#### linéaire 
#### unique

	Remarque: Dans un espace euclidien, si on prend une base, elle DOIT être orthonormé.
	BON!!!
	
$$
	\text{soit}   x \in E, X = Mat(x,\epsilon) \in M_{n,1}(\mathbb{R}),A = Mat(u,\epsilon) \in M_{n}(\mathbb{R})
$$
$$
\forall x \in E, x = \sum_{k = 1}^{n}<e_{k},x>\cdot e_{k}
$$
$$
X = [<e_{k},x>]_{1\leq k\leq n}
$$
$$
A = [<e_{i},u(e_{j})>]_{1\leq i,j\leq n}
$$
#### Matriciel
$$
Mat(u^{*},\epsilon) = ^{t}A
$$
	Remarque:On utilise souvent si M $\in M_{n}(\mathbb{R})$ vérifie $\forall (x,y) \in M_{n,1}(\mathbb{R})^{2},^{t}X \cdot M \cdot Y = 0$
	alors $M = 0_{M_{n}(\mathbb{R})}$
- $(f+g)^{*} = f^{*}+g^{*}$
- $(\lambda \cdot f)^{*} = \lambda \cdot f^{*}$
- $(f^{*})^{*} = f$
- $(0_{L(E)})* = 0_{L(E)}$ et $(id_{E})* = Id(E)$
- $(fog)* = g*of*$
- $f* \in GL(E),f^{-1}* = (f*)^{-1}$
- $Ker(f*) = (Im(f))^{\perp} , Im(f*) = (Ker(f))^{\perp}$

# Endomorphismes auto-adjoint(symétrique)
## Définition 
Soit E euclidien, $u \in L(E)$, on dit que u est auto-adjoint si $u^{*} = u$
- on note $S(E)$
- $\forall (x,y) \in E^{2},<u(x),y> = <x,u(y)>$
## Proposition technique
Soit E euclidien, $u \in L(E),E_{1}$ sous-espace de E, alors:
$$
[u(E_{1})\subset E_{1}] \iff [u^{*}(E_{1}^{\perp}) \subset E_{1}^{\perp}]
$$
stable par $\dots$

## Théorème Spectral
u auto-adjoint $\longleftrightarrow$ $\exists(e_{1}\dots e_{n}) \in E^{n}$ base orthonormé, $\exists(\lambda_{1}\dots \lambda_{n}),\forall k \in [1,n],u(e_{k}) = \lambda_{k}e_{k}$
	Mat($u,(e_{1},\dots e_{n}) = Diag(\lambda_{1},\dots \lambda_{n})$
	si $u \in S(E)$

### Remarque
Les $\lambda_{k}$ ne sont pas nécessairement distincts.

## Dédoublement 
Je ne comprend pas.

## Propriété 
- $n = dim(E), \frac{n(n+1)}{2} = dim(\text{auto-adjoint de u})$
- endomorphisme auto-adjoint positif
- endomorphisme auto-adjoint défini positif
- Ces espaces sont des cônes positif

### Les remarques
- u $\in \mathcal{S}(E)$,$<u(x),x> = \sum_{k=1}^{n}\lambda_{k}<e_{k},x>^{2}$ 
	- consequences:
		- $\mathcal{S}^{+}$
		- $\mathcal{S}^{++}$
- $u \in \mathcal{L}(E)$, alors $u^{*} o u \in \mathcal{S}^{+}(E)$ ,si $u \in \mathcal{GL}(E)$,$u^{*} o u \in \mathcal{S}^{++}(E)$
	- $\forall f \in \mathcal{L}(E),Ker(f^{*}of) = Ker(f),Im(f^{*}of) = Im(f^{*})=(Ker(f))^{\perp}$
- les propriétés sur $A \in M_{n}(\mathbb{R})$ 
	- lien entre $A$ et $u$
	- $A \in M_{n}(\mathbb{R}),^{t}A A \in \mathcal{S}_{n}(\mathbb{R}).\exists P \in \mathcal{GL}_{n}(\mathbb{R}) ,P^{-1t} A A P \text{diagonal}$ 
	- $A \in M_{n,p}(\mathbb{R}),^{t}A A \in \mathcal{S}_{p}(\mathbb{R})$,et$A ^{t}A \in \mathcal{S}_{n}(\mathbb{R})$

## Racine Carrée
Soit $f \in \mathcal{S}^{+}(E),\exists !g \in \mathcal{S}^{+}(E)$,tel que:
$$
f = gog
$$
### Remarque
Si on n'impose pas v positif, alors tous les v qui ont une matrice de la forme
$$
to be conti\nu ed
$$
vérifient $vov = u$
	v déterminé de manière unique.

Quel est l'intérêt de trouver ça?
$<u(x),y> = <vov(x),y> = <v(x),v(y)>$
这应该是只对正交矩阵有用的

# Automorphisme Orthogonal
$$u \in \mathcal{GL}(E),u^{-1} = u^{*}$$
On note:
$$
\mathcal{O}(E) = \{u \in \mathcal{L}(E),u^{*} = u^{-1}\}
 = \{u \in \mathcal{L}(E),u^{*} o u = Id_{E}\}
$$
	$uou^{*} = Id_{E}$
$\mathcal{O}$ s'appelle le groupe orthogonal de E.
- $\forall (u,v)\in \mathcal{O}(E)^{2},uov \in \mathcal{O}(E)$
- $\forall u \in \mathcal{O}(E),u^{-1} \in \mathcal{O}(E)$

### Remarque
	这里的orthogonal跟上面的定义理解不太一样，注意区分。
- projecteur orthogonal
	- $p^{*} = p$, pas dans $\mathcal{O}$
- symétrie orthogonal 
	- $s^{*} = s$, dans $\mathcal{O}$
	- $s = 2p-id_{E}$, symétrie orthogonal associé.

## Caractérisations de lui
les propriétés suivantes sont équivalentes.
- $f \in \mathcal{O}(E)$
- $\forall x \in E, |f(x)| = |x|$ (conservation de la norme)
- $\forall (x,y) \in E,<f(x),f(y)> = <x,y>$ (conservation de produit scalaire)
- base orthonormée $E(e_{1},\dots e_{n})$, $(f(e_{1}),\dots ,f(e_{n}))$ est encore une base orthonormée
- Il exisite une base orthonormée de $E(e_{1},\dots e_{n})$, telle que $(f(e_{1}),\dots ,f(e_{n}))$soit encore une base orthonormée.

## Qu'est-ce qu'un automorphisme orthogonal
- $dimE = 1$
$$u = \pm id_{E}$$
- $dim E = 2$
$$
Mat(u,(e_{1},e_{2})) =
\begin{bmatrix}
\cos \theta & (-1)^{k}\sin \theta \\
\sin \theta & (-1)^{k+1}\cos \theta
\end{bmatrix}
$$

## Réflexion 
- une symétrie orthogonale
$$
E_{1} = \{x|u(x)=x\} \perp E_{2} = \{x|u(x) = -x\}
$$
- $dim E_{1} = dim E -1$,$E_{1}$ un hyperplan
- Si $(e_{1},e_{2},\dots,e_{n-1})$  base orthonormée de $E_{1}$,$(e_{n})$ base ... de $E_{2}$,
$$
Mat(u,(e_{1},\dots,e_{n})) = diag(1,\dots,1,-1)
$$
### Rappel 
	Toute rotation du plan peut être décomposé en un produit de réflexion (symétrie orthogonales par rapport à une droite)

## Proposition
Soit $u \in \mathcal{O}$, alors il existe $p \in \mathbb{N}$, des réflexions $s_{1},\dots,s_{p}$,
$$
u = s_{1} o \dots o s_{p}
$$
$p_{min} = codim(\{x \in E,u(x) = x\})$

## Rappel : Projecteur Orthogonal
$$
[Ker(p) \perp Im(p)] \iff [p^{*} = p] \iff [\forall x \in E, |p(x)|\leq |x|]
$$
$p_{1},p_{2}$ sont orthogonaux, donc:
- $(p_{1}+p_{2})^{*} = p_{1}^{*} + p_{2}^{*} = p_{1}+p_{2}$, donc $p_{1}+p_{2}\in\mathcal{S}(E)$
- $[p_{1} o p_{2} \in \mathcal{S}(E)] \leftrightarrow [p_{1} o p_{2} = p_{2} o p_{1}]$
- $E_{1}$ 没搞懂这个是什么东西
- 。。。

## Quotient de Rayleigh

## Mise sous forme canonique d'un automorphisme       orthogonal
	用到了上面将线性空间分解成很多个子线性空间的直和的性质。
### Un example

## Quelques notations 
- $\mathcal{O}_{n}(\mathbb{R}) = \{M \in \mathcal{GL}(\mathbb{R}),^{t}MM = (MM^{t}) = In\}$
- groupe speciel orthogonal
$$
\mathcal{SO}(E) = \{u \in \mathcal{O}(E),\det(u) = 1\}
$$
## Orientation d'un espace vectoriel
	1. une base de référence $B_{0}$
	2. B une autre base de E
	3. P^{B}_{B0}
- si $\det_{B_{0}}(B)>0$, B a la même orientation que $B_{0}$
- le contre

### Un Example
- base direct
- base indirect

## Usage de déterminant 
- Savoir si un matrice est inversible
- Si une base est direct ou indirect
- Calculer des volumes

# Endomorphismes antisymétrique
## Définition 
$$
f^{*} = -f
$$
On le note $\mathcal{A}(E)$

## Propriété 
$$
\mathcal{L}(E) = \mathcal{S}(E) \oplus\mathcal{A}(E)
$$
$$
dim (\mathcal{A}(E)) = \frac{n(n-1)}{2}
$$
$$
[f \in \mathcal{A}(E)] \iff [\forall x \in E,<x,f(x)> = 0]
$$
## Forme Canonique d'un endomorphisme anti-symétrique
