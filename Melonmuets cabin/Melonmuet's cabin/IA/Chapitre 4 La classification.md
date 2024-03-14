	Faire apparaître des groupes permettent de donner les données des catégories. On soit capable de donner un sens réel aux classes.
# Quelques Notions
## Inertie
inertie de la famille $\mathcal{X}$, par rapport à $\mathcal{F}$ la valeur
$$
\sum_{k=1}^{n}d(x_{k},\mathcal{F})^{2} 
$$
## Théorème de Huygens 
$$
\mathcal{J}_{\mathcal{F}}(\mathcal{X}) = \mathcal{J}_{\mathcal{F_{0}}}(\mathcal{X})+nd(G,\mathcal{F})^{2}
$$
## Inertie inter-classe
$$
\mathcal{J}^{inter}_{\mathcal{F}} \overset{\text{not}}= \sum_{q \in Q}n_{q}d(G_{q},\mathcal{F})^{2}
$$
## Inertie intra-classe
$$
\mathcal{J}^{intra}_{\mathcal{F}} \overset{\text{not}}= \sum_{q \in Q}\mathcal{J}_{\mathcal{F_{q}}}(q)
$$

# La Classification Supervisée
	Trouver une fonction qui affecte le mieux tout nouvel individu à sa classe.
## Analyse discriminante linéaire 
### Apprentissage
#### Sous-espace Discriminant
- Maximise minimise l'inertie inter-catégorie
- Minimise maximise l'inertie intra-catégorie
#### Citation
Un sous-espace discriminant de dimension s contient G et est dirigé par s vecteurs propres associés aux plus grandes valeurs propres de la matrice
$$
(B ^{t}B)^{-1}\left( \sum_{q \in Q} n_{q}\Phi \vec{GG_{q}}^{t}\Phi \vec{GG_{q}}\right)
$$
#### Problème de dimensions 
还没看懂
### Reconnaissance
	Ne soit pas assez entraîné.
	- le plan discriminant

#### Probabilité d'affectation 
#### Qualité de la discrimination 
#### Diagramme de Voronoi
La partie du découpage associée à $p \in S$ est définie par
$$
Vor_{s}(p) = {x \in E, \forall s \in S, d(x,p) \le d(x,s)}
$$

## Méthode de k-voisins
- On se fixe k.
- Pour tout nouvel individu, il appartient à la classe majoritaire de ses k plus proches voisins.
	Il fonctionne mal en grandes dimensions.

# La Classification Non Supervisée
	On ne précise pas les classes des individus.Le travail de les interpréter reste à la charge de l'utilisateur .
## La Classification Hiérarchique 
- $\Delta_{0} = \{\{x\},x \in E\}$
- $(A,B) \in \Delta_{n}^{2}$, qui minimise $\delta$, notons le $(A_{n},B_{n})$
- $\Delta_{n+1} = (\Delta_{n}\\\{A_{n},B_{n}\})\cup\{(A_{n}\cup B_{n})\}$
	$\delta$ est très important dans cet algorithme 
### Distance de Ward
	Permettre de minimiser la perte d'inertie inter-classe

$$
\delta(A,B) = \frac{n_{A}n_{B}}{n_{A}+n_{B}}d(G_{A},G_{B})^{2}
$$
### La Méthode des k-moyennes
- $\mu_{1}^{(0)},\dots,\mu_{1}^{(k)}$
- $Vor_{Sp}(\mu_{j}^{(0p}) = \{x_{k},\forall i \in |1,k|,|x_{k}-\mu_{j}^{(p)}| \le |x_{k}-\mu_{i}^{(p)}|\}$, p itérations
- $S_{p+1} = \left\{ \frac{1}{card(Vor_{Sp}(\mu_{j}^{(p)}))}\left( \sum_{x \in Vor_{Sp}(\mu_{j}^{(p)})}x \right),j \in |1,k| \right\}$