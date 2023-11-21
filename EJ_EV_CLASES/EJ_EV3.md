# **PROBLEMA**

Se desea poder recopilar la asistencia de  algunos cursos extraprogramáticos. Para esto se cuenta con un archivo que trae la lista de los estudiantes y la asistencia a cada clase que se realizó. Se busca que con esta información se entregue el procentaje de asistencia de cada estudiante en base al total de clases que hay en el archivo.

Se le solicita crear una función llamada "`evaluar`" que reciba un string que es el nombre del archivo de entrada con las información del curso. La función debe generar el archivo "`resultado.txt`" con la asistencia de cada estudiante.


## Consideraciones

* Puede y debe probar su función con un bloque principal adecuado, sin embargo, cuando evalúe los test cases, no use ni input ni print.

## Entrada

La entrada de la función es un string, correspondiente al nombre del archivo con la información del curso (el nombre del archivo incluye la extensión del archivo):
```[python]
def evaluar(nombre_archivo):
  <código_de_la_función_evaluar>
```
El archivo, en las primeras líneas, tiene los nombres de los estudiantes inscritos en el curso. Luego viene la información de los estudiantes que asistieron a cada clase, donde cada clase comienza con la palabra "`Clase`" y el número de la clase de forma correlativa, seguido de los estudiantes que asistieron.

Ejemplo del archivo con la asistencia.
```
Melloney Shelhamer
Dahlia Bacone
Wynne Campa
Leyla Kinzle
Venus Griffth
Clase 1
Leyla Kinzle
Clase 2
Dahlia Bacone
Wynne Campa
Clase 3
Dahlia Bacone
Leyla Kinzle
Clase 4
Melloney Shelhamer
Clase 5
Venus Griffth
Wynne Campa
Clase 6
Melloney Shelhamer
Leyla Kinzle
Clase 7
Venus Griffth
Clase 8
Wynne Campa
Leyla Kinzle
```


## Salida

Debe generar el archivo "`resultado.txt`". Este debe tener a un estudiante por línea junto con un signo de dos puntos y un espacio, "`: `". Luego el porcentaje de asistencia con un decimal de precisión y finalmente el signo de procentaje "`%`".

Ejemplo del archivo resultado.txt
```
Melloney Shelhamer: 25.0%
Dahlia Bacone: 25.0%
Wynne Campa: 37.5%
Leyla Kinzle: 50.0%
Venus Griffth: 25.0%
```


## Ejemplos
A continuación se muestran ejemplos del archivo de entrada con los casos y su salida.
### Ejemplo 1

Entrada
```
Zulema Oas
Mathilde Louil
Nerte Abolt
Cecilia Daskam
Doloritas Hatley
Sidonia Minvielle
Nerte Mutton
Kelcy Oliphant
Cleo Ruben
Clovis Wagganer
Stephenie Boatfield
Ladonna Navas
Kiley Scherschligt
Wilhelmina Tobolski
Emili Cockriel
Clase 1
Zulema Oas
Kelcy Oliphant
Nerte Abolt
Wilhelmina Tobolski
Mathilde Louil
Clovis Wagganer
Sidonia Minvielle
Doloritas Hatley
Emili Cockriel
Stephenie Boatfield
Kiley Scherschligt
Clase 2
Stephenie Boatfield
Clovis Wagganer
Doloritas Hatley
Kelcy Oliphant
Nerte Abolt
Cecilia Daskam
Cleo Ruben
Emili Cockriel
Ladonna Navas
Wilhelmina Tobolski
Nerte Mutton
Zulema Oas
Clase 3
Zulema Oas
Stephenie Boatfield
Ladonna Navas
Wilhelmina Tobolski
Cecilia Daskam
Cleo Ruben
Mathilde Louil
Kelcy Oliphant
Kiley Scherschligt
Sidonia Minvielle
Nerte Abolt
Clovis Wagganer
Clase 4
Cecilia Daskam
Wilhelmina Tobolski
Nerte Abolt
Nerte Mutton
Cleo Ruben
Clovis Wagganer
Ladonna Navas
Sidonia Minvielle
Mathilde Louil
Kelcy Oliphant
Kiley Scherschligt
Zulema Oas
Stephenie Boatfield
Clase 5
Zulema Oas
Mathilde Louil
Ladonna Navas
Wilhelmina Tobolski
Cecilia Daskam
Cleo Ruben
Nerte Mutton
Doloritas Hatley
Kiley Scherschligt
Emili Cockriel
Kelcy Oliphant
Clase 6
Ladonna Navas
Kelcy Oliphant
Zulema Oas
Wilhelmina Tobolski
Nerte Abolt
Emili Cockriel
Doloritas Hatley
Kiley Scherschligt
Nerte Mutton
Cecilia Daskam
Clovis Wagganer
```
Salida:

```
Zulema Oas: 100.0%
Mathilde Louil: 66.7%
Nerte Abolt: 83.3%
Cecilia Daskam: 83.3%
Doloritas Hatley: 66.7%
Sidonia Minvielle: 50.0%
Nerte Mutton: 66.7%
Kelcy Oliphant: 100.0%
Cleo Ruben: 66.7%
Clovis Wagganer: 83.3%
Stephenie Boatfield: 66.7%
Ladonna Navas: 83.3%
Kiley Scherschligt: 83.3%
Wilhelmina Tobolski: 100.0%
Emili Cockriel: 66.7%
```

# Ejemplo 2
Entrada
```
Rhea Mortel
Vicky Wojtowicz
Winna Cutbirth
Francine Zomberg
Cesya Darling
Lynsey Pecos
Lauryn Decristofaro
Margalit Ancheta
Lyda Nola
Donielle Galaska
Clase 1
Rhea Mortel
Margalit Ancheta
Francine Zomberg
Lauryn Decristofaro
Lyda Nola
Winna Cutbirth
Clase 2
Margalit Ancheta
Rhea Mortel
Lauryn Decristofaro
Cesya Darling
Vicky Wojtowicz
Lyda Nola
Lynsey Pecos
Clase 3
Francine Zomberg
Cesya Darling
Lyda Nola
Margalit Ancheta
Winna Cutbirth
Lynsey Pecos
Donielle Galaska
Rhea Mortel
Clase 4
Donielle Galaska
Lynsey Pecos
Vicky Wojtowicz
Margalit Ancheta
Lauryn Decristofaro
Lyda Nola
Rhea Mortel
Cesya Darling
Clase 5
Cesya Darling
Rhea Mortel
Lynsey Pecos
Winna Cutbirth
Vicky Wojtowicz
Lyda Nola
Lauryn Decristofaro
Margalit Ancheta
Clase 6
Lynsey Pecos
Margalit Ancheta
Rhea Mortel
Winna Cutbirth
Vicky Wojtowicz
Donielle Galaska
Cesya Darling
Clase 7
Lauryn Decristofaro
Margalit Ancheta
Lynsey Pecos
Cesya Darling
Donielle Galaska
Rhea Mortel
Clase 8
Winna Cutbirth
Cesya Darling
Vicky Wojtowicz
Rhea Mortel
Margalit Ancheta
Donielle Galaska
Lynsey Pecos
Lauryn Decristofaro
Clase 9
Lynsey Pecos
Winna Cutbirth
Rhea Mortel
Cesya Darling
Margalit Ancheta
Donielle Galaska
```

Salida
```
Rhea Mortel: 100.0%
Vicky Wojtowicz: 55.6%
Winna Cutbirth: 66.7%
Francine Zomberg: 22.2%
Cesya Darling: 88.9%
Lynsey Pecos: 88.9%
Lauryn Decristofaro: 66.7%
Margalit Ancheta: 100.0%
Lyda Nola: 55.6%
Donielle Galaska: 66.7%
```
