# Tableaux
## Définition de tableaux et accès aux valeurs
Javascript propose la possibilité de stocker des tableaux de variables. Ils fonctionnent également comme des listes (list), des piles(stack) ou des files(queue).

Ci-dessous les différentes manières d'instancier des tableaux : 
```javascript
var array1 = [1,2,3,4];
var sameArrayAs1 = new Array(1,2,3,4);
```
Comme dans d'autres langages, en javascript les tableaux supportent l'accès à un élément du tableau à l'aide des crochets:
```javascript
var pouet = array1[2];
```

En Javascript les tableaux sont "sparse". Ca veut dire que nous pouvons définir la valeur d'une position sans avoir au préalable défini les positions précédentes.
```javascript
var array = []
array[2] = "pouet";
console.log (array);        //qu'est-ce qui s'affiche dans la console?
```

En javascript, chaque élément d'un tableau peut être d'un type différent. Il est tout à fait possible d'écrir : 
```javascript
var truc = ["machin", 3, true];
```

## Manipulation de tableaux
Comme les tableaux fonctionnent aussi comme des listes(list), piles(stack) ou 
files(queue), il existe beaucoup de fonctions permettant de manipuler les tableaux.
### push
La function push sur un tableau permet d'insérer un élément à la fin d'un tableau : 
```javascript
var myArray = [];
myArray.push(1);
myArray.push(3);
myArray.push(42);
```
### pop
Pour utiliser le tableau comme une pile (stack) nous pouvons utiliser pop sur le tableau pour retirer le dernier élément qui a été insérer dans le tableau : 
```javascript
var myArray = [];
myArray.push(1);
myArray.push(4);
myArray.push(56);
console.log(myArray);       //affiche [1,4,56]
console.log(myArray.pop()); //affiche 56
console.log(myArray);       //affiche [1,4]
```
### shift et unshift
Pour utiliser le tableau comme une file (queue) nous pouvons utiliser shift et unshift.

shift va supprimer les valeurs du tableau dans l'ordre exact dans lesquelles elles ont été insérées.

unshift va insérer une valeur au début du tableau
```javascript
var myArray = [];
myArray.push(1);
myArray.push(4);
myArray.push(56);
console.log(myArray);           //affiche [1,4,56]
console.log(myArray.shift());   //affiche 1
console.log(myArray);           //affiche [4,56]
myArray.unshift(0);
console.log(myArray);           //affiche [0,4,56]
```