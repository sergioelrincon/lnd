# Bootstrap

## Introducción

[Bootstrap](https://getbootstrap.com/) es una biblioteca de recursos CSS y Javascript que nos permite realizar desarrollos de front-end con muy poco esfuerzo y sin necesidad de conocimientos de bajo nivel en dichos lenguajes.

Fue creado por Twitter inicialmente y posteriormente liberado como código abierto. Actualmente, con cerca de 161k *starts*, es uno de los proyectos más detacados en [GitHub](https://github.com/twbs/bootstrap/).

Bootstrap cuenta con un gran número de estilos que permiten la realización de diseños responsives, estilos para la creación de menús, formularios, tablas, botones, etc. 

## Instalación

Para poder utilizar Bootstrap en nuestros proyectos no es necesario descargar el código fuente. Simplemente tenemos que copiar el CDN de Bootstrap en el `<head>` de nuestra página HTML, tal y como se muestra en el siguiente ejemplo (puede variar la versión, dependiendo del momento en el que hagas la instalación):

    <head>
        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css">
    </head>

Cuando el navegador lea la línea anterior, se descargará los ficheros Bootstrap si no los tiene cacheados. Es bastante probable que ya los haya descargado previamente, ya que Bootstrap es uno de los frameworks más usados en la actualidad.

También podemos copiar y pegar en nuestro HTML la plantilla que se muestra en [la siguiente URL](https://getbootstrap.com/docs/5.3/getting-started/introduction/#quick-start) y comenzar a editar nuestra página a partir de dicha plantilla.

**Es importante** tener en cuenta que Bootstrap requiere la declaración del elemento `doctype`, ya que sin él es posible que algunos estilos no se muestrn corretamente:

    <!doctype html>
    <html lang="en">
    ...
    </html>

Una tercera forma de utilizar Bootstrap en nuestros proyectos es descargarnos el código fuente e incluirlo en nuestros ficheros mediante `<link href="./css/bootstrap.css">`. En este caso, el fichero no se cacheará en el navegador y en la mayoría de los casos será necesario descargarlo, lo cual ralentizará un poco más la carga.

Nosotros partiremos de la plantilla publicada en la web oficial para crear nuestros diseños con Bootstrap.