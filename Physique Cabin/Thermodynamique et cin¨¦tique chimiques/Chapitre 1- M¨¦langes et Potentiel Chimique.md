# Enthalpie Libre
## Description d'un système physico-chimique
- formule chimique : Les proportions des éléments 
- une phase bien définie : ça nous donne une espace physico-chimique
### Compositions d'un mélange 
intensives
- fraction molaire
- fraction massique
- concentration
## Évolution Monotherme Monobare
### Définition
- La pression extérieure est maintenue constante égale à $P_{0}$
- La température extérieure est maintenue constante égale à $T_{0}$
	MTMB
### Entropie créée : Principe d'évolution 
$$
S_{cr} = \frac{-[G]^{final}_{initial}}{T_{0}}
$$
L'enthalpie libre(énergie de Gibbs)
$$
G \overset{\text{def}} = U+PV-TS = H-TS
$$
$$
[G]^{final}_{initial}\leq 0
$$
Un état d'équilibre thermodynamique minimise la fonction enthalpie libre G d'un système en évolution MTMB.
## Enthalpie libre d'un mélange monophasé 
### Relations différentielles fondamentales et potentiel chimique 
- des paramètres physiques : T, P
- des paramètres de compositions : $n_{1},n_{2},n_{3}\dots n_{N}$
$$
(\frac{\partial G}{\partial T})_{P,n_{j}} = -S ; (\frac{\partial G}{\partial P})_{T,n_{j}} = V
$$
$$
(\frac{\partial G}{\partial n_{i}})_{T,P,n(j\neq i)} \overset{\text{def}} = \mu_{i}
$$
$$
dG = VdP-SdT+\sum_{i = 1\dots N}\mu_{i}dn_{i}
$$
### Relation d'Euler
$$
G(T,P,n_{1},n_{2},\dots,n_{N}) = \sum_{i}\times \mu_{i}(T,P,n_{1},n_{2},\dots,n_{N})
$$
Le potentiel chimique wat une grandeur intensive, elle ne dépend que des fractions molaires des différents composants su mélange.
## Uniformité du potentiel chimique d'un composé dans un système biphasé
$$
\mu_{i}^{(l)} = \mu_{i}^{(g)}
$$
À l'équilibre, le potentiel chimique d'un corps pur donné est le même dans toutes les phases 
	rq : Elle reste vraie même quand le système est le siège de réactions chimiques.

# Gaz Parfaits et son Mélanges Idéaux
## Gaz parfait pur
### État standard
À une température T, on appelle la pression standard : 
$$
P^{o} = 1 \text{bar}
$$
### Expression de Potentiel Chimique
(\*) : Le système est constitué d'un gaz pur .
$$
(\frac{\partial \mu^{*}}{\partial P})_{T} = V^{*}_{m}
$$
$$
\mu^{*}(T,P) = \mu^{o}(T) + RT\ln(\frac{P}{P^{o}})
$$
Les fonctions $\mu^{o}$ sont supposées connues.
## Mélange Idéal de Gaz Parfait
### Définition
- qui se comporte globalment comme un gaz parfait
- pour gaz i$$
\mu_{i}(T,P,x_{1},x_{2},\dots,x_{N}) = \mu^{o}_{i} + RT\ln(\frac{x_{i}P}{p^{o}})
$$
### Pression Partielle
La pression partielle de chaque gaz est la pression qu'il aurait s'il était seul dans le volume V.
$$
P_{i} = x_{i}P
$$
$$
P = \sum_{i}P_{i}\text{Loi de Dalton}
$$
$$
\mu_{i} = \mu^{o}_{i}(T) + RT\ln(\frac{P_{i}}{P^{o}})
$$
### G et S et H et U
$$
G = \sum_{i}n_{i}\mu_{i}^{T,P}+RT\sum_{i}n_{i}\ln(x_{i})
$$
$$
S = \sum_{i}n_{i}S^{*}_{m,i}(T,P)-R\sum_{i}n_{i}\ln(x_{i})
$$
$$
H = \sum_{i}n_{i}H^{*}_{m,i}(T,P)
$$
$$
U = \sum_{i}n_{i}U^{*}_{m,i}(T,P)
$$
# Phase Condensée 
## Phase condensée pure
### Imcompressible Indilatable
$$
\mu^{*}(T,P) = \mu^{o}(T) + V^{*}_{m}(P-P^{o})
$$
$$
\mu^{o}(T) = \mu^{o}(T,P^{o})
$$
$V^{*}_{m}$ très petit, négligeable.
### Phase Condensée Idéale 
$$\mu^{*}(T,P) = \mu^{o}(T)$$
## Mélange Idéal de phases condensées
### Définition 
$$
\mu_{i}(T,P) = \mu_{i}^{*}(T)+RT\ln(x_{i})
$$
### Propriétés
$$
S = \sum_{i}n_{i}S^{*}_{m,i}(T,P)-R\sum_{i}n_{i}\ln(x_{i})
$$
$$
H = \sum_{i}n_{i}H^{*}_{m,i}(T,P)
$$
## Solutions Idéales
### Définition 
$$
x_{solvant}\to 1
$$
infiniment diluée
### Potentiel chimique 
$$
\mu_{solvant}(T,P) = \mu^{*}_{solvant}(T,P) = \mu^{o}_{solvant}(T)
$$
### Potentiel chimique de Soluté
$$
\mu_{i}(T,P) = \mu_{i}^{*}(T)+RT\ln(x_{i})
$$
$$
\mu_{i}(T,P) = \mu_{i,c,\infty}^{o}(T)+RT\ln(\frac{c_{i}}{c_{0}})
$$
$$
\mu_{i,c,\infty}^{o}(T) = \mu_{i}^{o}(T)+RT\ln(c^{o}\times V_{m,solvant})
$$
# Activité
## Expression générale du potentiel chimique
$$
\mu_{i}(T,P,x_{1},x_{2},\dots,x_{N}) = \mu_{i}^{o}(T) + RT\ln(a_{i})
$$
- $a_{i}$ : coefficient d'activité; sans dimension 
- $\mu_{i}^{o}$ : potentiel standard
	L'état standard d'un composé est l'état pour lequel l'activité vaut 1

