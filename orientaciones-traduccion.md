# Orientaciones para la **traducción** de Fontanero-API

## 0. Organización del trabajo
Cada capítulo tiene asignada una persona a cargo de la traducción, que es responsable de que esta se lleve a cabo. La forma de organizarse queda a criterio de cada quien: se puede realizar de forma individual, buscar colaboradores o realizar una actividad abierta de traducción (por ejemplo, a través de RLadies o el grupo de Usarios de R (RUG) local.

## I. Aspectos a tener en cuenta para la traducción del texto

__1. Al traducir lo que buscamos es generar una versión de cómo diríamos en español lo que en el capítulo está escrito en inglés.__ En algunos casos eso puede implicar alterar el orden de los elementos de una oración o agregar palabras que no estaban en el original. Lo importante es que la traducción "suene" lo más natural posible en español, respetando el contenido que se quiso transmitir en el original.

__2. La variedad dialectal del español que ocuparemos en la traducción es la de Latinoamérica__ (porque el posible público destinatario que la habla es más amplio). Trataremos de que sea una versión lo más neutra posible, por lo que:

* Evitaremos expresiones o usos locales/regionales, es decir, que no están extendidos en toda Latinoamérica.
* No utilizaremos el voseo (_vos/vosotros_). Fontanero-API está dirigido a una segunda persona, así que para cautelar la neutralidad la traduciremos como _tú_ (... _you'll learn_ > ... _aprenderás_). 

__3. Género gramatical.__ A diferencia del inglés, el español tiene género gramatical (masculino, femenino y muy, pero muy pocos neutros). En general, como R4DS está dirigido a un _tú_ y se habla de datos, variables y funciones, hay pocas situaciones en las que haya que tomar una decisión respecto de cómo manejar este tema; pero las hay. Por ejemplo, acá: “... _for collaborating with other data scientists”_. Como son pocos casos, la idea es ir resolviéndolos a medida que aparezcanu.  En principio, las dos opciones más habituales que se han seguido en traducciones de este tipo son:

* Usar el femenino para incluir al género gramatical poco representado: _para colaborar con otras científicas de datos._
* Ajustar la redacción para evitar tener que asignar un género: _para colaborar con otras personas que trabajan en Ciencia de Datos._

__4. El español es una lengua menos repetitiva que el inglés.__ Como los verbos tienen marca de persona, género y número, tenemos la flexibilidad de poder omitir el sujeto, ya que por contexto se suele entender a qué nos estamos refiriendo.

Ejemplo:
> The first argument is the name of the data frame. The second and subsequent arguments are the expressions that filter the data frame.

Traducción:
> El primer argumento es el nombre del _data frame_. El segundo y los subsiguientes son las expresiones que filtran el _data frame_.

O incluso:
> El primer argumento es el nombre del _data frame_. El segundo y los subsiguientes son las expresiones para filtrarlo.

En todos los casos, hay que tratar de pensar cómo suena más natural/normal en español y cómo queda más claro para quien lee.

__5. Hay regularidades que no siempre se cumplen.__ Por ejemplo, en inglés las palabras con función adjetiva se anteponen a los sustantivos (missing values, help pages, etc.), mientras que en español suele ser al revés: ponemos los adjetivos después del sustantivo: valores faltantes, páginas de ayuda, etc.
Sin embargo, hay casos en que en español la forma “no marcada”, es decir, la que nos suena más natural, es con el adjetivo al principio:

Ejemplo:
> ...this small example helps to understand... > ...este pequeño ejemplo ayuda a entender...

En general, ante dudas de este tipo, pensar en qué es lo que suena más natural/normal en español.

__6. Las expresiones idiomáticas no son traducibles de manera literal.__ En caso de que las hubiere (lo iremos descubriendo en el camino), hay que proponer una traducción que permita entender el sentido de ella.

Ejemplo:  
> _it’s raining cats and dogs_ > _está lloviendo a cántaros_

__7. Toma distancia para revisar.__ Cuando trabajamos mucho rato en un texto cuesta identificar errores de tipeo. Como sugerencia, una vez que termines la traducción del capítulo deja pasar algunas horas (o un día) antes de hacer la última lectura y enviarla. Eso hace más fácil que salten a la vista este tipo de detalles y permite que quienes hagan la revisión se concentren en la calidad de la traducción más que en correcciones ortotipográficas.

## II. Traducción (o no) de términos técnicos.
Hay términos técnicos que será necesario traducir y otros que no. El criterio suele estar en si existe una versión en español extendida (o entendible), o si se suele utilizar la versión original en inglés. En el caso de los últimos, hay que determinar qué género gramatical asignarle y si ofreceremos una traducción explicativa la primera vez que los utilicemos.
A medida que avancemos con la traducción, la idea es ir discutiendo este punto en el canal a través de issues en el repositorio. A partir de lo que se acuerde, iremos completando las siguientes listas de términos.

#### Términos técnicos que se traducen
Pese a que hay términos que traduciremos al español, es importante que quien traduzca evalúe si corresponde mencionar de todos modos el término en inglés la primera vez. Por ejemplo, si bien _string_ es un término que tiene una traducción (_cadena de caracteres_) la primera vez que se menciona sería útil ofrecer también la versión en inglés, porque así resulta más claro por qué el paquete se llama __stringr__. Por ejemplo: "Este capítulo te introducirá en la manipulación de cadenas de caracteres (_strings_) en R.". En el caso de términos cuya traducción en español no está tan extendida, es necesario evaluar si corresponde agregar una pequeña explicación (por ejemplo, _mapping_ > "..._mapear, es decir, indicar qué variables se asignarán a cada eje_...".

| término en inglés | traducción a utilizar |
| ----------- | ----------- |
| aesthetics | estéticas |
| assignment operator | operador de asignación |
| atomic vectors | vectores atómicos |
| backtick (\`) | acento grave |
| base R | R base |
| by default | por defecto |
| click | hacer clic |
| console | consola |
| debugging | depurar |
| dataset | conjunto de datos / set de datos |
| facet | separar facetas |
| input | input (la palabra existe en español, no se traduce) |
| list-columns | columnas-lista |
| log-transformation | transformación logarítmica |
| mapping | mapear |
| named list | lista nombrada |
| partial matching | coincidencia parcial |
| parse | segmentar o analizar (depende del contexto) |
| placeholder | marcador de posición |
| query | consulta |
| raw data | datos sin procesar |
| test set | set/datos de validación |
| training set | set/datos de entrenamiento |
| tidy data | datos ordenados |
| ... | ... |


#### Términos técnicos que se mantienen
Estos términos irán _en cursiva_. De ser pertinente, se debe ofrecer una posible traducción al español, ya que en algunos casos permite entender mejor el concepto que está detrás (por ejemplo, que _pipe_ es tubo / tubería). En caso de que sean nombres de paquetes o palabras nuevas en inglés (cuyo uso en este contexto no se encontraría en un diccionario), ofreceremos una indicación sobre cómo se pronuncian la primera vez que aparezcan. Por ejemplo: "... el uso de un _pipe_ (/paip/)...".  

| no traducir    |
| ----------------------------|
| Big Data |
| un _dashboard_ |
| un _data frame_ |
| un _notebook_ |
| un _output_    |
| un _pipe_ |
| un _script_ |
| un _tibble_    |
| el _tidyverse_    |
| ... |


[Las Carpentries](https://github.com/Carpentries-ES/board/blob/master/Convenciones_Traduccion.md) tienen algunas convenciones que podemos ir revisando y ver si se adecuan al propósito de la traducción que estamos realizando.

## III. Traducción del código:

__1. Nombres de funciones.__ Se debe ofrecer una traducción la primera vez que aparecen.

Original:
> * Pick observations by their values (`filter()`).
> * Reorder the rows (`arrange()`).

Traducción:
> * Escoger observaciones según sus valores (`filter()`  — del inglés _filtrar_).
> * Reordenar las filas (`arrange()`  — del inglés _organizar_).


__3. Los objetos/variables creados a partir de los datos se traducen, al igual que los títulos, etiquetas y nombres de ejes en los gráficos.__

Por ejemplo:

__original__
```r
not_cancelled <- flights %>%
  filter(!is.na(dep_delay), !is.na(arr_delay))
  ```

  __traducción variable + datos__
```r
no_cancelados <- vuelos %>%
  filter(!is.na(atraso_salida), !is.na(atraso_llegada))
  ```
## IV. Aspectos de formato

* Los nombres de los paquetes van __en negrita__.
* Los términos en inglés van _en cursiva_.
* La propuesta de pronunciación de un término en inglés va entre barras: /tibl/.

## V. Aspectos de ortografía / gramática del español

* Ni los demostrativos ni el adverbio "solo" se tildan.
* Días y meses se escriben con minúscula en español.
* Los títulos llevan mayúscula solo en la palabra inicial (salvo que incluyan un nombre propio).
* Para consultar la forma convencional de una abreviatura en español, revisar este [enlace](http://www.rae.es/diccionario-panhispanico-de-dudas/apendices/abreviaturas). Hasta el momento ha aparecido _por ejemplo_ > _p. ej._.


