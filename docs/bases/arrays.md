# Les arrays
Un array sert avant tout à stocker les informations sous forme de liste, c'est un peu semblable à une liste d'épicerie.

## Comment les utiliser
1- Pour commencer, vous avez besoin de dire quelle type de donnée sera stocker dans votre array. 

Par exemple, vous pourriez mettre : 
- int
- double
- bool

2- Le nom de l'array dois être descriptif et unique, Vous devez attribuer une longueur à l'array entre crochet **`[]`** juste après le nom.

Par exemple :  **`int turnAngles[3];`**
> Le point-virgule sert à mettre fin à la ligne et à passer à la suivante

3- Les valeurs de l'array peuvent être défini à leurs créations à l'aide d'accolade

Par exemple : **`bool boolArray[2] = { false, true };`**

4- Les valeurs de l'array peuvent aussi être défini individuellement par index 
> l'Index est la position de la variable dans l'array

Par exemple : 

    bool boolArray[2] = { false, true };
    bool variable = boolArray[0];
	
	// la variable va être égal à false parce que la position 0 de l'array est la
	// valeur false
	// si l'index aurait été égal à 1 la valeur aurait été true

5- Pour lire les valeurs de l'array, inscrivez l'index d'un élément entre crochets
Par exemple : **`int value = integerArray[2];`**