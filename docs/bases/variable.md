
# Les variables


Les variables en C++ sont un peu comme les atomes dans une molécule: **c'est la base de tous programmes**. Elles peuvent stocker différente information, ça peut être un chiffre, un chiffre décimal, une valeur vrai ou fausse et beaucoup d'autres chose.

## Les types de variables 😎

comme dit précédemment, il existe plusieurs **types** de variable. En voici quelque une:

|Type  | Explication|
|--|--|
|`bool`  | une variable vrai ou fausse |
|`int`   |  un nombre entier sans décimale  |
|`double`| un nombre avec des décimales avec une précisions de **15 		nombres** après la virgules  |
|`float`| un nombre avec des décimales avec une précisions de **7 nombres** après la virgules  |
|`char[]`   |  une variable qui continent un mot ou une phrase  |


## Créer une variable ❓

pour créer une variable il faut simplement écrire le type de variable, écrire le nom de la variable et écrire à quoi elle est égal :

    bool variable = true;
   
  **À la fin de la variable, vous voyez probablement le **";"**, en C++ la plupart des lignes de codes en prenne un à la fin.** 

## Les math avec les variables 🔢

En C++, il est possible de faire des opération avec les variables. Par exemple:

Nous pouvons créer une variable du type int en additionnant 2 nombres

    int variable = 1 + 1; // va être égal à 2

 Il est aussi possible de faire une variable en additionnant  deux autres variables ensemble

    int variable = 3;
    int variable2 = 5;
    int variable3 = variable + variable2; // va être égal à 8

### Les opérateurs de base ➕

En C++, il y a différents types d'opérateurs qui vont exécuter des opérations mathématiques. **En résumé, c'est les plus, moins, diviser, multiplier.** 

|Opérateur| Explication |
|--|--|
| `+` | Une addition |
| `-` | Une soustraction|
| `*` | Une multiplication|
| `%` | Une opération de modulo|

L'opérateur **%** est en fait le restant d'une division. Par exemple,

    int x = 11 % 3;
donnerait une valeur de **2** parce que dans le nombre 11, il rentre trois fois le chiffre 3 et le ce qu'il reste à la fin est le chiffre 2. En résumé, c'est le restant de la division du nombre.


