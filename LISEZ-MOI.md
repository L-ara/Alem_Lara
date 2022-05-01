# LE JUSTE PRIX


![Le juste prix](https://upload.wikimedia.org/wikipedia/en/f/f6/Logo_Le_Juste_Prix.png) 


## But du jeu:  
Le but du jeu est d'accroitre sa cagnotte en amassant le plus de gains possible. Pour cela, le candidat aura un nombre limité à 5 tentatives pour deviner un prix, mais pas n'importe lequel,__" LE JUSTE PRIX !"__. Il fera alors des estimations et celui qui aura donné l'estimation la plus proche du juste prix aura gagné.


## Programmation:
Le programme va donc génèrer un prix rond aléatoire (au hasard) situé entre 1€ et 500€. Chaque fois que l’utilisateur (le candidat) fait une estimation différente du juste prix, l’ordinateur lui dira si c’est plus (lorsque son estimation est inférieure au juste prix) ou moins (lorsque son estimation est supérieure au juste prix).  


* Le juste prix ayant été choisi au hasard (nombre aléatoire), nous utiliserons la fonction random : 
`import random`  
`juste prix = random.randint (1,500)`. 


* Le nombre de tentatives étant limité à 5, nous utiliserons une boucle `while . Nous aurons alors les 3 possibilités suivantes:  
  * L'utilisateur donnera un prix inférieur au juste prix, dans ce cas-là le programme renverra `"C'est plus !"`;   
  * L'utilisateur donnera un prix supérieur au juste prix, dans ce cas-là le programme renverra `"C'est moins !"`;  
  * L'utilisateur donnera un prix égal au juste prix, dans ce cas-là le programme renverra `"Félicitations, vous avez trouvé le juste prix !"` et nous utiliserons donc la fonction `break` pour sortir de la boucle.

* Enfin, la dérnière étape du code sera d'afficher le résulat selon le nombre de tentatives de l'utilisateur : s'il a réussi à trouver le juste prix, en combien d'essai ? Sinon, si l'utilisateur n'a pas réussi à le trouver au bout des 5 essais, on affichera le message `"Oh non! Vous avez dépassé les 5 tentatives autorisées."` et en précisant le juste prix choisi aléatoirement par l'ordinateur.  

* Enfin on modélisera quelques possibilités (graphiquement) traduisant des estimations du juste prix.
