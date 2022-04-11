# Curso "Introducción al Procesamiento Natural con Python - Parte II" - Grupo de Ingeniería Linguística, UNAM
Material usado en el curso "Introducción al Procesamiento Natural con Python - Parte II" del Grupo de Ingeniería Lingüistica de la UNAM.

Todas las sesiones se detallan a continuación, y se añaden links para visualizar las notebooks usadas en cada sesión.

## 0. Repaso de Python
* 0.1 **Sintaxis de Python**
  - cómo escribir una línea de código
  - cómo nombrar variables
  - para qué sirven las variables
  - qué son las palabras reservadas
* 0.2 **Strings**
  - qué son
  - comparar dos strings
    - `string1 == string2`
  - qué hacen:
    - `len(string)`
    - `string.lower()`
    - `string.capitalize()`
*  0.3 **Listas**
  - qué son
  - cuál es su utilidad en la lingüistica computacional
  - cómo acceder a un elemento en una lista por medio de su índice:
    - `lista[indice]`
  - cómo acceder a varios elementos dentro de una lista por medio de sus índices:
    - `lista[indice_inicial:indice_final]`
  - qué hacen: 
    - `sorted(lista)`
    - `len(lista)`
    - `.append()`
    - `.pop()`
* 0.4 **Condiciones `if`**
  - qué es
  - cómo funciona
  - condiciones `if`-`else`
  - condiciones `if`-`elif`
* 0.5 **Ciclos `for`**
  - qué son
  - cómo funcionan
* 0.6 **Lectura y escritura de archivos con `pandas`**
  - cómo leer un archivo `.csv` en Python y guardarlo en una variable
  - cómo guardar un archivo en formato `.csv` en nuestro Drive
* 0.7 **Funciones**
  - qué son
  - cómo se nombran
  - qué es el "parámetro" de una función
  - qué significa que una función "regrese" algo
  - cuál es la utilidad de usar funciones
  - qué es una librería 

## 1. Principales técnicas del PLN

* 1.1 **Tokenización** 
- qué es
- cómo realizarlo

* 1.2  **Lemmatización** 
- qué es
- cómo realizarlo
- cómo escribir casos especiales o que no estén dentro de los modelos de spaCy

* 1.3  **Part-of-Speech Tagging**
- qué es, cómo se hace en spaCy
- cómo entender las etiquetas
- Ejercicio de desambigüación de oraciones usando POS

* 1.4  **Relaciones sintácticas**: 
- cómo hacer análisis de dependencias sintácticas con spaCy
- cómo buscar la descripción de las etiquetas de spaCy
- Ejercicio: Obtener la lista de dependencias sintácticas de una oración. ¿Qué significa ROOT y qué tiene que ver esa token con las demás ?
