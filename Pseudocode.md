# Norme pseudcode pour 420-A6W

Dans le cadre du cours _420-A6W-SW: Programmation d'algorithme_, nous utilisons un langage en pseudocode pour écrire nos algorithmes. 
L'utilisation d'un pseudocode nous permet de nous abstraire des contraintes d'un langage spécifique et de nous concentrer sur la logique et la création des algorithmes.

## La gestion de la mémoire
Les

### Les variables

### Les types

### Les tableaux

### Les Structures


## Les structures de contrôle

### La conditionnelle

```C
Si <condition> Alors
   // Ce bloc est exécuté si <condition> est vrai
Sinon Si <condition2> Alors
   // Ce bloc est exécuté si <condition> est faux
   // et <condition2> est vrai
Sinon Si <conditions3> Alors
   // Ce bloc est exécuté si <condition> est faux
   // et <condition2> est faux
   // et <condition3> est vrai
... (Autant de bloc Sinon Si que nécessaire)
Sinon
   // Ce bloc est exécuté si toute les <conditionN> sont fausses
FinSi
```


### L'itération

### La boucle conditionnelle

## Les unités organisationnelles 

Tout algorithme pourrait théoriquement être écrit comme une longue suite d'instructions.
En pratique, cette approche rend rapidement incompréhensible l'algorithme et très difficile à concevoir.
On divise donc l'algorithme en une série de plus petite unité qui rend son écriture et sa compréhension beaucoup plus facile.

Cette approche est souvent nommée _divisé pour régner_ et est méthode extrêmement puissante pour être en mesure d'écrire des algorithmes et des programmes complexes.

### Fonctions et procédures

Les fonctions et les procédures sont les blocs de base qui permettrons de structurer en unités plus simple notre code.

#### Les fonctions

Pseudocode
```
Fonction Nom_de_la_fonction(type param1, type param2, ...)
   code de la fonction
FinFonction
```

#### La fonction `Main`
Un programme comporte généralement un grand nombre de fonctions, déclarations et fichiers. 
Lorsqu'on demande à l'ordinateur d'exécuter un programme, il doit savoir où commencer l'exécution.
Différente approche existe pour résoudreLa fonction `Main` 

#### Procédure

### Fichier
