# Variables et types
![alt text](https://static.passeportsante.net/i41686-canard.jpg "Canard")

>"Si je vois un oiseau qui vole comme un canard, cancane comme un canard, et nage comme un canard, alors j'appelle cet oiseau un canard" James Whitcomb Riley

Comme à peu près tous les langages dynamiques, Javascript utilise du typage "canard" (ou duck typing).

Qu'est-ce que le typage "canard"? Un exemple vaut mieux que de longs discours : 
```javascript
var a = 42;             //a sera de type number
var b = "canard";       //b sera de type string
var c = true;           //c sera de type boolean
var d = [];             //d sera un tableau
var e = {};             //e sera un objet
```
## Le cas de "undefined" et "null" :
![alt text](https://i.redd.it/w3a17dx4vq401.png "Undefined vs null")
Quand une variable est utilisée avant que n'on lui affecte une valeur, sa valeur vaut undefined.
En revanche, si une variable est explicitement vide, il faut utiliser null.
```javascript
var a;
console.log(a);         //affiche undefined dans la console
var b = null;
console.log(b);         //affiche null dans la console
```
