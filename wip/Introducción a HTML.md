# Introducción a HTML
HTML (Hypertext Markup Language) es el código que se emplea para estructurar una página Web y su contenido. Por ejemplo, el contenido podría estar estructurado con un conjunto de párrafos, una lista de viñetas o empleando imágenes y tablas de datos.

# ¿Qué es HTML?
HTML es un lenguaje de hipertexto (markup) que define la estructura del contenido. Consta de una serie de elementos que son empleados para delimitar partes del contenido para hacer que aparezcan o se comporten de cierta forma. Los tags pueden hacer que una palabra o imagen tengan un enlace a otro elemento, proveer itálicas a las palabras o cambiar el tamaño de la fuente.

Fragmento de HTML sin elementos

```html
En 1980, el físico Tim Berners-Lee propuso y elaboró un prototipo de ENQUIRE, un sistema para que los investigadores de CERN emplearan y compartieran documentos.En 1989, Berners-Lee escribió un memorandum proponiendo un sistema de hipertexto basado en HTML.  Berners-Lee especificó e implementó el software del navegador y el servidor a finales de 1990.
```

Fragmento de HTML con elementos
```html
<p>En 1980, el físico Tim Berners-Lee propuso y elaboró un prototipo de ENQUIRE, un sistema para que los investigadores de CERN emplearan y compartieran documentos.</p><p>En 1989, Berners-Lee escribió un memorandum proponiendo un sistema de hipertexto basado en HTML.</p><p>Berners-Lee especificó e implementó el software del navegador y el servidor a finales de 1990.</p>
```
Los principales elementos de un elemento son:
1. Tag de apertura: Consta del nombre del elemento (p, en este caso) envuelto en símbolos de menor y mayor que (`<`, `>`). Esto determina dónde inicia el elemento.
1. El tag  de cierre: Es el mismo que el tag de apertura, excepto que incluye una diagonal hacia adelante (`/`) antes del nombre del elemento. Esto indica dónde termina el elemento.
1. El contenido: Este es el contenido del elemento, que en este caso es solo texto.
1. El elemento: Incluye el tag de apertura, el tag de cierre y el contenido.

Los elementos pueden tener atributos como el siguiente:

```html
<p class="history-remark">En 1980, el físico Tim Berners-Lee propuso y elaboró un prototipo de ENQUIRE, un sistema para que los investigadores de CERN emplearan y compartieran documentos.</p>
```

Los atributos proveen información adicional acerca del elemento que no aparece en el contenido. En este caso class es el nombre del atributo e history-remark es el valor del atributo. El atributo class permite asignar al elemento un identificador no único que puede ser empleado para referirlo (así como otros elementos que tengan el mismo valor class). Los atributos se emplean para definir aspectos de apariencia visual, entre otros.

Un atributo siempre debe contar con:
1. Un espacio entre él y el nombre del elemento (o el atributo previo).
1. El nombre del atributo seguido del símbolo igual `=`.
1. El valor del atributo envuelto en símbolos de comillas.

# Elementos anidados
Es posible colocar elementos dentro de otros. Esto se conoce como anidado (nesting en inglés). 

En el siguiente fragmento de HTML el elemento `<strong>` se encuentra anidado dentro del elemento `<p>`

```html
<p>En 1980, el físico Tim Berners-Lee propuso y elaboró un prototipo de <strong>ENQUIRE</strong>, un sistema para que los investigadores de CERN emplearan y compartieran documentos.</p>
```

Es importante verificar que los elementos se encuentren anidados adecuadamente. El siguiente fragmento de HTML es inválido 
```html
<p>En 1980, el físico Tim Berners-Lee propuso y elaboró un prototipo de <strong>ENQUIRE</p>, un sistema para que los investigadores de CERN emplearan y compartieran documentos.</strong>
```

Los elementos anidados deben cerrarse (contar con su tag de cierre) antes que los elementos que los contienen.

# Elementos vacíos
Algunos elementos carecen de contenido y se denominan elementos vacíos. Por ejemplo el elemento `<img>`

```html
<img src="./images/favicon.ico" alt="Ícono de la aplicación"/>
```

Este elemento contiene dos atributos y con cuenta con un tag de cierre ni contenido interno. Esto es porque un elemento de imagen no envuelve contenido que afecte. Su propósito es integrar una imagen en la página HTML en el lugar en el que se coloca.

# Anatomía de un documento HTML
Los elementos individuales de HTML se combinan para formar una página HTML completa.

Consideremos el código de la página index.html de ejemplo.

* `<!DOCTYPE html>` - doctype: Es un preámbulo requerido. En los primeros años de HTML los doctypes fueron enlaces a un conjunto de reglas que la página HTML tenía que seguir para ser considerada buen HTML, lo cual podía significar corrección automática de errores y otros aspectos. Hoy en día se requieren para asegurar que el documento se comporta adecuadamente.
* `<html></html>` - el elemento `<html>`: Este elemento envuelve el contenido completo de la página y también se conoce como el elemento raíz.
* `<head></head>` - el elemento `<head>`: Este elemento contiene todo lo que se requiera incluir en una página HTML que no sea el contenido que se muestre a las personas que consulten la página. Esto incluye aspectos como palabras clave, la descripción de la página que se desee aparezca en los resultados de búsqueda, las plantillas CSS para definir el estilo del contenido, declaración del conjunto de caracteres y más.
* `<meta charset="utf-8">`: Este elemento define el conjunto de caracteres que será empleado por el documento. UTF-8 incluye la mayoría de los caracteres de la vasta mayoría de los lenguajes escritos.
* `<title></title>` - el elemento `<title>`: 