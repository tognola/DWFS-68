# Clase 5

## Display
La propiedad CSS display especifica si un elemento es tratado como un elemento:

- **block:** hace que el comportamiento del elemento sea como un bloque.
- **inline:** el elemento se renderizará en línea con otros elementos.
- **inline-block:**  fluyen con el texto y demás elementos como si fueran elementos en-línea y además respetan el ancho, el alto y los márgenes verticales.

Elementos block por defecto:
``` <address>
<article>
<aside>
<blockquote>
<canvas>
<dd>
<div>
<dl>
<dt>
<ul>
<fieldset>
<figcaption>
<figure>
<footer>
<form>
<h1>-<h6>
<section>
<table>
<tfoot>
<video>
<header>
<hr>
<li>
<main>
<nav>
<noscript>
<ol>
<p>
<pre>
```

Elementos inline por defecto:
```
<a>
<abbr>
<acronym>
<b>
<bdo>
<big>
<br>
<button>
<cite>
<code>
<time>
<dfn>
<em>
<i>
<img>
<input>
<kbd>
<label>
<map>
<object>
<output>
<tt>
<q>
<samp>
<script>
<select>
<small>
<span>
<strong>
<sub>
<sup>
<textarea>
<var>
```

## Float
La propiedad float especifica si un elemento debe salir del flujo normal y aparecer a la izquierda o a la derecha de su contenedor, donde los elementos de texto y los en línea aparecerán a su alrededor.

### Clear
La propiedad CSS clear especifica si un elemento puede estar al lado de elementos flotantes que lo preceden o si debe ser movido (cleared) debajo de ellos.

## Position
La propiedad position de CSS especifica cómo un elemento es posicionado en el documento. Las propiedades **top, right, bottom, y left** determinan la ubicación final de los elementos posicionados.



Un elemento posicionado es un elemento cuyo valor computado de position es **relative, absolute, fixed, o sticky**. (En otras palabras, cualquiera excepto static).

- **relative:** el desplazamiento es con respecto a su posición original.
- **absolute:** su desplazamiento es con respecto al primer contenedor padre que se encuentre posicionado.
- **fixed:** su desplazamiento es con respecto a la ventana del navegador
- **sticky:** el elemento es tratado como un relative hasta que cruza un límite establecido (por top, bottom, left o right) y pasa a ser tratada como un fixed.