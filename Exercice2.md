#420-A6W-SW : Exercices 2


## La carte

La carte est décrite par un tableau en deux dimension.

```
\\ La carte du monde
Structure Carte:
   int dim_x // La dimension en x de la carte
   int dim_y // La dimension en y de la carte
   string[,] tiles // Un tableau 2D de string.
FinStructure
```

La fonction `CreationCarte(dim_x, dim_y)` permet de créer une nouvelle carte.

Ainsi, si on veut attribuer une valeur à un carreau de la carte, par exemple à l'emplacement [2, 3].  

```
Carte carte <- CreationCarte(10, 12)

carte.tiles[2, 3] <- "Arbre"
carte.tiles[2, 4] <- "Eau"
```

```
\\ Creation d'une nouvelle carte
\\ Paramètres:
\\ 	int x: La dimension en x
\\      int y: La dimension en y
\\ Retourne: Carte
\\ 	Retourne une nouvelle carte de dimension x par y où
\\      toute les casses contiennent le string "sol"
Fonction CreationCarte(int x, int y): Carte
   // Déclaration d'une variable de type c
   Carte c 
   
   // Assigner x à la dimension en x de la carte
   c.dim_x <- x

   // Assigner y à la dimension en y de la carte
   c.dim_y <- y

   // Création d'un tableau de string de dimension [x,y]
   c.tiles <- string[x, y]

   // Mettre dans chaque entrée du tableau, la valeur "sol"
   Pour i de 0 à x-1 Faire
      Pour j de 0 à y-1 Faire
         c.tiles[i, j] <- "sol"
      FinPour
   FinPour

   // Retourner la nouvelle carte
   Retourne c
FinFonction
```

## Fonction que nous allons considérer comme existantes et fonctionnelles.

### Affichage

```
\\ Afficher le monde, le joueurs et les ennemis à l'écran
\\ Paramètres:
\\      Map m: La carte du monde
\\      Joueur j: Le joueur
\\      Ennemis[] e: La liste des énnemis
Procedure AfficherMonde(Map m, Joueur j, Ennemis[] e)
```

```
\\ Affiche un message au joueur
\\ Paramètres:
\\ 	string message: Message à afficher
Procedure AfficherMessage(string message)
```

```
\\ Obtenir un nombre aléatoire
\\ Paramètres:
\\ 	int a: valeur minimale
\\      int b: valeur maximale
\\ Retourne: int
\\ 	Retourne une valeur aléatoire entre a et b inclusivement
Fonction Random(int a, int b): int
```

