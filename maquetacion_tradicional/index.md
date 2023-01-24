# Maquetación tradicional


* [`<div>`](https://www.w3schools.com/tags/tag_div.ASP)
* [`<span>`](https://www.w3schools.com/tags/tag_span.asp)
* [Modelo de cajas](https://codepen.io/psande/pen/nKOJyX)
* Elementos *en bloque* (div, p, h1, h2, ul, ol, table, etc.)
  * Rompen el flujo de la línea y provocan un salto de línea anterior y posterior.
  * Ocupan todo el ancho de la etiqueta que los contiene.
* Elementos *en línea* (span, a, b, i, img, label, select, strong, u, etc.). 
  * No rompen el flujo de la línea. 
  * Se van colocando uno detrás de otro. 
  * Aceptan margin y padding, pero solo se tienen en cuenta los valores horizontales. 
  * Ignoran width y height.
* [Propiedad **display**](https://www.w3schools.com/cssref/pr_class_display.php)
  * inline
  * block
  * inline-block
  * none: desaparecen de la página. No dejan un espacio vacío, aunque siguen en el código HTML. (La propiedad "visibility: hidden" sí deja el espacio aunque no se muestre el elemento)
* [Propiedad **position**](https://www.w3schools.com/css/css_positioning.asp)
  * Valor *static*: Es el valor por defecto. El elemento sigue el flujo que le corresponde
  * Valor *relative*: Es como *static* pero sí atiende a los desplazamientos expresados
en top,bottom,left,right o z-index.
    * Desplaza el elemento con respecto a la posición en la que le tocaba estar con posicionamiento normal.
    * El espacio donde le tocaba ir queda reservado.
  * Valor *fixed*: Se le aplica top,bottom,right o z-index en relación con el comienzo
del documento.
  * Valor *absolute*: Se comporta como fixed pero en relación con la primera etiqueta
padre que tenga position:relative.
  * Valor *sticky*: Se comporta como relative hasta llegar a una posición de scroll y a
partir de entonces, fixed.
* [Propiedad **float**](https://www.w3schools.com/css/css_float.asp)
  * Especifica cómo debería flotar un elemento. Por ejemplo, nos permite especificar que una imagen flote a la izquierda de un texto en un contenedor.
* [Propiedad **box-sizing**](https://www.w3schools.com/css/css3_box-sizing.asp)
  * Si le asignamos el valor "border-box", el valor de ancho y alto que le demos al elemento será la suma de altura del contenido + padding + borde.
* [Propiedad **z-index**](https://www.w3schools.com/cssref/pr_pos_z-index.php)
  * Nos permite establecer capas decidiendo el orden de solapamiento
de estos elementos. 
  * Se mostrará por encima del resto aquel elemento de los que
se solapen con el mayor valor de z-index. 

<!-- * Centrado
  * En horizontal
    * Elementos en línea: añadiremos la propiedad "text-align:center" al contenedor padre. 
    * Elementos en bloque: dentro de su etiqueta
contenedora añadiremos la propiedad CSS "margin: X auto" al elemento que queramos centrar. (Donde X es una distancia expresada en cualquier unidad)
  * En vertical
    * Elementos en línea: configurar el mismo padding arriba y abajo. 
    * Elementos en bloque: 
      * Si conocemos la altura:
      * Si no conocemos la altura: -->