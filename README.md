# Curso "Introducción al Procesamiento del Lenguaje Natural con Python - Parte II" - Grupo de Ingeniería Linguística, UNAM
Material usado en el curso "Introducción al Procesamiento Natural con Python - Parte II" del Grupo de Ingeniería Lingüistica de la UNAM.

Todas las sesiones se detallan a continuación, y se añaden links para visualizar las notebooks usadas en cada sesión.

---

## 0. Repaso de Python
* **0.1 Sintaxis de Python**
  - cómo escribir una línea de código
  - cómo nombrar variables
  - para qué sirven las variables
  - qué son las palabras reservadas
* **0.2 Strings**
  - qué son
  - comparar dos strings
    - `string1 == string2`
  - qué hacen:
    - `len(string)`
    - `string.lower()`
    - `string.capitalize()`
*  **0.3 Listas**
    - qué son
    - cuál es su utilidad en la lingüistica computacional
    - cómo acceder a un elemento en una lista por medio de su índice
    - cómo acceder a varios elementos dentro de una lista por medio de sus índices
    - qué hacen los métodos `sorted(lista)`, `len(lista)`, `.append()`, `.pop()`
* **0.4 Condiciones `if`**
  - qué es
  - cómo funciona
  - condiciones `if`-`else`
  - condiciones `if`-`elif`
* **0.5 Ciclos `for`**
  - qué son
  - cómo funcionan
* **0.6 Lectura y escritura de archivos con `pandas`**
  - cómo leer un archivo `.csv` en Python y guardarlo en una variable
  - cómo guardar un archivo en formato `.csv` en nuestro Drive
* **0.7 Funciones**
  - qué son
  - cómo se nombran
  - qué es el "parámetro" de una función
  - qué significa que una función "regrese" algo
  - cuál es la utilidad de usar funciones
  - qué es una librería 

### Notebook:

https://github.com/juanmvsa/CursoPLN2-UNAM/blob/main/sesio%CC%81n%200%20-%20Repaso%20de%20Python/sesio%CC%81n%200%20-%20Repaso.ipynb

---

## 1. Principales técnicas del PLN
* **1.1 Tokenización** 
  - qué es
  - cómo realizarlo
* **1.2  Lemmatización** 
  - qué es
  - cómo realizarlo
  - cómo escribir casos especiales o que no estén dentro de los modelos de spaCy
* **1.3  Part-of-Speech Tagging**
  - qué es, cómo se hace en spaCy
  - cómo entender las etiquetas
  - Ejercicio de desambigüación de oraciones usando POS
* **1.4  Relaciones sintácticas**
  - cómo hacer análisis de dependencias sintácticas con spaCy
  - cómo buscar la descripción de las etiquetas de spaCy
  - Ejercicio: Obtener la lista de dependencias sintácticas de una oración. ¿Qué significa ROOT y qué tiene que ver esa token con las demás ?

### Notebook:

https://github.com/juanmvsa/CursoPLN2-UNAM/blob/main/sesio%CC%81n%201%20-%20Principales%20te%CC%81cnicas%20del%20PLN.ipynb

---

## 2 y 3. Exploración y extracción de características lingüísticas de textos usando spaCy
* **2.1 El objeto ‘token’ en spaCy**
  - qué es
  - cómo imprimir tokens en una notebook 
  - qué hace doc.sents
* **2.2 El método `doc.noun_chunks`**
  - qué regresa este método
* **2.3 El `span` de spaCy**
  - qué es
  - cómo obtener los spans de un `doc`
  - ejemplo de cómo obtener la similitud semántica de dos spans
* **2.4 Modelos de spaCy**
  - qué son
  - cómo cargarlos
  - cómo identificar sus diferencias
* **2.5 Dependencias sintácticas**
  - qué son
  - cómo obtener las dependencias de una oración usando una variable `nlp` con un modelo de spaCy precargado
* **2.6 Extracción de tokens a partir de sus dependencias sintácticas**
  - cómo obtener los tokens por oración
* **2.7 Ejercicio de repaso: Extracción de características lingüísticas de un texto**
  - cómo crear una variable de pandas, que contenga una tabla de datos en formato `.csv`

### Notebook:

https://github.com/juanmvsa/CursoPLN2-UNAM/blob/main/sesio%CC%81n%202%20-%20Exploracio%CC%81n%20y%20extraccio%CC%81n%20de%20caracteri%CC%81sticas%20lingu%CC%88i%CC%81sticas%20de%20textos%20usando%20spaCy/sesiones%202%20y%203%20-%20Exploracio%CC%81n%20y%20extraccio%CC%81n%20de%20caracteri%CC%81sticas%20lingu%CC%88i%CC%81sticas%20de%20textos%20usando%20spaCy.ipynb

---

## 4.1 Extracción de caracterícticas lingüísticas (parte 2)
  - cómo obtener sólo ciertas partes del discurso usando una condición `if`
  - función `obtiene_pos` para obtener sólo los `token.text` de un texto, que esten etiquetados con cierto `token.pos_`

### Notebook:

https://github.com/juanmvsa/CursoPLN2-UNAM/blob/main/sesio%CC%81n%204%20-%20Extraccio%CC%81n%20caracteri%CC%81sticas%20lingu%CC%88i%CC%81sticas%2C%20y%20vectores%20de%20palabras/sesio%CC%81n%204.1%20-%20Extraccio%CC%81n%20de%20caracteri%CC%81sticas%20lingu%CC%88i%CC%81sticas.ipynb

---

## 4.2 Vectores de palabras
* **4.2.1 Introducción**
  - qué son
  - por qué usarlos, y no hacer una simple representación con 1s y 0s
* **4.2.2 Ejemplos**
  - cómo usar la función `similarity` de spaCy para obtener la similitud semántica entre dos tokens
  - cómo usar la función `similarity` de spaCy para obtener la similitud semántica entre dos tokens de tipo `NOUN`
* **4.2.3 Funciones**
  - función `cargar_datos`
  - función `elimina_columnas_en_pandas`
  - función `calcula_estadisticas_basicas`

### Notebook:

https://github.com/juanmvsa/CursoPLN2-UNAM/blob/main/sesio%CC%81n%204%20-%20Extraccio%CC%81n%20caracteri%CC%81sticas%20lingu%CC%88i%CC%81sticas%2C%20y%20vectores%20de%20palabras/sesio%CC%81n%204.2%20-%20Vectores%20de%20palabras.ipynb

---

## 5. Visualizaciones


### Notebook:

---

## 6. Reglas manuales en spaCy e introducción a modelos estadísticos con `huggingface`


### Notebook:

https://github.com/juanmvsa/CursoPLN2-UNAM/blob/main/sesio%CC%81n%206%20-%20Reglas%20manuales%20en%20spaCy%20e%20introduccio%CC%81n%20a%20modelos%20estadi%CC%81sticos%20con%20huggingface.ipynb

---

## 7. Entrenamiento de modelos de clasificación supervisada, y procesamiento con modelos de aprendizaje profundo en `huggingface``


### Notebook:


