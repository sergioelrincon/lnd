# Bootstrap

## Introducción

[Bootstrap](https://getbootstrap.com/) es una biblioteca de recursos CSS y Javascript que nos permite realizar desarrollos de front-end con muy poco esfuerzo y sin necesidad de conocimientos de bajo nivel en dichos lenguajes.

Fue creado por Twitter inicialmente y posteriormente liberado como código abierto. Actualmente, con cerca de 161k *starts*, es uno de los proyectos más detacados en [GitHub](https://github.com/twbs/bootstrap/).

Bootstrap cuenta con un gran número de estilos que permiten la realización de diseños responsives, estilos para la creación de menús, formularios, tablas, botones, etc. 

## Instalación

Para poder utilizar Bootstrap en nuestros proyectos no es necesario descargar el código fuente. Bastará con copiar y pegar en nuestro HTML la plantilla que se muestra en [la siguiente URL](https://getbootstrap.com/docs/5.3/getting-started/introduction/#quick-start) y comenzar a editar nuestra página a partir de dicha plantilla.

**Es importante** tener en cuenta que Bootstrap requiere la declaración del elemento `doctype`, ya que sin él es posible que algunos estilos no se muestrn corretamente:

    <!doctype html>
    <html lang="en">
    ...
    </html>

Otra forma de utilizar Bootstrap en nuestros proyectos es descargarnos el código fuente ([Compiled CSS and JS](https://www.w3schools.com/cssref/css3_pr_text-shadow.php)) e incluirlo en nuestros ficheros mediante `<link href="./css/bootstrap.css">`. En este caso, el fichero no se cacheará en el navegador y en la mayoría de los casos será necesario descargarlo, lo cual ralentizará un poco más la carga.