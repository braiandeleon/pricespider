# Introduccion a HTML 

Todas las páginas web utilizan HTML. No es un lenguaje de programación propiamente dicho, sino, un lenguaje de Markup(opens in a new tab), lo cual significa que incorporan al texto marcas o etiquetas que luego son interpretadas para darle información extra sobre la estructura del texto. En el caso de HTML, este será interpretado por los browsers, que también presentaran el código en forma gráfica.

![Alt text](https://articulateusercontent.com/rise/courses/dl1cg5TN83uEG1OIka3o-Brt45jemcMm/voDQz2GfAvghZQQB.jpg)

Es decir, que las paginas web se escriben con un lenguaje de etiquetado (marcado) notese que no hemos dicho que es un lenguaje de programacion. Que ademas, contiene links (Hiper Vinculos o Hyper Text). Ademas de dotar a la pagina web con el texto, la estructura y posicion de esta no hace nada mas. 

## 1. Elementos basicos del HTML 

HTML define una serie de elementos (o etiquetas, o tags) que serviran para delimitar texto. Cada tag está encerrado en < > y tiene un nombre. Los tags se abren y se cierran, los tags de cerrado incluyen con un “/” en el principio del tag que cierra. Por ejemplo:

<element>
  ...
</element>

![Alt text](https://articulateusercontent.com/rise/courses/dl1cg5TN83uEG1OIka3o-Brt45jemcMm/xFd0mbhiQDsuH6NN.png)

Algunos tags html, por su naturaleza, no necesitan tener nada adentro. Por lo tanto podemos abreviar su escritura y en vez de abrir y cerrar el tag, simplemente agregamos un “/” antes del bracket final.




<pre>
    <code>
        &lt;img src="http://imagen.com/img.jpg" /&gt;
    </code>
</pre>

## 2. Atributos

En su mayoría de los atributos de un elemento son pares nombre-valor, separados por un signo de igual «=» y escritos en la etiqueta de comienzo de un elemento, después del nombre del elemento. El valor puede estar rodeado por comillas dobles o simples. Los atributos de los tags nos sirven para cambiar su comportamiento o configurarlos.

Por ejemplo, el tag "img" sirve para mostrar una imagen. Este tag recibe el atributo src que indica la URL (opens in a new tab)de donde está la imagen que queremos mostrar.

## 3. Tags basicos

<p>

## html 
El tag "html" va a contener a todos los demás tags dentro suyo. Este tag básicamente sirve para avisarle al browser que el contenido debe ser interpretado como html.

## head
Este tag "head" sirve para contener tags que contengan información sobre el documento, pero es información que no queremos que se renderee. Comunmente contiene el titulo de la página y links a recursos externos que pueda usar la página (javascript o css).

## title

El tag "title" es el título de la página, se mostrará en el tab del browser o en la parte superior (pero no en la página).

## body 
En este tag "body" estára encerrado todo lo que querramos que se vea en la pantalla.

Entonces, hasta ahora, un documento HTML se ve así.

Como ven, para mayor fácilidad en la lectura y la estructuración del documento, el documento HTML se escribe indentando (o usando sangría).

(Todos los tags que presentaremos más abajo van siempre adentro de un tag "body")


## p
El tag "p" es para los párrafos. Mostrará el texto contenido dentro en una nueva línea.

<pre>
    <code>
        &lt;p&gt;Soy un párrafo&lt;/p&gt;
    </code>
</pre>



## span 
El elemento "span" es un contenedor de texto genérico. No inserta una nueva linea, como lo hace el elemento p. Sirve básicamente para darle estilo al texto.

## div 
El elemento "div" es un contenedor genérico. Es usado principalmente para dar estilo, imaginen que es una caja (cuyo tamaño y color podes modificar a piacere), y que dentro podés poner otras cajas iguales.

## a
El tag "a" (del inglés anchor), nos permite crear links a otros documentos y páginas. Este tag recibe el atributo href que indica a dónde apunta el link.

<pre>
    <code>
       &lt;a href="http://www.soyhenry.com"&gt;Esto es un link!&lt;/a&gt;
    </code>
</pre>



## h1...h6
Los tags "h1, h2, h3, h4, h5, h6" de encabezado o títulos, están pensandos del 1 al 6, para indicar la importancia del contenido y su jerarquía.



## img
Este tag "img" nos permite mostrar imágenes en la pantalla. Necesita el atributo src que indica la URL de donde sacar la imagen a mostrar.

<pre>
    <code>
       &lt;img src="http://www.soyhenry.com/imageurl.jpg" /&gt;
    </code>
</pre>



## ul
Este tag "ul" representa una lista desordenada (del inglés “unordered list”). Este tag está diseñado para contener otros tags de tipo item. También existe el tag "ol" que viene de “ordered list”.

## li
Los tags "li" son los que contienen los items de la lista (‘list item’).

</p>

# Introduccion a CSS

Como vimos, HTML nos sirve para dar estructura al contenido. En las primeras épocas de internet las páginas eran así. De hecho, todavía esta online la primera página web(opens in a new tab). Como ven es bastante aburrida. Luego se introdujo el concepto de CSS (Cascading Style Sheets); ¡una forma de poder agregar color y estilos en nuestras páginas!

## Reglas CSS

Básicamente una regla CSS está compuesta por un atributo o propiedad y un valor. Seǵun el atributo que usemos y el valor que le pongamos a ese atributo vamos a obtener resultados visuales distintos en nuestro html.
Por ejemplo:

<pre>
    <code>
html  {
  color: red; /* "Color" es la propiedad y "red" el valor */
  font-size: 12px; /* "font-size" es la propiedad y "12px" el valor */
      }
    </code>
</pre>

En este ejemplo, vemos dos atributos: color y font-size, el primero permite modificar el color del texto, en este caso está seteado a black; el segundo indica el tamaño del texto, en este caso 17px.
Es importante notar que distintos atributos pueden recibir distintos valores, generalmente los que indican un color reciben un color (red, blue, etc…), los que son medidas reciben una medida (12px, 15px, etc…), y hay otras propiedades que reciben valor especificos, por ejemplo: la propiedad border (que dibuja un borde alrededor de un elemento) recibe tres valores: el color del borde, el ancho de la linea y el tipo de linea (punteada, continua, etc…).

Hay muchos atributos CSS disponibles, más de los que podemos recordar. Así que no se asusten, con el tiempo van a empezar a memorizar estas propiedades. Pueden ver una lista completa acá(opens in a new tab).

Antes de empezar a dar estilos, necesitamos una forma de decirle al browser qué vamos a darles reglas de estilo. Hay varias formas de lograr esto (más adelante veremos en detalle como funcionan cada una):

Usando el atributo style: esta es la forma primitiva más simple, básicamente le damos reglas a cada tag html.

Usando el tag "style": Se utiliza este tag en el "head" del documento HTML, con esto logramos agrupar todas las reglas que luego queremos que se apliquen a los elementos HTML.


Usar el tag "link": Este método nos permite definir las reglas CSS en un documento separado e importarlo a nuestra página (la ventaja que tiene es que podemos importar el mismo CSS a varias páginas).


## Selectores

Para poder aplicar reglas de estilo a los elementos html, necesitamos una forma de saber cómo seleccionar los elementos a los que deseamos aplicar las reglas, para esto sirven los selectores CSS.

![Alt text](https://articulateusercontent.com/rise/courses/dl1cg5TN83uEG1OIka3o-Brt45jemcMm/bBMGbmy7TByuSp9s.png)

Hay varios tipos de selectores, los más básicos son los de tipo, donde indicamos a qué clase de elemntos se van a aplicar las reglas, el ejemplo de arriba usa un selector de tipo. Está diciendo: aplicarle a todos los elementos de tipo "p" la regla de texto color rojo.

El selector de tipo se puede usar con cualquier tipo de tag: p, div, body, etc. Otra forma de usar selectors poniendole un nombre o identificador a cada elemento HTML. Para esto existe un atributo que pueden recibir todos los tags llamados: id y class.

<pre>
    <code>
&lt;div id="divId"&gt;&lt;/div&gt;
&lt;div class="divClass"&gt;&lt;/div&gt;
    </code>
</pre>

Id: son nombre que sólo pueden aparecer una sólo vez en el documento. Es super especifico y sirve para seleccionar UN solo elemento en particular

Class: podemos asignarle el nombre de una clase a un grupo de elementos html.

## Selectores basicos

Selector de tipo
Selecciona todos los elementos que coinciden con el nombre del elemento especificado.
Sintaxis: eltname
Ejemplo: input se aplicará a cualquier elemento "input".


bullet
Selector de clase
Selecciona todos los elementos que tienen el atributo de class especificado.
Sintaxis: .classname
Ejemplo: .index seleccionará cualquier elemento que tenga la clase “index”.


bullet
Selector de ID
Selecciona un elemento basándose en el valor de su atributo id. Solo puede haber un elemento con un determinado ID dentro de un documento.
Sintaxis: #idname
Ejemplo: #toc se aplicará a cualquier elemento que tenga el ID “toc”.


bullet
Selector universal
Selecciona todos los elementos. Opcionalmente, puede estar restringido a un espacio de nombre específico o a todos los espacios de nombres.
Sintaxis: ns| |
Ejemplo: * se aplicará a todos los elementos del documento.


bullet
Selector de atributo
Selecciona elementos basándose en el valor de un determinado atributo.
Sintaxis: [attr] [attr=value] [attr~=value] [attr|=value] [attr^=value] [attr$=value] [attr*=value]
Ejemplo: [autoplay] seleccionará todos los elementos que tengan el atributo “autoplay” establecido (a cualquier valor).

## Box Model

Ahora que sabemos como seleccionar los elementos a los que queremos aplicar las reglas podemos escribir qué reglas queremos que se apliquen. Para el ejemplo vamos a usar la etiqueta <style>.


<pre>
    <code>
&lt;style&gt;
  body {}

  .divClass {}

  #divId {}
&lt;/style&gt;
    </code>
</pre>


En el ejemplo de arriba vemos tres selectores. El primero es para el elemento body, el segundo para todos los elementos de la clase divClass y el tercero para el elemento que tenga el id: divId. Dentro de los {} vamos a escribir todas las reglas que queremos que se apliquen a esos elementos.

Ahora que tenemos los elementos seleccionados podemos empezar a agregar las reglas que habíamos visto antes...


Para poder entender y luego manipular la forma en que los elementos HTML aparecen distribuidos en la página, tenemos que aprender cómo son representados estos en el browser.

![Alt text](https://articulateusercontent.com/rise/courses/dl1cg5TN83uEG1OIka3o-Brt45jemcMm/2ruPQGj4Yzl3j5li.png)

En un documento html cada elemento es representado como una caja rectangular y en CSS cada una de estas cajas tiene 4 capas que podemos manipular. Esto se conoce como Modelo de Caja o Box Model. 

Yendo desde afuera hacia adentro, las capas son:

margin: el espacio que separa al elemento de los otros elementos. Si los pensamos como cajas, es el espacio entre las cajas.

border: el “borde de la caja”. Podemos hacerlo visible con diferentes grosores, estilos y colores, como ya hicimos varias veces en ejercicios anteriores.

padding: el espacio entre el borde de la caja y su contenido. En la metáfora de la caja, podríamos por ejemplo tener una caja grande con algo chiquito adentro, osea que “habría mucho padding”.

content: el contenido de la caja. Por ejemplo el texto en un h1, otros tags anidados, etc, todo lo que esté contenido en el elemento.

Heigth y Width 

Podemos decirle al navegador exactamente qué tan alto y ancho queremos que sea nuestro elemento (contenido), esto se usa en div, img y otros elementos basados en la altura (para determinar el tamaño del texto, necesitaremos usar un propiedad de estilo diferente). Los valores de tamaño pueden estar en muchas medidas diferentes, pero el más común es el píxel “px”.

![Alt text](https://articulateusercontent.com/rise/courses/dl1cg5TN83uEG1OIka3o-Brt45jemcMm/YOpavDaQli8ryKtb.png)

Margin

El margen es el área transparente alrededor del elemento que deseas que no choque con nada. Es la capa más externa en el Modelo de caja.

Border

Borde establecerá un borde alrededor de su elemento, puedes determinar el tamaño, color y estilo del borde. Puede encontrar una lista de estilos de borde aquí: https://developer.mozilla.org/en-US/docs/Web/CSS/border(opens in a new tab). El borde está fuera del padding, pero dentro del margen. 

![Alt text](https://articulateusercontent.com/rise/courses/dl1cg5TN83uEG1OIka3o-Brt45jemcMm/LQOkLD9HNDTdUxwo.png)

Padding 

El padding es el área transparente entre el borde y el contenido, es similar al margen, pero para adentro

Cálculo del box model

Cuando establecemos el alto y el ancho de un elemento a traves de la regla css height y width, sólo estamos configurando el contenido. Para calcular la altura y el ancho reales, tenemos que tener en cuenta el padding, el borde y el margen.

padding es un área transparente alrededor del contenido.
border se envolverá alrededor del relleno
margin es el área transparente más externa que envuelve toda la caja.
Por ejemplo, si establecemos la altura del contenido en 20 px y el ancho en 20 px, el relleno en 5 px, el borde en 1 px y el margen en 10 px.

Altura real = 25px (contenido) + 2 * 5px (relleno, cada lado) + 2 * 1 (borde de cada lado) + 2 * 10 (margen, cada lado) = 57px
Ancho real = 25px (contenido) + 2 * 5px (relleno, cada lado) + 2 * 1 (borde de cada lado) + 2 * 10 (margen, cada lado) = 57px

Saber esto nos ayudará a dimensionar y posicionar nuestros elementos correctamente.

## Otras propiedades CSS, hojas de estilo externas y elemento

background
–
El background se puede establecer en una variedad de reglas, la más común sería establecer el fondo en un color o una imagen. Ambos se muestran a continuación.



.divClass {
background: red;
}

#divId {
background: url ('http://imageurl.com/image.jpg');
}

color
–
El color se usa sólo para texto. Establecerá el color de tu texto

font-size
–
No podemos usar ancho o alto para el texto, pero podemos determinar el tamaño de la fuente utilizada. Puede usar cualquier unidad de tamaño aquí que usaría con una fuente en un procesador de textos (px, em, in, etc.). El más popular es px.

Hojas de estilo externas y el elemento <link>

Hemos explicado cómo usar el elemento html <style>. Esto está bien si tiene una página web muy pequeña y un estilo mínimo, pero la mayoría de las páginas comenzarían a sentirse abarrotadas muy rápidamente si incluimos todo nuestro CSS en el HTML.
Afortunadamente, tenemos una solución para eso, hojas de estilo externas y el elemento <link>.

Una hoja de estilo externa es simplemente otro archivo con el tipo de archivo .css. Convencionalmente, este archivo se llama algo así como “style.css”. Podemos tomar todas las reglas de estilo que escribimos entre las etiquetas <style> y transferirlas directamente al archivo css. No necesitamos incluir nada más, solo las reglas de estilo.

Una vez que tengamos una hoja de estilo externa creada, necesitaremos asegurarnos de que el navegador lea ese archivo y aplique las reglas a nuestra página. Le decimos al navegador que busque ese archivo utilizando el elemento <link>. Podemos eliminar las etiquetas <style> y en su lugar agregar el elemento <link>. Dentro del elemento de enlace, necesitaremos proporcionar la ubicación y el tipo de archivo que estamos vinculando. Utilizaremos dos banderas, la bandera “rel” y la bandera “href”.

La bandera rel solo le dirá al navegador qué tipo de archivo es y cómo procesarlo. En nuestro caso lo configuraremos como “hoja de estilo”

La bandera href le dirá al navegador dónde encontrar el archivo. Si el archivo está en la misma carpeta que nuestro archivo html, podemos configurarlo en: “./styles.css” (esta ruta será relativa)

<link rel = "stylesheet" href = "./ styles.css" />

Ahora que tenemos nuestra hoja de estilo externa vinculada a nuestro archivo HTML, deberíamos ver las reglas de estilo que establecemos reflejadas en nuestra página.


