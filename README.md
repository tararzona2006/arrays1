# arrays1


- Un array es una zona de almacenamiento continuo, donde se pueden introducir varios valores cada uno de ellos ubicados por la posicion que ocupa en el array
- Tambien son llamados como arreglos o vectores, y cuando son de dos dimensiones son llamados matrices.
- Los arrays nos brindan la capacidad de almacenar una coleccion de elementos y acceder a ellos de manera indivudual.
-Cada elemento se identifica mediante su posicion en el array denominada indice y estos **indices** son siempre secuenciales
- En javascript son altamente flexibles en terminos de los diferentes tipos de datos que podemos almacenar en cada posicion del array

## Crear un array 

1. Declarando un array con elementos en linea

```Javascript
let miArray = [1,2,3]:
console.log(miArray);
```

2. Declarando un array con la sintaxis **new Array()**

```Javascript
let miArray = new Array(1,2,3);
console.log(miArray);
```

3. Declarando un array con un tamaño especifico utilizando la sintaxis **new Array** y asignando valores despues:

```Javascript
let miArray = new Array(3);
miArray[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
```

4. Declarando un array con diferentes tipos de datos

```Javascript
let miArray4 = [1, "dos", tres, {nombre: "pedro", edad:30}];
console.log(miArray4);
```

## Accediendo a la información de un array
- Devuelve la cantidad de elementos del array.

### Operador [pos]
-Permite acceder para leer o modificar el elemento pos del array.

### Método at(pos)
- Devuelve el elemento de la posición pos. El parámetro admite valores negativos, lo que significa que empieza a contar por el dinal del array.

```Javascript
const letters = ["A", "B", "C"];
console.log(letters.leight);
console.log(letters[2]);
console.log(letters[5]);
```

## Añadir o eliminar elementos
- push(ele1, ele2); añade uno o varios elementos al final del array. Devuelve el tamaño del array.

```Javascript
let miArray = [1, 2, 3];
miArray.push(4); // Agrega el elemento 4 al final del array
console.log(miArray);
```

- pop(): devuelve el ultimo elemento del array y lo elimina
```Javascript
let miArray = [1, 2, 3];
miArray.pop(); // Elimina el último elemento del array
console.log(miArray);
```
- unshift(ele1, ele2): añade uno o varios elementos al inicio, devolviendo el tamaño del array después de añadidos
```Javascript
let miArray = [1, 2, 3];
miArray.unshift(0); // agrega el elemento 0 al inicio del array
console.log(miArray);
```

- shift(): devuelve el primer elemento del array y lo elimina
```Javascript
let miArray = [1, 2, 3];
miArray.shift(0); // elimina el primer elemento del array
console.log(miArray);
```

- concat(ele1, ele2): concatena dos arrays
```Javascript
let miArray = [1, 2, 3];
let miArray = [4, 5];
let nuevoArray = miArray.concat(miOtroArray);
console.log(miArray);
console.log(miOtroArray);
console.log(minuevoArray);
```

- split(separador): a partir de una cadena, crear un array dividiendo dicha cadena en elementos delimitador por separador
```Javascript
let miString = "Hola, ¿cómo estás?";
let miArray = miString.split(" ");
console.log(miArray);
```

- join(separador): a partir
```Javascript
let miArray = ["Hola,", "¿cómo", "estás?"];
let miString = miArray.join(" ");
console.log(miString);
```