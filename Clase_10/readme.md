# Flexbox

## flex-direcion
![](https://css-tricks.com/wp-content/uploads/2018/10/flex-direction.svg)
 
 Establece el eje principal del contenido


 ```css
 .container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

## flex-wrap
![](https://css-tricks.com/wp-content/uploads/2018/10/flex-wrap.svg)

Por defecto los elementos van a tratar de encajar todos en una línea, con esta propiedad pueden cambiar eso y permitir que los elementos se ajusten según sea necesario.

```css
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

## flex-flow
Combinación de flex-direction y flex-wrap
```css
.container {
  flex-flow: column wrap;
}
```

## justify-content
![](https://css-tricks.com/wp-content/uploads/2018/10/justify-content.svg)

Define la alinación de los elementos a lo largo del eje principal (horizontalmente si trabajamos con ```flex-direction: row``` o verticalmente si trabajamos con ```flex-direction: column```).

- **flex-start** (predeterminado): los elementos se empaquetan hacia el inicio de la dirección flexible.
- **flex-end**: los artículos se empaquetan hacia el final de la dirección de flexión.
- **center**: los elementos se centran a lo largo de la línea
- **space-between**: los elementos se distribuyen uniformemente en la línea; el primer elemento está en la línea de inicio, el último elemento en la línea final
- **space-around**: los elementos se distribuyen uniformemente en la línea con el mismo espacio alrededor. Tenga en cuenta que visualmente los espacios no son iguales, ya que todos los elementos tienen el mismo espacio en ambos lados. El primer elemento tendrá una unidad de espacio contra el borde del contenedor, pero dos unidades de espacio entre el siguiente elemento porque el siguiente elemento tiene su propio espacio que se aplica.
- **space-evenly**: los elementos se distribuyen de modo que el espacio entre dos elementos (y el espacio hasta los bordes) sea igual.

## align-items
![](https://css-tricks.com/wp-content/uploads/2018/10/align-items.svg)

Como se alinean los items a lo largo del eje perpendicular.

```css
.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
}
```

## align-content
![](https://css-tricks.com/wp-content/uploads/2018/10/align-content.svg)

Como se alinean las filas cuando hay espacio extra en el contenedor.

```css
.container {
  align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;
}
```