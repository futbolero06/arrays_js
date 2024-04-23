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

## Accediendo a la información de un Array 

### Propiedad length
- Devuelve la cantidad de elementos del Array

### Operador [pos]
- Perite acceder para leer o modificar el elemento pos del array

### Método at(pos)
- Devuelve el elemento de la posición pos. El parámetro admite valores negativos, lo que significa que empiezan a contar por el final del array.

```Javascript
const letters = ["A","B","C"];
console.log(letters.length);
console.log(letters[2]);
console.log(letters[5]);
```

## Añadir o eliminar elementos
- push(ele1, ele2): añade uno o varios elementos al final de array. Este método devuelve el tamaño del array.

```Javascript
let miArry = [1,2,3];
miAray.push(4); // Agrega el elemtno 4 al final  del array
console.log(miArray);
```

-pop():devuelve el ultimo elemento del array y lo elimina

```Javascript
let miArry = [1,2,3];
miAray.pop(); // Elimina el último elemento del array
console.log(miArray);
```

- unshift(ele1, ele2): añade uno o varios elementos al inicio devolvieldo el tamaño del array despues de añadidos

```Javascript
let miArry = [1,2,3];
miAray.unshift(0); // agrega el elemento cero al inicio del array
console.log(miArray);
```

- shift(): devuelve el primer elemento del array y lo elimina 

```Javascript
let miArry = [1,2,3];
miAray.unshift(0); // eliminar el primer elemento del array
console.log(miArray);
```

- concat(ele1, ele2): concatenaa dos arrays

```Javascript
let miArry = [1,2,3];7
let miOtroArray = [4,5];
let nuevoArray = miArray.concat(miOtroArray)
console.log(miArray);
console.log(miOtroArray);
console.log(nuevoArray);
```

- split(separado): a partir de una cadena,crear un array y dividiendo dicha cadena en elementos delimitados por separador

```Javascript
let miString = "Hola, ¿Cómo estás?";
let miArray = miString.split(" ");
console.log(miArray);
```

- join(separador): a partir de un array, crea una cadena separando cada elemento con el separador

```Javascript
let miArray = ["Hola,", "¿cómo", "estás?];
let miString = miArray.join(" ");
console.log(miString);
```

## Busqueda de elementos en un array
- includes(elemento): devuelve true o false si el elemento existe o no dentro del array
- indexOf(elemento): devuelve la posición de la primera aparición del elemento. Si no existe, devuelve -1.
- lastINdexOf(elemento:) devuelve la posición de la ultima aparición del elemento. Si no existe, devuelve -1.

## Modificar el array o crear fragmentos
-slice(inicio, fin): devulve un array con los elementos desde la posición inicio hasta la posición fin, ambos excluidos.

## Ordenar elementos de un array
- reverse(): invierte el orden de los elementos del array
- sort(): ordena el array alfabeticamente
- sort(criterio): ordena el array con el criterio determnado por la función criterio

## Borrar elementos de un array 
- Se puede borrar el contenido de un elemento de un array poniendo su valor a null o asignando una cadena vacía " ".
- Para eliminar completamente unelemento del array se utiliza el operador delete.

## Recorrido de un array
1. Recorre con un bucle clásico pasando por todos los elementos.

``` Javascript
var dias = ["lunes", "martes", "miércoles", "jueves", "viernes", "sabado", "domingo" ];
for (i=0,i<dias.length;i++)
{
    console.log(dias[i]);
}
```
2. Recorre con un while pasando por todos los elementos.

``` Javascript
var dias = ["lunes", "martes", "miércoles", "jueves", "viernes", "sabado", "domingo" ];
var i = 0;
while(i<dias.length)
{
    console.log(dias[i]);
    i++;
}
```
3. Usando la sentencia for..in.

``` Javascript
var dias = ["lunes", "martes", "miércoles", "jueves", "viernes", "sabado", "domingo" ];
for (let index in dias)
{
    console.log(dias[index]);
}
```

## Arrays multidimensionales

``` Javascript
const matrix = [
    [1,2,3],
    [4,5,6],
    [7,8,9],
];
```

- Recorrer una matriz utilizando bucles anidados

``` Js
var dias = ["lunes", "martes", "miércoles", "jueves", "viernes", "sabado", "domingo" ];
for (i=0,i<matriz.length;i++)
{
    for (let j=0;matriz[i].lenght; j++)
    {
        console.log(matriz[i][j]);
    }
}

```


# Ejercicios

1. Dada una lista de números separados por coma, calcular la suma,el mayor, el menor y la media de todos.

2. Introduciry dos cadenas con elementos separados por coma, y con un botón concatenar las dos cadenas y mostrarlas en pantalla.

3.  Introducir uno a uno los elementos en un array a través de un botón. Con otro botón se va eliminado el último elemento. Siempre que se pulse alguno de los botones se debe mostrar el contenido del array.

4. Introducir un conjunto de números separados por comas. Cuando se pulsa el botón "Pares" cargar una tabla con los números introducidos y luego crear otra que solo incluya los números pares y mostrarla.