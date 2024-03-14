# Modèle Scalaire
## Définition
signal lumineux, amplitude lumineuse, un champ réel
$$
s(M,t)
$$
## Superposition
$$
s(M,t) = s_{1}(M,t)+s_{2}(M,t)
$$
## Ordre de grandeur

## Éclairement 
### Puissance lumineuse
$$
dP(M,t) = Ks^{2}(M,t)dS
$$
$$
K = 2
$$
### Éclairement 
L'intensité (ou éclairement) 
$$
I(M) = 2<s^{2}(M,t)>
$$
$$
I(M) = \frac{P}{S}
$$
可能是这个关系
rq : Extension spatiale du détecteur

## Onde lumineuse monochromatique
### Définition 
$$
s(M,t) = a(M)\cos(\omega t-\phi(M))
$$
$\phi$ est la phase retard de l'onde au point M
- longeur d'onde dans le vide : $\lambda_{0} \overset{ \text{def} } = c\frac{2\pi}{\omega }$
- pulsation spatiale : $k_{0} \overset{ \text{def} } = \frac{\omega}{c} = \frac{2\pi}{\lambda_{0}}$
- signal complexe : $\underline{s}(M.t)\overset{ \text{def} } = a(M)\exp j(\omega t-\phi(M))$
- amplitude complexe : $\underline{A}(M) \overset{ \text{def} } = a(M)\exp[-j\phi(M)]$
### éclairement d'une onde monochromatique
$$
I = a^{2}(M)
$$
$$
I = \underline{s}(M,t)\times \underline{s}^{*}(M,t) = |\underline{s}(M,t)|^{2} = |\underline{A}(M)|^{2}
$$
复数部分被消掉了
Les détecteurs sont insensible à la phase de l'onde.

# Propagation et Déphasage 
## Chemin Optique
### Définition
	就是光在介质中走过这段路程所花费的时间允许它在真空中走过的路程
	
$$
(SM) \overset{ \text{def} } = c\times \tau_{SM}
$$
- cas général 
- cas d'un milieu uniforme 
## Déphasage 
### Relation générale 
$$
s(M,t) = \gamma \times s(S,t-\tau_{SM})
$$
$$
a(M) = \gamma a(S),\phi(M) = \phi(S)+\omega \tau_{Sm} = \phi(S)+k_{0}(SM)
$$
### Dans un milieu
$$
\lambda = \frac{\lambda_{0}}{n},k = n\times k_{0}
$$
## Surface d'onde
ou surface équiphase, l'ensemble des points M ayant la même phase.
Elles sont fixes dans l'espace.
### Surface d'onde pour une source ponctuelle
$$
(SM) = ste
$$
### Théorème de Malus
Après un nombre quelconque de réflexion et de réfraction, les rayons lumineux issus d'une source ponctuelle sont orthogonaux aux surfaces d'onde.
### Stigmatisme et chemin optique
Le chemin optique qui relie deux points conjugués est indépendant du rayon considéré.

## Ondes fondamentales
### Ondes sphériques
$$
<P_{R}> = \overset{ sphère }\int \int I(M)\times dS_{M} = a^{2}(R)\times 4\pi R^{2}
$$
### Ondes Planes
vecteur d'onde

# Autres Phénomènes affectant le signal optique 
## Changment d'amplitude : absorption
$$
\gamma_{NM} = e^{-\alpha \times NM}
$$
## Réflexion et transmission en amplitude
$$
\underline{A_{r}}(M^{r}) = r \underline{A_{i}}(M^{i}),\underline{A_{t}}(M^{t}) = t \underline{A_{i}}(M^{i})
$$
- r : coefficient de réflexion en amplitude 
- t : coefficient de transmission en amplitude 
- R : coefficient de réflexion en puissance 
- T : coefficient de transmission en puissance
$$
R = \frac{I_{r}}{I_{i}} = \frac{n_{1}|\underline{A_{r}}(M^{r})|^{2}}{n_{1}|\underline{A_{i}}(M^{i})|^{2}} = |r|^{2}
$$
$$
T = \frac{I_{t}}{I_{i}} = \frac{n_{2}|\underline{A_{t}}(M^{t})|^{2}}{n_{1}|\underline{A_{i}}(M^{i})|^{2}} = \frac{n_{2}}{n_{1}}|t|^{2}%%
$$
$$
R+T = 1
$$
	实际情况中，功率跟材料的折射率有关系
### incidence normal
$$
r = \frac{n_{1}-n_{2}}{n_{1}+n_{2}},t = \frac{2n_{1}}{n_{1}+n_{2}}
$$
$$
\mid r\mid^{2}+\frac{n_{2}}{n_{1}}\mid t\mid^{2} = 1
$$
## Réflexion sue un miroir parfait 
## Passage par un point de convergence
