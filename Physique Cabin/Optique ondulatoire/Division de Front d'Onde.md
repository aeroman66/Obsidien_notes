# Principe de l'Expérience des Trous de Young
## Diffraction de la Lumière par un trou
- Un trou de très petite dimension (comparable ou plus petit que la longeur d'onde de la lumière)
- Sous-source : une source ponctuelle
-  L'amplitude du signal en M est proportionnelle à la surface du trou.
## Schéma expérience
### Description
trois éléments principaux 
- une source principale S, ponctuelle, monochromatique
- un plan opaque: plan des trous
- un écran d'observation
### Différence de marche
Il faut regarder la démonstration.
	较为简单的展开即可。
$$
\delta_{2|1} = a\frac{x}{D}
$$
## Figure d'interférences
### Géométrie 
$$
\delta_{2|1} = m\lambda_{0} , \delta_{2|1} = (m+\frac{1}{2})\lambda_{0}
$$
### Éclairement 
$$
I(M) = 2I_{0}(1+\cos k_{0}\delta_{2|1}(M)) = 2I_{0}(1+\cos(\frac{2\pi}{\lambda_{0}}\frac{ax}{D}))
$$
Le phénomène d'interférences conduit à une redistribution de la puissance lumineuse dans l'espace.Il n'y a ni gain ni perte de puissance.

# Variation sur l'Expérience des trous de Young
## Observations à l'infini
### Montage
### Différence de marche 
$$
\delta_{2|1} = a\frac{x}{f^{'}}
$$
$$
i = \frac{\lambda_{0}f^{'}}{a}
$$
## Élargissement incohérent de la source 
### Déplacement de la source
$$
\delta_{2|1} = a\frac{x}{D}+a\frac{X}{D^{'}}
$$
L'interfrange i reste la même.
### Remplacement de la source ponctuelle par une fente incohérente éclairée
$$
I = 2I_{0}[1+\sin c(\pi\frac{L}{L_{b}})\cos(k_{0}\frac{ax}{D})]
$$
### Étude de la figure d'interférence 
$$
I = 2I_{0}(1+v\cos(k_{0}\frac{ax}{D}))
$$
Le paramètre de visibilité :
$$
v \overset{\text{def}} = \sin c(\frac{\pi L}{L_{b}}) = \sin c(\frac{\pi La}{\lambda_{0}D'})
$$
Dans tous les cas, le contraste de la figure d'interférences est donné par la relation : 
$$
\gamma = |\sin c(\frac{\pi L}{L_{b}})|
$$
### Bilan
- Le contraste est indépendant de la dimension selon Oy.
- Le contraste tend globalement à diminuer lorsque la largeur de la fente augmente.
- Les franges se brouillent uniformément ,en tout point de l'écran.
- $L = n \times L_{b}$, le contraste est nul.
- La diminution de contraste lorsque L augmente n'est pas monotone.
	Il est donc, très difficile, avec ce type de dispositif, d'obtenir des franges très lumineuses.因为你得保证光源很细，只能增加它的长度，通光量其实很小。
## Fentes de Young
...

# Interférences à N ondes - Réseaux
## Interférence à N ondes
### Description
- réseau de fentes
- pas de réseau :nombre de traits par unité de longueur. 
$$
n_{f} = \frac{1}{a}
$$
### Montage expérimental - Configuration de Fraunhofer
- La source et l'observations sont à l'infini.
- Les angles d'incidence et observation ne sont pas nécessairement petits.
### Déphasage entre deux ondes adjacentes
$$
\delta_{n|n+1} = a \times(\sin \theta_{obs}-\sin i)
$$
	这里的角度都是又方向的，这会影响相位差的大小
## Caractéristiques générales de l'éclairement 
### Maxima principaux : relation des réseaux 
$$
a \times(\sin \theta_{obs}-\sin i) = m\lambda_{0}
$$
- m : l'ordre de diffraction
- m = 0, $\theta_{obs} = i$, toujours un maximum d'éclairement.
### Éclairement maximum 
$$
\underline{A}_{n}(M_{\infty}) = \underline{A}_{1}(M_{\infty})\exp(-j\delta \phi _{n|1}) = \underline{A}_{1}(M_{\infty})\exp(j(n-1)\delta \phi)
$$
$$
I_{max} = N^{2}I_{0}, \delta \phi = 0
$$
### Éclairement en dehors des maxima
$$
I_{tot} = I_{0} \times \frac{\sin^{2}\left( \frac{N\delta \phi}{2} \right)}{\sin^{2}\left( \frac{\delta \phi}{2} \right)}
$$
Dès que N est plus grand qu'une certaine, on peut complètement négliger l'éclairement diffracté en dehors des directions des maxime principaux.
## Réseau réel 
La relation des réseaux est valable pour toute structure périodique unidimensionnelle de période a.

# Conséquence de la relation des réseaux 
## Nombre d'ordres observables
$$
-1\leq \sin \theta_{m}<1
$$
$$
\frac{a}{\lambda_{0}}(-1-\sin i)\leq m\leq\frac{a}{\lambda_{0}}(1-\sin i)
$$
## Déviation dans un ordre donné
$$
D_{m} = \theta_{m}-i
$$
$$
\frac{dD_{m}}{di} = \frac{\cos i}{\cos \theta_{m}}-1
$$
$$
i = -\theta_{m}
$$
$$
\sin(\frac{D_{m,min}}{2}) = m\frac{\lambda_{0}}{2a}
$$