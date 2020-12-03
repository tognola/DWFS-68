# Clase 4: CSS

## Selectores

![](https://lh5.googleusercontent.com/m_4qLb-iAq8Tkhs1ob-VdgRYlvxt6YvhjGmmffQ3pqsO8tJ0k44RrANwFzy3EIJFpiyMFUQ6ulxrwvPfaIMGWVN8hbiHbtgut70LCzKlrGEB3jwP-v1M9-BACOAMB2lKRYUPXtkZut0)

### Tipos de selectores:
- Selector universal (*)
- Selector por tipo (body, p, a, etc.)
- Selector por clase (.mi-clase)
- Selector por ID (#id-elemento)

### Especificidad de selectores:
ID > clase > tipo > universal >>>> !important.

## Propiedades (resúmen):
### Para texto:
- **font-family:** Cambiar la fuente del texto. Generalmente se asigna una triada (Ej: Arial, Helvetica, sans-serif).
- **font-style:** Estilo de la fuente (italic, oblique, etc.)
- **font-weight:** Espesor de la fuente -en negrita- (Ej: bold, bolder o valores de 100 a 900).
- **color:** color del texto.
- **text-align:** Alineación del texto (right -derecha-, left -izquierda, center -centrado-, justify -justificado-)

## Modelo de caja:
- **width:** Ancho del elemento.
- **height:** Altura del elemento.
- **border:** Borde del elemento. Primero el espesor, luego estilo del borde y por último el color (Ej: 1px solid black).
- **background-color:** Color de fondo del elemento.
- **margin:** Separación del elemento con otros elementos (desde el borde para afuera)
- **margin-top**
- **margin-right**
- **margin-bottom**
- **margin-left**
- **padding:** Espacio entre el borde y el contenido del elemento.
- **padding-top**
- **padding-right**
- **padding-bottom**
- **padding-left**
- **box-sizing:**
   - **content-box (por defecto):** el tamaño total del elemento será igual al tamaño asignado por el width y el height más el padding y el espesor del border.
  - **border-box:** el tamaño total del elemento será el determinado por el valor asignado a el width y height, el padding y espesor del border estarán contenidos dentro de esas dimensiones.


## Colores
Los colores en CSS se pueden escribir de tres maneras:
- Nombre del color en inglés (blue, white, black, etc...)
- **Con rgb**(intensidad de rojo, intensidad de verde, intensidad de azul). Los valores de intensidad van del 0 al 255, siendo rgb(255,255,255) el blanco y rgb(0,0,0) el negro.

- **Color hexadecimal** #RRVVAA (R: rojo, V: verde, A: azul) los valores van desde 00 a FF, siendo #FFFFFF el blanco y #000000 el negro.
Ver selector de colores: https://htmlcolorcodes.com/es/

### Colores con transparencia
Los colores que vimos hasta ahora, son colores sólidos.  Pero se pueden aplicar transparencias a éstos de dos formas:

- **Con rgba(rojo,verde,azul, transparencia)**. La transparencia es un valor de 0 a 1 (con decimales), siendo 0 totalmente transparente y 1 color sólido.  Ej: rgba(255,255,255,1) es un color blanco completamente sólido, rgba(255,255,255,0.5) color blanco con una transparencia media y rgba(255,255,255,0) color completamente transparente (no visible).
- **Con hexadecimal #RRVVAATT** siendo TT la transparencia y puede tomar valores de 00 a FF, 00 completamente transparente y FF color sólido.

## Ejemplo 1

En carpeta
```
/Ejemplo_1
----/index.html
----/style.css
```

## Ejemplo 2

En carpeta
```
/Ejemplo_2
----/index.html
----/style.css
```

## Blog
En carpeta
```
/Blog
----/index.html
----/style.css
```
