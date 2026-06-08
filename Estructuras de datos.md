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
