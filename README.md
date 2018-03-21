# StadLine Technical Test

### Tache

Le sujet de base est simple : Il faut créer une page permettant de suivre le score d'une partie de bowling d'un unique joueur.

### Règles du test

* Le temps est libre mais il est tout de même conseillé de passer moins de 4h sur le sujet (temps de setup d'environnement compris)
* Il est conseillé de finir les points requis avant de s'attaquer au bonus. 
* Il est aussi conseillé de faire un maximum de commit pour bien détailler les étapes de votre raisonnement au cours du développement.
* N'hésitez pas à nous faire des retours et nous expliquer les éventuelles problématiques bloquantes que vous auriez rencontrées durant le développement vous empéchant de finir.

### Setup

* La charte graphique n'est pas imposée et sera jugée en bonus. L'emploi d'un framework CSS type Twitter Bootstrap est fortement conseillé. 
* Inutile de réinventer la présentation d'une feuille de socre de bowling : [en voici des tas d'exemples](https://www.google.fr/search?q=bowling+scoreboard&espv=2&biw=1680&bih=849&source=lnms&tbm=isch&sa=X&ved=0ahUKEwjG38Dx3YrSAhXHvRQKHR8VD1YQ_AUIBigB)

### Les pré-requis

* Lors d'une première étape on demandera à l'utilisateur de saisir le déroulé sous forme d'une chaîne.
  Les chaînes saisies seront la suite du nombre de quilles qui tombent à chaque lancer. Dans cette chaîne de caractères un X signifie un strike, un / signifie un spare et un - signifie un manqué. Exemples de chaînes : 
```XXXXXXXXXXXX```, ```9-9-9-9-9-9-9-9-9-9-```
* Dans une seconde étape on affichera le score et le déroulé sous forme de tableau

### Les règles

Une partie de bowling se déroule en 10 "frames". 
A chaque frame, le joueur lance donc une ou deux boules afin de faire tomber les 10 quilles :
  * Si après 2 lancers, toutes les quilles ne sont pas tombées, le socre de la frame est égal au nombre de quilles à terre
  * Si le joueur utilise les 2 lancers pour faire tomber les 10 quilles, il s'agit d'un spare. La frame rapporte 10 points plus le nombre de quilles qui seront abattues par la boule suivante
  * Si le joueur utilise 1 seul lancer pour faire tomber les 10 quilles, il s'agit d'un strike. La frame rapporte 10 points plus le nombre de quilles qui seront abattues par les deux boules suivantes.
  * Lors de la dernière frame, le joueur peut être amené à lancer 1 ou 2 boules supplémentaires respectivement s'il a fait un spare ou un strike.
  
#### Exemples de scores

 * XXXXXXXXXXXX (la partie parfaite) rapporte 300 points
 * 9-9-9-9-9-9-9-9-9-9- rapporte 90 points
 * 5/5/5/5/5/5/5/5/5/5/ rapporte 150 points

### Bonus

* Afficher si la partie est terminée
* Afficher les scores frame par frame (c'est du bonus, on se concentrera principalement sur le score final avant de faire les scores intermédiaires)
* Validation de la chaîne
* Responsive
* Multiplayer
* Toutes les fonctionnalités que vous aurez le temps d'ajouter seront aussi bonnes à prendre. Un bonus autour de votre créativité pourra être considéré.

### Délivrabilité

* Forkez le projet sur GitHub et codez directement dans le projet forké. 
* Commitez aussi souvent que possible et commentez vos commits pour détailler votre chemin de pensée. 
* Mettez à jour le README pour ajouter le temps passé et tout ce que vous jugerez nécessaire de nous faire savoir (déploiement, dépendances ...). 
* Envoyez le lien avec le projet à recrutement@stadline.com. 

**Bonne chance !**
