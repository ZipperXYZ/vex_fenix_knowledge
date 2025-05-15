# Boucle
En C++, une boucle sert à exécuter un bloc de code quand certaine condition spécifique sont atteintes.
Les boucles permettent de sauver du temps, réduit le risque d'erreur, et elles rendent le code plus lisible.
## boucle while
Les boucles while permettent d'exécuter un bloc de code quand une condition spécifique est vrai

Par exemple, si vous travaillez en ayant comme objectif d'accumuler 1000$ dans votre compte, vous arrêterez de travaillez quand cette condition sera atteinte.

### Comment créer une boucle while
Voici la syntaxe d'une boucle while : 

    while (condition) {
    	// votre code
    }
   

> Les conditions sont les mêmes que lors d'une condition `if`

   Par exemple : le code s'exécutera en boucle tant que la variable ( **`i`** ) est moins que 5

	int i = 0;
	  
    while (i < 5) {
	    i = i+1  
    }
    // Dans l'exemple, le code s'exécutera 4 fois car rendu à la cinquième ( i )
    // sera égal à 5 et ne respectera plus la condition

Exemple 2 : 

    while (true) {
	   // le code s'exécutera à l'infini  
    }
	
## Les boucles For

Une boucle for est une sorte de boucle. Elle est utilisé quand que vous savez le nombre de fois que vous voulez exécuter un code. 

Par exemple, si quelqu'un a trois pommes et qu'il veut en donner une à ses trois amis, il faudra qu'il fasse l'action de donner une pomme trois fois.

### Comment créer une boucle For

Pour créer une boucle for, il faut, en premier, mettre une variable qui va servir de compteur et de première déclaration dans la boucle for. Il faut, en deuxième, mettre une condition (un peu comme dans les condition **If**) pour déclarer quand que la boucle for devra arrêter. En troisième, il faut déclarer l'incrémentation de la première variable. Pour être plus claire, c'est l'augmentation de la variable.

Voici la syntaxe de la boucle for: 

    for (le compteur, la limite, l'augmentation de la variable) {
		// le code ici
	} 

Voici un exemple en pratique: 

     for (int i = 0, int < 6, i++) {
		// le code serait exécuter 5 fois puisque l'augmentation de 
		// la variable est de 1. La variable va donc se faire 
		// augmenter 5 fois avant d'atteindre la limite.
	} 
    
> les `++` après la variable `i` est l'équivalent d'écrire `i = i + 1`
