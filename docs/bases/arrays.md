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

3- Les valeurs de l'array peuvent être défini à leurs créations à l'aide d'accolade.

Par exemple : **`bool boolArray[2] = { false, true };`**

4- Les valeurs de l'array peuvent aussi être défini individuellement par index. 
> l'Index est la position de la variable dans l'array

Par exemple : 

    bool boolArray[2] = { false, true };
    bool variable = boolArray[0];
	
	// la variable va être égal à false parce que la position 0 de l'array est la
	// valeur false
	// si l'index aurait été égal à 1 la valeur aurait été true

5- Pour lire les valeurs de l'array, inscrivez l'index d'un élément entre crochets.

Par exemple : **`int value = integerArray[2];`**

# Array 2d
Pour faire simple une array 2d est une array dans une autre array.

## Comment les utiliser
1- Pour commencer, vous avez besoin de dire quelle type de donnée sera stocker dans votre array. 

Par exemple, vous pourriez mettre : 
- int
- double
- bool

2- Le nom de l'array dois être descriptif et unique, Vous devez attribuer les dimension de l'array entre crochet **`[]`** juste après le nom.
Vous devez déclarer un nouvel array 2d avec 3 lignes et 3 colonnes.

Par exemple : **`int my2DArray[3][3];`**

3- La valeur de l'array peut être défini à ça création en utilisant des accolades.

Par exemple : 

     int my2DArray[3][3] = { 
          { 0, 1, 2 },
          { 3, 4, 5 },
          { 6, 7, 8 }
        };
   > La valeur **[3]** [3] détermine le nombre d'array dans l'array 2d
   > Par exemple :
      `int array = { { 0, 1, 2 }, { 3, 4, 5 }, { 6, 7, 8 } }` serait aussi [3] [3] car il y a trois array dans l'array 2d et trois valeur par array individuel
      
4- Les valeurs de l'array peuvent aussi être défini individuellement par index.

Par exemple : 

    int my2DArray[3][3] = { 
      { 0, 1, 2 },
      { 3, 4, 5 },
      { 6, 7, 8 }
    };
	
	int variable = my2DArray[0][0]
    
    // La variable va être égal à 0 parce que la première valeur de la première
    // array dans l'array 2d va être 0

5- Pour lire les valeurs de l'array, inscrivez l'index d'un élément entre crochets.

Par exemple : **`int angle = turnAngles[1][0];`**

## Exemple
L'exemple présente une double array 2d appelé myAngles qui sera un array 2d pour les angles.

Par exemple :

     double myAngles[2][3] = {
      {45.5, 90.0, 88.2},
      {25.0, 75.5, 45.0}
    };