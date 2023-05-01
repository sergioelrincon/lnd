# XML Schema

## Introducción

Un esquema XML es un documento que describe la estructura y las restricciones de los datos que se pueden incluir en un documento XML. Básicamente, un esquema XML es como un mapa que define qué elementos y atributos se pueden usar en un documento XML, así como las reglas que se deben seguir al utilizarlos.

En un esquema XML, se definen los **elementos** que se pueden utilizar en un documento XML y la **estructura** que deben tener. Por ejemplo, si estuviéramos creando un esquema para un documento XML que describe los detalles de un libro, podríamos definir que el elemento raíz se llame "libro" y que tenga sub-elementos para el título, el autor, el año de publicación, etc. También podríamos especificar que algunos elementos son obligatorios y otros son opcionales.

Además de los elementos, también se pueden definir **atributos** en un esquema XML. Los atributos son información adicional que se puede agregar a un elemento. Por ejemplo, si nuestro esquema define un elemento para la portada de un libro, podríamos incluir un atributo para la imagen de la portada.

Un esquema XML es una herramienta muy útil para asegurarnos de que los documentos XML que creamos sigan una estructura consistente y coherente, lo que facilita el intercambio de información entre diferentes sistemas y aplicaciones.

## Ventajas frente al uso de DTD

Tanto los XML Schema como los Document Type Definitions (DTD) se utilizan para validar documentos XML y definir su estructura. Sin embargo, los XML Schema tienen varias ventajas sobre los DTD:

* **Tipos de datos más avanzados:** XML Schema ofrece una amplia variedad de tipos de datos, incluyendo tipos de datos de fecha y hora, tipos de datos numéricos y tipos de datos personalizados. Los DTD solo admiten un conjunto limitado de tipos de datos, lo que limita la precisión y flexibilidad en la validación de documentos.
  
* **Soporte para espacios de nombres:** Los XML Schema admiten el uso de espacios de nombres, lo que permite definir elementos y atributos con el mismo nombre en diferentes contextos. Los DTD no ofrecen soporte para espacios de nombres, lo que puede dificultar la creación de documentos XML complejos y bien estructurados.
  
* **Validación más exhaustiva:** XML Schema permite realizar una validación más exhaustiva de documentos XML que los DTD. Los XML Schema permiten la validación de atributos específicos, valores de atributos y valores de elementos, lo que aumenta la precisión y la calidad de la validación.
  
* **Mejora de la legibilidad:** Los XML Schema son más legibles que los DTD debido a su sintaxis clara y estructurada. Esto hace que sea más fácil para los desarrolladores y los usuarios entender y trabajar con los esquemas.
  
Aunque los DTD siguen siendo utilizados en algunos proyectos, los XML Schema ofrecen muchas ventajas sobre los DTD y son la opción preferida para la validación y definición de estructuras de documentos XML en la mayoría de los casos.

## Creación de un fichero XSD

Crear un fichero XSD puede parecer un poco compleja al principio, pero una vez que entiendes la estructura básica, es bastante sencillo. Aquí hay algunos pasos para crear un fichero XSD básico:

* Comprender la **estructura básica** del XSD: En un fichero XSD, se define la estructura y las restricciones de los datos que se pueden incluir en un documento XML. Un XSD utiliza una estructura jerárquica de elementos y atributos para definir la estructura del documento XML. **El elemento raíz en un XSD es "schema"** y dentro de él se definen los elementos que se utilizarán en el documento XML.
  
* Crear el **esqueleto** del fichero XSD: Inicie un editor y cree un nuevo documento. En la primera línea, escriba `<?xml version="1.0" encoding="UTF-8"?>` para indicar que se trata de un documento XML. En la segunda línea, escriba `<xsd:schema xmlns:xsd="http://www.w3.org/2001/XMLSchema">` para indicar que está creando un fichero XSD.
  
* Definir los **elementos**: En el esqueleto del fichero XSD, comience a definir los elementos que se utilizarán en el documento XML. Para definir un elemento, utilice la etiqueta `<xsd:element>` y especifique su nombre y su tipo de datos. Por ejemplo, si estuviéramos creando un XSD para un documento XML que describe los detalles de un libro, podríamos definir un elemento llamado "title" de la siguiente manera:

        <xsd:element name="title" type="xsd:string"/>

    Aquí, estamos definiendo un elemento llamado "title" con un tipo de datos de "xsd:string", lo que significa que el valor del elemento debe ser una cadena de texto.

* Definir **atributos**: Además de los elementos, también se pueden definir atributos en un fichero XSD. Para definir un atributo, utilice la etiqueta `<xsd:attribute>` y especifique su nombre y su tipo de datos. Por ejemplo, si estuviéramos creando un XSD para un documento XML que describe los detalles de un libro, podríamos definir un atributo llamado "isbn" para el elemento "book" de la siguiente manera:

        <xsd:element name="book">
            <xsd:complexType>
                <xsd:attribute name="isbn" type="xsd:string"/>
            </xsd:complexType>
        </xsd:element>

    Aquí, estamos definiendo un elemento llamado "book" y dentro de él estamos definiendo un atributo llamado "isbn" con un tipo de datos de "xsd:string".

* Guardar y probar el fichero XSD: Una vez que haya definido todos los elementos y atributos necesarios en su fichero XSD, guárdelo en su ordenador con una extensión ".xsd". Ahora puede probar su fichero XSD abriendo un documento XML en un editor y añadiendo la siguiente línea al principio:

        <?xml version="1.0" encoding="UTF-8"?>
        <book xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="[ruta al fichero XSD]">
