# CSS: Animaciones

## Gradientes

- Linear gradient
- Radial gradiente
```css
.box{
    width: 100px;
    height: 100px;
    margin: 15px;
}
.linear-gradient {
    background: rgb(111,83,212);
    background: linear-gradient(90deg, rgba(111,83,212,1) 0%, rgba(205,76,211,1) 50%, rgba(38,167,209,1) 100%);
}

.radial-gradient{
    background: rgb(111,83,212);
    background: radial-gradient(circle, rgba(111,83,212,1) 0%, rgba(205,76,211,1) 50%, rgba(38,167,209,1) 100%);
}

```
## Z-index

**IMPORTANTE!!** : el elemento debe estar posicionado para que esta propiedad tenga efecto.

```css

.z-box1{
    position: relative;
    background-color: lightblue;
    z-index: 1; /* es NECESARIO que el elemento esté posicionado */
}

.z-box2{
    position: relative;
    bottom: 50px;
    left: 20px;
    background-color: lightcoral;
    z-index: 0;
}

```
## Pseudoclases

Una pseudoclase CSS es una palabra clave que se añade a los selectores y que especifica un estado especial del elemento seleccionado. Por ejemplo,  **:hover** aplicará un estilo cuando el usuario haga hover sobre el elemento especificado por el selector.

Otras pseudoclases importantes:
- :active
- :hover
- :focus
- :checked

[**Ver más...**](https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-classes)

```css

.box1{
    background-color: lightgreen;
}

.box1:hover{
    border: 5px solid black;
    background-color: brown;
}

```

## Pseudo-elementos
Al igual que las pseudo-classes, los pseudo-elementos se añaden a los selectores, pero en cambio, no describen un estado especial sino que, permiten añadir estilos a una parte concreta del documento.

```css
.parrafo{
    font-family: 'Courier New', Courier, monospace;
}

.parrafo::before{
    content: "Antes ";
    color: red;
    font-weight: bolder;
}

.parrafo::after{
    content: "Despues";
    color: blue;
    font-weight: bolder;
}

.icono-flecha::before{
    content: url(https://cdn.iconscout.com/icon/free/png-64/right-arrow-1965038-1660431.png);
    
}
```

## Transitions
La propiedad transition es una propiedad abreviada de transition-property, transition-duration, transition-timing-function, y transition-delay. Permite definir la transición entre dos estados de un elemento. Hay diferentes estados que pueden ser definidos utilizando pseudo-clases como :hover o :active.


```css
.transition-box{
    background-color: green;
    transition: all 0.5s linear;
}

.transition-box:hover{
    background-color: red;
}

.box-scale{
    background-color: lightseagreen;
    transform: scale(0.5);

}

.box-rotate{
    background-color: lightcoral;
    transform: rotate(25deg);
}

.box-translate{
    background-color: red;
    transform: translate(20px, 15px);
}

.box-skew{
    background-color: lightseagreen;
    transform: skew(15deg, 15deg);
}


.box-mix{
    background-color: lightseagreen;
    transform: translate(200px) rotate(30deg) ;
}


.rotate-transition{
    border: 1px solid black;
    background-color: aquamarine;
    transition: all 0.5s linear;
}

.rotate-transition:hover{
    transform: rotate(45deg);
}

.translate-transition1{
    background-color: blue;
    transition: all 1s linear;
}

.translate-transition1:hover{
    transform: translateX(300px);
}

.translate-transition2{
    background-color: red;
    transition: all 1s ease-in;

}

.translate-transition2:hover{
    transform: translateX(300px);
}

.translate-transition3{
    transition: all 1s ease-out;
    background-color: green;
}
.translate-transition3:hover{
    transform: translateX(300px);
    transition: all 1s ease-in;

}

.translate-transition4{
    background-color: yellow;
    transition: all 1s ease-in-out;

}
.translate-transition4:hover{
    transform: translateX(300px);
}
```

## Animation - @keyframes

```css
.animation-box{
    background-color: aquamarine;
    animation: desplazamiento 2s ease-in-out infinite;
}

@keyframes desplazamiento{
    50%{
        transform: translateX(250px);
    }
}

```