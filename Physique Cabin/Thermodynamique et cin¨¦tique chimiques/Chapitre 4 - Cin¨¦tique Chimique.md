# Vitesse
## définition
### vitesse de formation et disparition
Ces vitesses sont volumiques. Elles s'expriment en $mol \cdot L^{-1} \cdot{}s^{-1}$.
$$
\mathnormal{v}_{\mathnormal{f}} \overset{\text{def}}=\frac{1}{V}\frac{dn_{i}}{dt} = \frac{d[C_{i}]}{dt}\\
$$
$$
\mathnormal{v}_{\mathnormal{d}} \overset{\text{def}}=-\frac{1}{V}\frac{dn_{i}}{dt} = -\frac{d[C_{i}]}{dt}
$$
$$
v_{d} = -v_{f}
$$
同一个物质可以同时定义这两个量，是algébriques的，有正有负。
produit的formation为正，réactif的disparition为正（通常）
### vitesse de réaction
Elle est volumique.
$$
\mathnormal{v} \overset{\text{def}}=\frac{1}{V}\frac{d\zeta}{dt}
$$
$$
\frac{dn_{i}}{dt} = \nu_{i}\frac{d\zeta}{dt}
$$
$$
v_{d}(C_{i}) = \mid \nu_{i}\mid \times v
$$
$$
v_{f}(C_{i}) = \nu_{i} \times v
$$

### Temps de demi-réaction
$$
t_{\frac{1}{2}}
$$
La moitié de l'avancement final est atteinte.
donne un ordre de grandeur du temps caractéristique.

## Détermination expérimentales
### Principe général
courbe $[A](t)$,en déterminant la dérivee par une méthode graphique ou numérique.
Pour détreminer $t_{\frac{1}{2}}$ 
- pas total:$[A]_{\infty}$
- total:$[A]_{\infty}$ = 0
### Méthodes 
- physique 
	- conductimétrie 
		- $\sigma = \sum_{i,ions}\lambda_{i}\times c_{i}$
	- Spectrophotométrie 
	- PH-métrie
	- Mesure de pression
- chimique 
	- réaction de dosage 
### Facteurs cinétiques
tout ce qui peut influencer la vitesse d'une réaction(pour ce chapitre)
- concentration
- température 
- présence d'un catalyseur 

# Loi de Vitesse
## Définition 
La relation donnant la vitesse de réaction $\mathnormal{v}$ en fonction des concentrations des espèces présentes.
$$
\mathnormal{v} = \mathnormal{f}([C_{1}],[C_{2}],\dots[C_{n}])
$$
Expérimentalement 
## Réaction avec ordre 
Très souvent.
$$
\mathnormal{v} = \mathnormal{k}\times [C_{1}]^{p_{1}}[C_{2}]^{p_{2}}\dots [C_{n}]^{p_{n}}
$$
ordre partiel : $p_{i}$
ordre global : $p = p_{1}+p_{2}+\dots+p_{n}$
constante de vitesse de la réaction : $k$ depend de la temperature
### Pas ordre courant
???

### Cas d'ordre 1
$$\mathnormal{v} = \mathnormal{k}[A]$$
$$
\frac{d[A]}{dt} = -\alpha v = -\alpha k[A]
$$
$$
[A] = [A]_{0}\exp(-\alpha kt)
$$
$$
t_{\frac{1}{2}} = \frac{\ln_{2}}{\alpha k}
$$
rq : La désintégration d'un nucléide radioactif est également un processus d'ordre 1.

### Cas d'ordre 2 par rapport à un seul réactif 
$$
\mathnormal{v} = \mathnormal{k}[A]^2
$$
$$
\frac{d[A]}{dt} = -\alpha v = -\alpha k[A]^{2}
$$
$$
[A] = \frac{[A]_{0}}{1+[A]_{0}\alpha kt}
$$
$$
t_{\frac{1}{2}} = \frac{1}{\alpha k[A]_{0}}
$$
## Simplication d'une loi de vitesse
On simplifie cette loi selon les quantités initialement introduites.
### Cas de réactifs dans les proportions stœchiométriques 
$$
\frac{n_{1,0}}{|\nu_{1}|} = \frac{n_{2,0}}{|\nu_{2}|} = \dots = \frac{n_{n,0}}{|\nu_{n}|}
$$
$$
\frac{A_{1}}{|\nu_{1}|} = \frac{A_{2}}{|\nu_{2}|} = \dots = \frac{A_{n}}{|\nu_{n}|}
$$

$$
v = k^{'}\times[A_{1}]^{p_{1}+p_{2}+\dots+p_{n}} = k^{'}\times[A_{1}]^{p}
$$
$$
k^{'} = \frac{v_{1}^{p_{1}}v_{2}^{p_{2}}\dots v_{n}^{p_{n}}}{v_{1}^{p_{1}+p_{2}+\dots+p_{n}}}
$$
### Dégénérescence de l'ordre
$$
\frac{n_{1,0}}{|\nu_{1}|}\ll\frac{n_{2,0}}{|\nu_{2}|},\dots,\frac{n_{1,0}}{|\nu_{1}|}\ll\frac{n_{n,0}}{|\nu_{n}|}
$$
$$
v = k_{app}\times[A_{1}]^{p_{1}}
$$
$$
k_{app} = k[A_{2}]^{p_{2}}\dots[A_{n}]^{p_{n}}
$$
## Détermination expérimentale d'une loi de vitesse
### Méthode différentielle pour trouver un ordre
$$
\ln(-\frac{d[A]}{dt}) = \ln(\alpha k)+p\ln([A])
$$
### Méthode intégrale pour confirmer un ordre supposé
Seulement $[A]$
On intègre tout d'abord l'équation différentielle correspondante pour savoir quelle fonction de $[A]$ doit être une fonction affine du temps.

### Méthode du temps de demi-réaction
Il est proportionnel à $[A]_{0}^{p=1}$

## Exemples de reactions complexes
### Réaction équilibre avec ordre 1
$$
\frac{[B]_{\infty}}{[A]_{\infty}} = \frac{k_{+}}{k_{-}}
$$
	La loi de Guldberg et Waage.
### Réactions parallèles
$$
\frac{[B]}{[C]} = \frac{k_{1}}{k_{2}} = cte
$$
### Réactions successives

## Mécanismes Réactionnels 
### Notions
#### acte élémentaire
- réaction élémentaire
- molécularité(réactifs)
- loi de vitesse : les ordres partiels sont les nombres stœchiométriques.
#### Intermédiaires réactionnels
- peu stable
- très petit quantité 
- ne figurent pas dans le bilan global

### Influence de la température 
#### Loi d'Arrhenius
Dans les relations avec ordre,
$$
k = \alpha \exp(-\frac{E_{a}}{RT})
$$
$Ea$ est l'énergie d'activation

## Catalyse
### définition 
Sa présence augmente la vitesse d'une réaction,mais qui n'apparaît pas dans l'équation bilan.
#### Catalyse homogène 
Modifier le mécanisme réactionnel 
### Catalyse hétérogène 
Les interactions entre les réactifs et la catalyseur 
### Catalyse enzymatique
- La même phase que les réactifs
- mécanisme, plus proche de celui de la catalyse hétérogène.