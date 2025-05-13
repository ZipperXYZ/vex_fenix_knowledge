# les fonctions🖥️
Une fonction est un bloc de code qui est possible d'appeler pour faire une certaine action. **Par exemple, une fonction pourrait être utilisée pour lancer un autonome.**

## Comment créer une fonction❓
Pour créer une fonction, il faut, en premier, **mettre le type de variable que la fonction va retourner.**

Par exemple, la fonction pourrais retourner un `int` un `bool` et d'autres types de variable.

En deuxième, il faut écrire le nom de la fonction. Le nom peut être n'importe quoi. **La seul restriction est qu'il ne peut pas avoir d'espace et il ne peut pas avoir de tirets.**

En troisième, il faut écrire des `( )` pour déclarer que c'est une fonction.

Pour finir, il faut écrire des `{ }` à la fin pour déclarer ce qui est à l'intérieur de la fonction .

Au final, Une fonction ressemble à cela: 

	void fonction() {
	    // faire quelque chose
	}

> Une fonction avec `void` comme type est une fonction qui ne va rien retourner.

## Les retours des fonctions🔙

Les retours dans une fonction est une variable qui est retourner par la fonction. Par exemple:

La fonction ci-dessous va retourner l'addition entre le chiffre 8 et le chiffre mit en argument.

    int additionner(int chiffre) {
	    return 8 + chiffre; 
	}
	
	int variable1 = additionner(3);
	
	// la variable serait donc égal à 11 parce que 8 + 3 = 11  

## Les paramètres☂️

Dans une fonction, il est possible de mettre des paramètres. Il faut, dans les `()` de la fonction, écrire une variable qui va être utilisée en tant que que paramètre.

    void fonction(int chiffre) {
		// la variable va être égal à sa valeur qui est indiqué quand
		// que vous appeler la fonction. 
    }
	 
	 // la variable "chiffre" va être égal à 3 dans la fonction  
	fonction(3);
## Comment appeler une fonction📞

Pour appeler une fonction (et donc exécuter le code à l'intérieur) il faut simplement écrire le nom de la fonction et après mettre les `( )` et les paramètres de la fonction (s'il y en a).

Par exemple: 

    int autonome1(int numéro) {
		// faire la routine autonome
		return 1;
	}
	
	int main() {

		// Initializing Robot Configuration. DO NOT REMOVE!
		vexcodeInit();
		// Begin project code
		
		autonome1(4);
		
		// la fonction autonome1 va être exécuter après la 
		// configuration initial de vex avec le paramètre 
		// "chiffre" avec une valeur de 4
	}

> La fonction `main` est la première fonction qui est exécuter dans le
> programme C++. La fonction  `vexcodeInit` est la fonction qui initialise les composantes de vex **NE LA SUPRIMER PAS SAUF SI VOUS SAVEZ CE QUE VOUS FAITE**


