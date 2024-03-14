# Le Problème des grandes dimensions 
- de grande dimension 
- en grandes quantité 

# L'analyse en composantes principales
	Nous aurons besoin de faire des raisonnement affine dans un espace euclidien E.
## Notation
- $\vec{x} \in E$, comme un vecteur
- $X \in E$ comme un point

## Cas particulier de la dimension 1
### Droite de Régression Orthogonal 
La droite qui minilise
$$
\sum_{j=1}^{n}d(X_{i},\Delta)^{2}
$$
	On minimise la composante $V^{\perp}$
#### Distance à une Droite Affine
$$
d(X,\Delta)^{2} = ||\vec{\Omega X}||^{2}-<\Omega X,\vec{u}>^{2}
$$
	Dans la droite de répression orthogonale 
	$$
	\Omega = G,\vec{u} = \vec{e}
	$$
	où $\vec{e}$ est un vecteur propre unitaire associé à la plu grande valeur propre de la matrice $B ^{t}B$

#### Deux types de régressions linéaires dans le plan

#### Cas ou on connait une base orthonormee de E

## Les Autres Dimensions
	Pouvoir garder un peu plus de dimensions et d'évaluer la perte d'information.
### Sous-espace Principal
sous-espace principal de dimension k du nuage de points
$$
\sum_{j=1}^{n}d(X_{j},\mathcal{V})^{2}
$$
est minimal

### Analyse en Composantes Principales
$$
\Omega = G,(\vec{e_{1}},\dots,\vec{e_{k}})
$$
une famille orthonormée de vecteurs propres associés aux k plus grandes valeurs propres de la matrice $B ^{t}B$

### Composantes Principales
Les vecteurs propres trouvés.

### Mesure de la qualité de la projection 
$$
\frac{\sum_{s=1}^{k}\lambda_{s}}{\sum_{s=1}^{p}\lambda_{s}}
$$
	En IA, on a très souvent besoin de préparer les données pour pourvoir les exploiter.

# La Décomposition en valeurs Singulières


	感觉还是得找个时间把代码敲一遍