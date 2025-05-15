# Les conditions if/else
Une condition if else est un peu comme quelqu'un qui veut renter dans un bar. Par exemple, une personne VIP pourra rentrer facilement alors qu'une personne qui n'a pas de pièce d'identité ne pourra pas.


## Comment créer une conditions

Pour commencer, il existe 3 types de conditionneurs.

|Conditioneurs| Explication |
|--|--|
| `if` | une condition simple qui décrit que si une certaine valeur	 est égal a répond a un certain critère, elle fait un certain bloc de code 
| `else if` | une autre condition qui va être prise en compte si la première est fausse.
| `else` | le bloc de code qui va être exécuter si aucune des autres conditions n'ont été vrai.

Les conditions If/Else utilisent des opérateurs de comparaison pour faire leur condition. 

Un opérateur de comparaison est un opérateur qui est utilisé pour comparé deux variables. Pour être plus claire, c'est les opérateurs plus petit, plus petit ou égal, etc. 

| Opérateurs | Explication |
|--|--|
| `a < b` | plus petit que |
| `a <= b` | plus petit ou égal que |
| `a > b` | plus grand que |
| `a >= b` | plus grand ou égal que|
| `a == b` | égal à|
| `a != b` | pas égal à|



Pour créer une condition, Il faut, en premier mettre un conditionneur comme un  `if`. Après cela, il faut mettre entre `( )` en utilisant les opérateurs de comparaisons.

Voici un exemple: 

    int variable = 3;
	
	if (variable > 4) {
		// ce bloc de code ne va pas être exécuter parce que
		// n'est pas pas plus grand que 4 
	} else if (variable > 2) {
		// ce code serait exécuter car 3 est plus grand que 2
	} else {
		// ce code serait exécuter seulement si les 2 autres
		// conditions auraient été fausses
	}

En résumer, la première condition `if (variable > 4)` ne va pas être exécuter car la variable n'est pas plus grande que 4. La deuxième condition `else if (variable > 2)` va être exécuté parce que la variable est plus grande que 2. La troisième condition serait exécuter si aucune des 2 autres auraient été vrai.