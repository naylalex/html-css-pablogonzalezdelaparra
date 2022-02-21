# Laboratorio de CSS
Los archivos del laboratorio de CSS se encuentran en la carpeta ./labs/css_lab/student

Añade en el head de index.html una referencia a la hoja de estilo styles.css

Para ello deberás emplear el elemento link con los atributos rel y href

```html
<link rel="stylesheet" href="styles.css">
```

Añade una regla en styles.css para que el color de los encabezados h1 sea rojo
```css
h1 {
    color: red;
}
```

Añade una regla a styles.css para que el color de todos los párrafos sea verde
```css
p {
  color: green;
}
```

Modifica la regla anterior para que todos los párrafos y elementos de lista sean verdes empleando selectores múltiples

```css
p, li {
    color: green;
}
```
Elimina los estilos asociados con los elementos de lista
```css
li {
  list-style-type: none;
}
```

Modifica la viñeta de los elementos de lista para que sea cuadrada por medio del valor `square`.

En el documento HTML añade el atributo class con valor special al segundo elemento de la lista.

En la hoja de estilo añade reglas para que el color sea naranja y el peso de la fuente bold para la clase special.

```css
.special {
  color: orange;
  font-weight: bold;
}
```

En el documento HTML asigna la clase special al span que está dentro del primer párrafo.

El selector de tipo descendant combinator permite identificar elementos a los que se les apliquen reglas de estilo CSS de acuerdo con su ubicación en el documento.

```css
li em {
    color: rebeccapurple;
}
```

El selector adjacent sibling combinator permite aplicar un estilo a un elemento que siga directamente a otro en el mismo nivel de jerarquía en el documento HTML. 

Implementa un selector adjacent sibling combinator para que el tamaño de la fuente de un párrafo siguiente a encabezados h1 sea 200%.

```css
h1 + p {
    font-size: 200%;
}
```

Añade un estilo para que un span dentro de un párrafo sea de color rojo
```css
p span {
    color: red; 
}
```

Añade un estilo para que los enlaces no visitados sean de color rosa
```css
a:link {
    color: pink;
}
```
Añade un estilo para que los enlaces visitados sean de color verde
```css
a:visited {
    color: green;
}
```
