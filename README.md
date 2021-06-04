# Blockchain Demo pour des étudiants

Ce répertoire contient une démo à faire avec des étudiants du niveau gymnase.
Il s'agit pour eux de travailler ensemble de la même manière que les nœuds travaillent
ensemble dans une blockchain.

Durée de préparation pour l'enseignant: 1h-2h
Durée de la démo: 1h-2h

Ce que les étudiants peuvent apprendre avec ce démo:
* Le sense du Proof-of-Work
* Comment les blocs sont reliés entre eux
* Faire un consensus dans un système décentralisé

# Préparation

Pour donner une motivation aux étudiants, on peut leur proposer qu'à la fin ils·elles peuvent
récupérer leur récompense dans la blockchain en forme de chocolat et/ou de fruits.
Donc il faut que l'enseignant prépare des récompenses pour un total de 15-20 points.

On peut faire le jeu soit avec un chat et es ordinateurs, soit manuel avec du papier.

## Ordinateur et chat

Dans ce cas, il faut donner aux étudiants accès aux choses suivantes:
- BrainCoin - Feuille de calcul: attention, chaque groupe d'étudiants doit avoir sa propre feuille!
- un groupe de chat où ils peuvent envoyer leur solution à l'enseignant
- s'assurer que le partage de l'écran de l'enseignant fonctionne

## Papier

Le jeu marche aussi très bien avec seulement du papier.
Pour ceci il faut imprimer la feuille suivante pour chaque groupe d'étudiants:
- BrainCoin - Feuille de calcul - multiples

En plus il faut imprimer des "Blocs", en tout cas 4 ou 8 par groupe:
- BrainCoin - Bloc - 4x4

## Identités des groupes

L'algorithme pour calculer le _Proof-of-work_ est très simpliste et ne donne pas
toujours un résultat qui permet de faire un bloc.
Les meilleures identités sont ceux qui se terminent en `0`, `6`, et `8`.
Donc dans la préparation il faut introduire des identités soit sur les feuilles, soit
sur les fichiers à distribuer.
On peut ajouter n'importe quel chiffre de dizaine. Le `10` va être traité
de la même manière que le `20`, vu qu'on ne prend que le dernier chiffre.

## Ouverture de la blockchain

Dans le fichier `index.html` il y a une blockchain très simple qui permet de visualiser
l'avancement de la chaîne.
Assurez-vous que vous arrivez à ouvrir le fichier et que ça s'affiche correctement.

## Assistants

Il est très utile d'avoir 1 ou 2 assistants qui peuvent vous aider à trier les blocs
quand ils arrivent.
Surtout vers la fin du jeu il y a souvent plusieurs groupes qui ont des blocs à ajouter,
et vous n'auriez pas le temps d'expliquer à toutes les élèves qui viennent pourquoi leur
bloc ne passe pas.
Le mieux est qu'il y a les deux assistants qui vérifient si les blocs sont valides par
rapports aux points suivants:
* Compteur: est-ce que c'est bien un numéro qui peut s'insérer dans la chaîne existante?
* Last proof-of-work: est-ce que ceci existe avec le compteur indiqué?
* Proof-of-work: est-ce que le dernier chiffre est bien en-dessous ou égal au target?
* Target: est-ce que c'est bien 2 pour un premier bloc du groupe, ou plus petit dans
le cas des blocs suivants dans la chaîne?

En faisant ceci, les assistants peuvent alléger le travail de l'enseignant qui va
saisir les blocs.

## Exercice blanche

Il faut absolument faire l'exercice une fois en avance.
Par exemple avec les profs du gymnase ou d'autres personnes, au moins 5 groupes.
Si possible avec les assistants présents pour qu'ils puissent voir quelles sont les
questions qui viennent souvent.

Sans une exercice préalable, l'exercice avec les étudiants a de fortes chances
de tomber à l'eau!

# Déroulement

## introduction

Il faut d'abord faire une petite introduction sur les blockchains, par exemple avec
les transparents dans `Blockchain - Introduction` de ce répertoire.
Après vous pouvez disposez les étudiants en groupe.
Le mieux est d'avoir un total de 10 groupes.
S'il y en a plus, ça serait trop rapide vers la fin, s'il y a moins, autant faire les
groupes plus petits, c'est plus chouettes pour les étudiants.

## BrainCoin

Commencer avec les 5 premiers transparents de la présentation
`BrainCoin - Transparents`.
Puis demandez-leur de se séparer en 10 groupes.
Distribuez les feuilles et passer les transparents 6 à 40, en bien indiquant les
liens entre les transparents et les feuilles qu'ils·elles ont reçues.

Laisser le temps pour des questions, et n'hésitez pas à refaire l'exemple.

## Minage

Une fois que tout le monde a ses feuilles, et qu'ils ont inscrits leur nom de groupe
et copié le premier chiffre de leur identité, le jeu peut commencer.
Faites un compte à rebours et afficher ou recharger la page pour afficher un nouveau
bloc avec un nouveau `Proof-of-work`, afin que tout le monde puisse commencer ensemble.

Pendant le minage il est important que les assistant font la pré-vérification, et que c'est
seulement eux qui discutent avec les étudiants.
La personne qui entre les blocs sur le site n'a pas le temps de faire aussi
l'explication!

## Motivation

Réfléchissez bien comment vous pouvez motiver les étudiants qui ont de la peine
à faire des calculs.
Le système est fait de façon que ceux qui ont déjà une avance auront plus de peine
à trouver une solution, donc ça aide déjà un peu.

## Finaliser le jeu

On peut faire 10 à 15 blocs, qui prend à peu près 15-20 minutes.
Il ne faut pas hésiter à faire quelques commentaires, surtout au début, pour rappeler:
* travailler avec la chaîne la plus longue
* pas oublier de correctement mettre à jour la feuille

2 blocs avant la fin on peut déjà annoncer qu'on va s'arrêter au bloc 10 ou 15.
Ceci aide les étudiants à se préparer qu'ils ne vont peut-être pas pouvoir ajouter
leur bloc en route.

## Fin du jeu

Une fois que le 10ème ou le 15ème bloc est affiché, on proclame la fin du minage.
On peut maintenant afficher la chaîne gagnante, qui est en vert.
Pour chaque groupe qui a au moins un bloc dans cette chaîne, compter le nombre
de blocs.
Ce nombre correspond aux points gagnés par ce groupe.

## Explications

Demandez aux étudiants comment ça s'est passé.
Répondez aux questions qui se posent, si vous ne le savez pas, encouragez-les
de chercher la solution eux-mêmes.

Puis terminez avec les transparents.

## Distribution des récompenses

A la fin on peut laisser chaque groupe choisir les récompenses désirés.
