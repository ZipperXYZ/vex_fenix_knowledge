# La programmation orienté objet

La programmation orienté objet (OOP) est un type de programmation. Il est utile pour créer plusieurs objet qui doivent être tous différents, mais tous avoir les même fonction et les même variable. 

Par exemple, nous pourrions faire un jeu vidéo de course avec des voitures. Chaque voiture serait tous fabriquer, dans le code, sur la même structure. Il aurait, par exemple, les même fonction et les même variable, mais il pourrait tous avoir des valeur différente puisqu'il serait considérer comme des objets différents. Une voiture1 pourrais avoir une vitesse max de 30 kmh alors que la voiture2 pourrais avoir une vitesse max de 200 kmh. 

## Comment créer ces objets?

Dans le C++, pour créer des objet, nous utilisons se que nous appelons **des classes**. Les classes sont un peu le "Template" pour un objet. Par exemple, Une classe de voiture pourrais avoir plusieurs objet comme une ferrari, une volvo, une honda et d'autres voiture qui aurait tous des propriétés différentes.

## Comment créer des classes?

La syntaxe pour créer une classe est très simple: 

    class NomClasse { // la classe
	    public: // les spécification d'accès (à voir plus tard) 
		    int Nombre; // les variables (un nombre, par exemple)
    };

le type d'une classe en C++ est appelé **`class`** 

## Créer un objet

Il est très simple de créer un objet à partir d'une classe.

    class NomClasse {
	    public:
		    int Nombre;
    };
	// nous allons utiliser la classe de l'exemple précédent comme exemple

	int main() {
		NomClasse MonObjet; // nous créons un objet qui va s'appeller MonObjet
		NomClasse MonObjet2; // un deuxième objet
		
		MonObjet.Nombre = 13; // ici, dans cette objet, la variable Nombre va
		// va être égal à 13
		
		MonObjet2.Nombre = 6; // mais ici, dans cette objet la variable va être 			
		// égal à 6 car c'est un autre objet et pas le même
		
	}


Voici un autre exemple dans un contexte plus réaliste: 

    class Voiture {
	    public:
		    double Vitesse;
		    char[] Marque;
    };
	// une classe de voiture simple

	int main() {
		Voiture Ferrari; // nous créons une Ferrari
		Voiture Volvo; // ici une volvo
		
		// ici, nous définissons les valeurs de la Ferarri
		Ferrari.Vitesse = 200.46;
		Ferrari.Marque = "Ferrari";

		// ici, celle de la volvo
		Volvo.Vitesse = 142.2;
		Volvo.Marque = "Volvo";
		
	}

## Créer des méthodes dans une classe (fonction)

Une méthode est une fonction, mais dans une classe. Par exemple, une classe de voiture pourrait avoir une fonction pour faire démarrer le moteur. 

Voici un exemple en code:

    class Voiture {
	    public:
		    double Vitesse;
		    char[] Marque;
			
			void Demarrer() {
				// le code pour démarrer 
			}
    };
	// une classe de voiture simple

	int main() {
		Voiture Ferrari; 
		
		Ferrari.Vitesse = 200.46;
		Ferrari.Marque = "Ferrari";

		Ferrari.Demarrer(); 
		// nous appelons la fonction pour démarrer le moteur ici
	}

Dans l'exemple, la classe voiture a une fonction **`Demarrer`** qui est utile pour démarrer le moteur de la voiture.

Il y a aussi possible de déclarer la méthode a l'extérieur de la classe (utile pour des gros programmes)

Voici comment faire: 

    class Voiture {
	    public:
		    double Vitesse;
		    char[] Marque;
			
			void Demarrer()
    };

	void Voiture::Demarrer(){
		// faire quelque chose		
	}

Comme vous pouvez le voir, on utilise le "scope resolution `::` operator" (de l'anglais) pour définir la fonction à l'extérieur. 

**Comme des fonctions régulières, vous pouvez aussi passer des paramètres:**

    class Voiture {
	    public:
		    double Vitesse;
		    char[] Marque;
			
			void setSpeed(double Speed)
    };

	void Voiture::setSpeed(double Speed){
		Vitesse = Speed;		
	}

	int main() {
		Voiture Ferrari; 
		
		Ferrari.Vitesse = 200.46;
		Ferrari.Marque = "Ferrari";

		Ferrari.setSpeed(145.4)
		// nous appelons la fonction pour changer la vitesse ici
	}

## Le constructeur d'une classe

Le constructeur d'une classe est une méthode spéciale qui est appelé quand qu'un objet est créé. C'est un peu comme la fonction qui initialise les composantes importantes de la méthode.

Pour créer la méthode de constructeur, il faut écrire le nom de la classe **SANS AUCUN TYPE DEVANT** et après cela la déclarer avec des **`( )`**.

Voici les règles à suivre:

 - Pas de type devant 
 - Aucun retour de variable 
 - Il doit être déclarer `public` (à voir plus tard)

En voici un  exemple:

    class Voiture {
	    public:
		    double Vitesse;
		    char[] Marque;

			Voiture(){
				// la fonction qui est appeler quand que nous créons un objet
			}
    };
    
	int main() {
		Voiture Ferrari; // le constructeur serait appeler à ce moment là
		
		Ferrari.Vitesse = 200.46;
		Ferrari.Marque = "Ferrari";
		
	}

**Comme méthodes, il est aussi possible de les définir à l'extérieur de la classe et d'y passer des paramètres**

Voici un exemple: 

	class Voiture {
	    public:
		    double VitesseMax;
		    char[] Marque;

			Voiture(){
				// la fonction qui est appeler quand que nous créons un objet
			}
    };
	
	Voiture::Voiture(char[] Sorte, double MaxSpeed){
	
		double VitesseMax = MaxSpeed;
		char[] Marque = Sorte;
		
	}
	
	
    
	int main() {
		Voiture Ferrari("Ferrari",200.46);
		// nous déclarons l'objet Ferrari en lui donnant des variable en 
		// paramètre. 
		
		// Ferrari.Vitesse = 200.46 puisque le constructeur égalise 
		// le paramètre MaxSpeed à la variable VitesseMax
		//  Ferrari.Marque = "Ferrari";
		
	}


## Spécifier l'accès des variables

Dans le C++, il est possible que vous vouliez qu'une variable soit seulement accessible par la fonction. Cela est très utile pour la sécurité du programme et des fonctions

Si nous avions une classe de voiture et que nous ne voudrions pas que des hacker gèrent les variables de la classe comme il voudrait, une protection est nécessaire. 

Il existe plusieurs type de spécificateurs d'accès:

|Spécificateur| explication |
|--|--|
| `public` | les membres de la classe peuvent être accédés à l'extérieur de la classe |
| `private` | les membres ne peuvent pas être accédées à l'extérieur de la classe
| `protected` | les membres peuvent seulement être accédées par des fonction hérité (à voir plus tard)

Voici un exemple de classe avec des accès protégés

    class  MaClasse {  
		public:  // Spécificateurs de l'accès publique
			int x; // Publique
		private:  // Spécificateurs de l'accès privé
			int y; // Privé  
	};  
  
	int main() {  
		MaClasse monObj;  
		monObj.x = 25; // nous pouvons y accéder
		monObj.y = 50; // ERREUR: nous ne pouvons pas y accéder
	}

De base, en C++, dans les classes, les variable sont privée. Il est donc pas nécessaire définir l'accès de la variable si elle est privée

    class  MaClasse {  
    
	    int x; // privé

	    public: 
		    int y; // publique
		    
	};  

 