## Estructuras de Datos en JavaScript
Las estructuras de datos son formas de organizar información en memoria para poder almacenarla, acceder a ella y modificarla de manera eficiente.

### Algunas estructuras comunes son:

1. Arreglos (Arrays)
2. Listas
3. Pilas (Stacks)
4. Colas (Queues)
5. Diccionarios (Objetos)
6. Árboles
7. Grafos

La estructura adecuada depende del problema que se desea resolver, escojer la estructura correcta aegura un mejor rendimiento de nuestro programa

## Arreglos (Arrays)
Es una colección de elementos almacenados en posiciones numeradas llamadas índices.
* Las maquinas cuentan desde 0 
` let frutas = ["manzana", "uva", "pera"]; `

| Indice | Valor |
|----------|----------|
| 0   | manzana   |
| 1    | uva   |
| 2    | pera   |

### Acceder a un elementos
` console.log(frutas[0]);`
Nos dará la salida: manzana

### Modificar un indice 
`frutas[1] = "banana";`

`console.log(frutas);`

Nos dara la siguiente salida: `["manzana", "banana", "pera"]`

### longitud de un arreglo
Se obtiene con :
`console.log(frutas.length);`

Nos da la salida `3` 


### Recorrer un arreglo
Se puede hacer recorriendo indice por indice

```javascript
for(let i = 0; i < frutas.length; i++){
    console.log(frutas[i]);
}
```
Tambien se puede hacer elemento por elemento

```javascript
for(let fruta of frutas){
    console.log(fruta);
}
```

### Agregar elementos
Se usa el metodo push ()
```javascript
frutas.push("sandia");

console.log(frutas);
```
Nos dara:
```javascript
["manzana", "uva", "pera", "sandia"]
```

### Eliminar elementos
se usa el metodo pop(), este elimina el ultimo elemento
Nos dara:
```javascript
frutas.pop();
```

El metodo shift() elimina el primer elemento.
```javascript
frutas.shift();
```

### Metodo map()
Sirve para crear un nuevo arreglo transformando cada elemento.
```javascript
let nums = [1,2,3,4,5];

let dobles = nums.map(num => num * 2);

console.log(dobles);
```

Esto nos da la salida:
```javascript
[2,4,6,8,10]
```

| Valor Original | Resultado |
|----------|----------|
| 1   | 2   |
| 2    | 4   |
| 3    | 6   |
| 4    | 8   |
| 5    | 10   |


### Método filter()
Sirve para seleccionar elementos que cumplan una condición.
```javascript
let nums = [1,2,3,4,5,6];

let pares = nums.filter(num => num % 2 == 0);

console.log(pares);
```

Nos da la salida:
```javascript
[2,4,6]
```
### Diferencia entre map() y filter()
Map

Transforma todos los elementos.map

```javascript
// este [2,4,6] pasa a este [2,4,6]
```
Filter
Selecciona ciertos elementos

```javascript
// este [1,2,3,4,5,6] pasa a este [2,4,6]
```

### Ejercicios Básicos
1. Crea un arreglo con 5 nombres y muéstralos en pantalla.
2. Muestra el primer y último elemento del arreglo.
3. Crea un arreglo con tres colores y agrega dos más usando push().
4. Crea un arreglo con cinco números y elimina el primero usando shift().
5. Muestra todos los elementos usando un ciclo for.
6. Convertir ma mayúsculas ["juan","ana","pedro"]
7. Filtrar pares [1,2,3,4,5,6,7,8]
