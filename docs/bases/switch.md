# Les switch
Les switch sont une autre façon de sélectionner un certain bloc de code . Par exemple, si vous ne voulez pas faire une condition `if` et que vous voulez directement allez a un certain bloc de code, les switch sont parfait pour cela.

## Comment créer un switch

Pour créer un  switch c'est très simple, il faut, en premier, écrire le switch. Après  cela, il faut mettre, entre parenthèse, un `int` qui va donner au switch l'information de quel bloc de code exécuter. il faut après créer les bloc de case en utilisant le 

voici la syntaxe: 

    switch (int chiffre) {
		case x:
			// un bloc de code ici
			break;
		case y:
			// un autre ici
			break;
		default:
			// le bloc de base
	}

> Le `default` est en fait le bloc de base qui est exécuter si le chiffre ne représente aucune case.

## Comment un un switch marche

Un switch va en fait prendre la valeur de son expression (le `int chiffre`) et va l'associer a une des case.

Par exemple:

    int action = 4;
    
    switch (action) {
	    case 1:
		    // faire une certaine action
		    break;
		case 2:
			// faire une autre action
			break;
		case 3:
			// faire une autre action
			break;
		case 4:
			// cela représente l'action qui va être exécuter parce 
			// que le int action est égal à 4 et la case 4 est
			// celle-ci
			break;
    }
	
	

> Un break est une façon de dire au code de s'arrêter a un certain point. On peut aussi l'utiliser dans des boucle **while** et **for**, dans des **fonctions** et à d'autres endroits

