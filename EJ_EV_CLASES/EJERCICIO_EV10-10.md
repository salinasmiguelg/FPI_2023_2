![logo](./assets/logo_usach.png)

# Ejercicio Ev. 1

## Problema
Las bases numéricas son sistemas de representación utilizados para expresar números. En esencia, son conjuntos de símbolos o dígitos que se combinan de acuerdo con ciertas reglas para representar cantidades. Las bases numéricas más comunes son la base 10 (decimal) que utiliza los valores del 0 al 9, la base 2 (binaria) que utiliza unicamente los valores 0 y 1, la base 8 (octal) que utiliza los valores del 0 al 7 y la base 16 (hexadecimal) utiliza los valores 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E y F.

En el caso de las bases numéricas superiores a 10 los valores de los símbolos después del 9 corresponden a los siguientes:
A = 10
B = 11
C = 12
D = 13
E = 14
F = 15

##### Ejemplo:
El valor 16 de la base decimal se puede escribir de las siguientes formas según su base:
```
base 2: 10000 =>  1x2^4 + 0x2^3 + 0x2^2 + 0x2^1 + 0x2^0 = 16
base 3: 121 => 1x3^2 + 2x3^1 + 1x3^0 = 16
base 4: 100 => 1x4^2 + 0x4^1 + 0x4^0 = 16
base 5: 31 => 3x5^1 + 1x3^0 = 16
base 6: 24 => 2x6^1 + 4x6^0 = 16
base 7: 22 => 2x7^1 + 2x7^0 = 16
base 8: 20 => 2x8^1 + 0x8^0 = 16
base 9: 17 => 1x9^1 + 7x9^0 = 16
base 10: 16 => 1x10^1 + 6x10^0 = 16
base 11: 15 => 1x11^1 + 5x11^0 = 16
base 12: 14 => 1x12^1 + 4x12^0 = 16
base 13: 13 => 1x13^1 + 3x13^0 = 16
base 14: 12 => 1x14^1 + 2x14^0 = 16
base 15: 11 => 1x15^1 + 1x15^0 = 16
base 16: F => 16x16^0 = 16
```

Construya un programa que dado un número en una base numérica indique si ese número es o no pandigital en su base.

Un número pandigital es aquel que contiene todos los "dígitos" de su base 0 al 9 (o del 1 al 9) al menos una vez. Es decir, en un número pandigital, se incluyen todos los "dígitos" disponibles en la base numérica utilizada.

Por ejemplo, el número 1234567890 es un número pandigital en base 10, ya que incluye todos los dígitos del 0 al 9 exactamente una vez y el número 101 es un número pandigital en la base 2.

## Entrada
El ingreso de los datos debe ser por teclado, siguiendo el siguiente formato

#### Ejemplo Entrada
`'5430357518 9`'

el primero es el número `'5430357518` que se encuentra en base `'9`', ambos se encuentran separados por un espacios. 

## Salida

Debe mostrar por cada valor el resultado en el mismo orden con el formato número_original, seguido de un espacio, luego la base_original, un espacio seguido de la frase `'es pandigital`' o `'no es pandigital`' según corresponda.

```
5430357518 9 no es pandigital
```

## Restricciones

* Considere que las entradas siempre serán números de bases entre la 2 y la 16.



## Ejemplos

### Ejemplo 1

Entrada:
```
032221440404003 5
```
Salida:
```
032221440404003 5 es pandigital
```

### Ejemplo 2

Entrada:
```
522454001545243 7

```

Salida:
```
522454001545243 7 no es pandigital
```
