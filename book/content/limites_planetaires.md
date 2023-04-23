# Limites planétaires

**Evolution d'une ressource**: (Etienne)

Sujet : Equations différentielles - Limites- Stabilité de l'équation

| 1e | 2e | 3e  | 4e  |
| ----------- | ----------- |-----|-----|
|  |  |     | **x** |

On cherche à étudier l'évolution de la quantité d'une ressource qui se renouvelle et qui est consommée, par exemple le bois issus des arbres. 
On note $Q$ la quantité initiale et $q(t)$ la fonction qui décrit la quantité en fonction du temps. On suppose que la ressource se renouvelle avec un taux $\alpha$ et qu'elle se consomme avec un taux $\beta$.
Chaque année $t$, on consomme donc  $\beta q(t)$ de la ressource, et une quantité $\alpha q(t)$ a été produite. 
On peut écrire que pour tout temps $t \in \mathbb{R}^+$ l'évolution de la quantité $q(t)$ est régie par l'équation différentielle suivante:

$ q'(t) = \alpha q(t) - \beta q(t) = (\alpha - \beta) q(t)$

1. De quel type d'équation différentielle s'agit-il? La mettre sous forme canonique.
2. En notant $\Tau = \alpha - \beta$ et en utilisant les conditions initiales, résoudre l'équation. 
3. Que représente $\Tau$?
3. Quelle est la limite de $q(t)$ en $+ \inf$ pour $\Tau>0$ ? Pour $\Tau<0$ ? Que se passe t'il pour $\Tau=0$ ? 
4. Expliquer ce que chacun des 3 cas représente et tracer $q$ en fonction de $t$ pour chaque cas

5. Quel est le risque de consommer plus de ressource que ce que l'on produit? Mathématiquement quelles sont les solutions pour résoudre ce problème.

En réalité, $\alpha$ et $\beta$ dépendent eux aussi du temps, en particulier la consommation qui n'est pas toujours la même. Ces cas là sont n'ont en général pas de solutions générales.
Cependant, est possible de les résoudre à l'ordinateur (voir activité à ce sujet).


**Gestion d'une population de nuisibles**: (Etienne)

Sujet : Equations différentielles - Stabilité de l'équation

| 1e | 2e | 3e  | 4e  |
| ----------- | ----------- |-----|-----|
|  |  |     | **x** |

Certaines espèces sont considérées comme nuisible pour l'Homme, c'est le cas de certains moustiques ou certaines mouches. Pourtant ces insectes font partis d'un cycle alimentaire entre proie et prédateurs qu'il faut préserver. 
Certains pays tentent donc de réguler les populations des nuisibles. Soit $N$ le nombre initiale de nuisible, on note $f(t)$ la fonction qui décrit l'évolution de la population en fonction du temps. Cette population a un taux de natalité $\alpha$ et un taux de mortalité $\beta$.
En l'absence de l'homme, l'évolution de la fonction $f$ suit l'équation différentielle suivante : 

$ f'(t) = \alpha f(t) - \beta f(t) = (\alpha - \beta) f(t)$

1. De quel type d'équation différentielle s'agit-il? La mettre sous forme canonique. 
2. En notant $\Tau = \alpha - \beta$ et en utilisant les conditions initiales, résoudre l'équation. 
3. Faire une hypothèse sur le signe de $\Tau = \alpha - \beta$ et calculer la limite de $f$ en $+ \inf$. 
4. Tracer la courbe pour une valeur de $\Tau positive.

On suppose maintenant que l'Homme chasse un taux $\delta$ de nuisible en fonction du temps. La nouvelle équation est donc:

$ f'(t) = \alpha f(t) - \beta f(t) - \delta f(t)= (\alpha - \beta - \delta) f(t)

5. On note maintenant $\gamma = \alpha - \beta - \delta$. Que signifie $\gamma$ négatif ?
6. Réécrire la solution de l'équation différentielle en fonction de $\gamma$.
7. Quelle est la limite de $f$ en $+ \inf$ si $\gamma<0$?
8. A quoi correspond le cas $\gamma=0$ ? ( Mathématiquement et dans la vraie vie)
9. Qualitativement, comment devrait évoluer $\gamma$ pour avoir une politique de gestion efficace ? Quel est le risque de vouloir gérer une population via la chasse?

**Limite de la croissance d'une population**: (Etienne)

Sujet : Limite - Equations différentielles

| 1e | 2e | 3e  | 4e  |
| ----------- | ----------- |-----|-----|
|  |  |     | **x** |

Source : https://fr.wikipedia.org/wiki/Dynamique_des_populations and https://en.wikipedia.org/wiki/Logistic_function#In_ecology:_modeling_population_growth

On souhaite décrire l'évolution d'une population dans un environnement donné. On note $N$ le nombre d'individus initialement et f(t)$ la fonction qui décrit l'évolution de la population en fonction du temps.
On suppose que l'environnement peut accueillir $K$ individus en terme de ressources et que la population évolue à un taux $r$ (taux de naissance moins taux de décés).
On peut décrire $f$ avec l'équation différentielle suivante:

$ f'(t) = rf(t) (\frac{K-f(t)}{K})= r f(t) (1-\frac{f(t)}{K}) $

1. Que représente le cas où $f(t)<K$ ? Quel est le signe de $f'$ dans ce cas? Comment va évoluer $f$?
2. Que représente le cas où $f(t)>K$ ? Quel est le signe de $f'$ dans ce cas? Comment va évoluer $f$?

Cette équation a pour solution en fonction de N:

<math display="block">f(t) = \frac{K N e^{rt}}{K + N \left( e^{rt} - 1\right)} = \frac{K}{1+\left(\frac{K-N}{N}\right)e^{-rt}}, </math>

3. Calculer la limite de la fonction en $+ \inf$. Commenter.
Le graphique suivant montre une solution de l'équation différentielle étudiée plus haut:

![](../images/capacity.png)

$k$ représente la limite du nombre d'individus avec la production des ressources d'un environnement.
Une population peut dépasser $K$ en stockant et en consommant plus de ressourses que l'environnement peut en fournir.
Dans ce cas on observe un dépassement de la valeur de K. Comme les ressources stockées ne sont pas éternelles, on obtient des oscillations du nombre d'individus comme sur la courbe ci-dessous:

![](../images/limite.gif)

4. Placer sur le graphique $N$ le nombre initial d'individu et $K$. Repérer des zones où $f(t)<K$ , $f(t)>K$ 
5. Une population peut-elle indéfiniement consommer plus de ressources qu'elle n'en produit?

Note: A comparer avec une croissance infinie : $f'(t) = rf(t) avec r>0$. Possibilités de continuer l'activité via une simulation
