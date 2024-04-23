# Arrays

- Un Array es una zona de almacenamiento continuo, donde se puedenintroduzir varios valores, cada uno de ellos ubicados por la posicición ue ocupa en el array.
- También son denominados arreglos o vectores, y cuando son de dos dimensiones son llamados matrices.
- Los arrays nos brindran la capacidad de almacenar una colección de elementos y acceder a ellos de manera individual
- Cada elemento se identifica mediante su posición en el array, denominada indice **indice** y estos indices so siempre secuenciales.
- En Javascript son altamente flexibles en términos de los diferentes tipos de datos que podemos almacenar en cada posición del array 

## Crear un array 

1. Declarando una rray con elementos en línea

```Javascript
let miArray = new Array(1,2,3);
console.log(miArray);
```
2. Declarando un array con la sintaxis **new Array()**

```Javascript

let miArray = new Array(1,2,3);
console.log(miArray);
```

3. Declarando un array con un tamaño específico  utilizando la sintaxis **new Array** y asignando valores después:

```Javascript

let miArray = new Array(3);
miArray[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
```
4. Declarando un array con elementos de diferentes tipos de datos 

```Javascript

let miArray4 = [1,"dos", true,{nombre:"Juan", edad;30}];
console.log(miArray4);
```