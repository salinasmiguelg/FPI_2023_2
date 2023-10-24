# Distancia de Hamming
---------------------------------------------

La distancia de Hamming es una pieza clave en la teoría de la información. Esta busca medir en cuántas componentes difieren dos palabras de la misma longitud. Lo que se traduce en el siguiente ejemplo:

![ham](./assets/hamming.png)

Construya una función en Python que reciba dos objetos iterables y retorne la distancia de Hamming entre ambas. En caso de que los objetos ingresados no coincidan en longitud debe retornar *False*.

## Consideraciones 
* Para este caso pueden generar un bloque principal para ayudarse en el desarrollo de la función solicitada, pero este no será considerado en los test de la plataforma, ósea se evaluará sólo la función solicitada por medio de los test. Para el correcto funcionamiento de esto debe procurar no cambiar el nombre de las funciones solicitadas.


## Ejemplos

### Ejemplo 1

Llamada:
```
hamming("100101001","100011001")
```
Retorno:
```
2
```


### Ejemplo 2

Llamada:
```
hamming("Hola mundo","Holi mondu")
```

Retorno:
```
3
```
