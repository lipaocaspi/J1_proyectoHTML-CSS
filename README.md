# PROYECTO HTML-CSS

Para este proyecto se crearon 5 archivos de estilos:

* **aboutStyle.css** --> hoja de estilos correspondiente al archivo *about.html*.
* **catalogueStyle.css** --> hoja de estilos correspondiente a los archivos llamados *catalogue.html* ubicados en cada uno de los directorios de categoría ubicados dentro del directorio *pages* .
* **mainProductStyle.css** --> hoja de estilos correspondiente a:
  * *mainProductOne.html*
  * *mainProductTwo.html*
  * *mainProductThree.html*
* **productStyle.css** --> hoja de estilos correspondiente a cada uno de los archivos html cuyo nombre comienza con *product*, los cuales se encuentran ubicados en cada una de los directorios de categoría.
* **style.css** --> hoja de estilos correspondiente al archivo principal *index.html* .



## aboutStyle.css

Al cuerpo del documento se le asigna un color de fondo y una fuente de texto.

```
body {
  font-family: "Kanit", sans-serif;
  background-color: #1e1d2b;
}
```

A un div que tenga la clase *container* se le aplica un relleno del 2% del ancho y alto, según corresponda, del div en todos los lados de este.

```
.container {
    padding: 2%;
}
```

A todos los elementos con etiqueta *p* se les quita el valor de margen por defecto.

```
p {
    margin: 0;
}
```

Todos los textos que tienen la clase *center* se centran.

```
.center {
    text-align: center;
}
```

A todos los textos que tengan la clase *linkTexts* se les quita cualquier decoración por defecto, se centran y se define su tamaño como 1.5rem.

```
.linkTexts {
    text-decoration: none;
    text-align: center;
    font-size: 1.5rem
}
```

A todos los textos que tengan la clase *linkDownTexts* se les quita cualquier decoración por defecto, se define su tamaño como 1.2rem y se les asigna el color blanco.

```
.linkDownTexts {
    text-decoration: none;
    font-size: 1.2rem;
    color: white;
}
```

A todos los textos que tengan la clase *whiteText* se les asigna el color blanco.

```
.whiteText {
    color: white;
}
```

A todos los textos que tengan la clase *blackText* se les asigna el color negro.

```
.blackText {
    color: black;
}
```

A todos los textos que tengan la clase *headerLinks* se les asigna un grosor de 500.

```
.headerLinks {
    font-weight: 500;
}
```

Al pasar el cursor por cualquier texto que tenga la clase *headerLinks* , se aumenta la escala del texto al 110% de su tamaño original, mientras el cursor esté sobre él.

```
.headerLinks:hover {
    transform: scale(1.1);
}
```

A todos los elementos que tengan la clase *icons* se le quita cualquier decoración por defecto.

```
.icons {
    text-decoration: none;
}
```

Se define un diseño de cuadrícula con dos columnas, donde la primera columna ocupa el 20% del ancho y la segunda el 80%. Los elementos dentro de este contenedor se alinean a la derecha en términos de justificación y se centran verticalmente.

```
.nav {
    display: grid;
    grid-template-columns: 20% 80%;
    justify-content: end;
    align-items: center;
}
```

Se define un contenedor flexible con anchura del 100%, y centra tanto horizontal como verticalmente los elementos hijos dentro del contenedor.

```
.logo {
    display: flex;
    width: 100%;
    justify-content: center;
    align-items: center;
}
```

Se define un contenedor flexible que centra horizontal y verticalmente su contenido. Además, se le añade un espacio de relleno del 5% alrededor del contenido y se establece que el contenedor ocupe todo el ancho disponible.

```
.logoMainPage {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 5%;
    width: 100%;
}
```

Se ocultan los elementos con las clases *navTarget* y *closeMenu*, se cambia el cursor a una mano, y se establece un orden de presentación de 1 para ambos elementos en un contenedor flexible.

```
.navTarget, .closeMenu {
    display: none;
    cursor: pointer;
    order: 1;
}
```

Se define un contenedor flexible que alinea sus elementos hijos a la derecha horizontalmente y los centra verticalmente.

```
.menuP {
    display: flex;
    justify-content: end;
    align-items: center;
}
```

Se define el estilo de un enlace *<a>* con la clase *menuA*. Elimina el subrayado, establece el color del texto a blanco, alinea el texto a la derecha, ajusta el peso de la fuente, agrega relleno y aplica una transición suave.

```
.menuA {
    text-decoration: none;
    color: #fff;
    text-align: end;
    font-weight: 500;
    padding: 0px 30px;
    transition: 0.4s;
}
```

A todos los elementos que tengan la clase *titlePage* se le asigna un tamaño de 2.5rem y se centra.

```
.titlePage {
    font-size: 2.5rem;
    text-align: center;
}
```

Se define un contenedor de cuadrícula con dos columnas, cada una ocupando el 50% del ancho del contenedor. Además, se agrega un espacio de relleno de 50 píxeles alrededor del contenido.

```
.box {
    display: grid;
    grid-template-columns: repeat(2, 50%);
    padding: 50px;
}
```

Se asigna un color al fondo del elemento con la clase *background* .

```
.background {
    background-color: #d9d9d9;
}
```

Se define un contenedor flexible que centra tanto horizontal como verticalmente sus elementos hijos.

```
.pictureMain {
    display: flex;
    justify-content: center;
    align-items: center;
}
```

Se aplica a elementos que tengan la clase *picture*, y ajusta su ancho al 50% del contenedor principal.

```
.picture {
    width: 50%;
}
```

Se define un contenedor flexible con dirección de columna, centrando verticalmente sus elementos hijos, justificando el texto y agregando un espacio de relleno alrededor del contenido.

```
.details {
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: justify;
    padding: 10px;
}
```

Se aumenta el tamaño de la fuente de los textos con la clase *desc*.

```
.desc {
    font-size: larger;
}
```

Se define un diseño para un botón con un fondo de color gris oscuro, texto blanco, esquinas redondeadas, y un tamaño y ancho específicos.

```
.contactButton {
    background-color: #3f3e53;
    font-size: 1rem;
    padding: 5px 10px 5px 10px;
    border-radius: 5px;
    color: white;
    width: 150px;
}
```

Se define un diseño para un contenedor con la clase *contact*, con un fondo de color gris oscuro y un espacio de relleno del 5%.

```
.contact {
    background-color: #2c2b47;
    padding: 5%;
}
```

Se define un contenedor de cuadrícula con dos columnas, un espacio entre las filas y columnas del 5%, y un espacio de relleno del 1%.

```
.listContact {
    display: grid;
    grid-template-columns: repeat(2, 50%);
    gap: 5%;
    padding: 1%;
}
```

Se define el aspecto de un título con la clase *titleContact*. Elimina el subrayado, establece el color del texto como blanco, centra el texto, ajusta el tamaño de la fuente y el peso de la fuente.

```
.titleContact {
    text-decoration: none;
    color: white;
    text-align: center;
    font-size: larger;
    font-weight: 600;
    font-size: 1.5rem;
}
```

Se define un elemento horizontal con la clase *hrContact* que tiene un ancho del 30% y un borde sólido gris de 1 píxel.

```
.hrContact {
    width: 30%; 
    border: 1px solid #d9d9d9;
}
```

Se define un espacio de relleno del 4% para los elementos con la clase *links*.

```
.links {
    padding: 4%;
}
```

Al pasar el cursor por cualquier elemento *i* , se aumenta la escala del elemento al 110% de su tamaño original, mientras el cursor esté sobre él.

```
i:hover {
    transform: scale(1.1);
}
```



Las siguientes reglas están relacionadas con el diseño responsivo, por lo que se aplican al momento que el ancho de la pantalla sea igual o menor 840px:



Se define un estilo para elementos con la clase *navTarget*. Los elementos se organizan en una disposición flexbox, se colocan en el extremo derecho del contenedor, se centran verticalmente y tienen un color de texto gris sin decoración de subrayado.

```
@media (max-width :840px) {
    .navTarget {
        display: flex;
        justify-content: end;
        align-items: center;
        color: #d9d9d9;
        font-size: 2rem; 
        text-decoration: none;
    }
    ...
}
```

Se define el estilo para un menú desplegable *menuP*. Cuando el menú está cerrado, se presenta como un círculo que se expande suavemente para revelar su contenido cuando se activa.

```
@media (max-width :840px) {
	...
    .menuP {
        position: fixed;
        width: 80%;
        background: #2c2b47;
        left: 0;
        top: 15%;
        display: flex;
        flex-direction: column;
        padding: 100px;
        z-index: 1;        
        clip-path: circle(0% at top right);
        transition: clip-path 0.4s;
    }
    ...
}
```

Al hacer clic en un enlace que tiene un fragmento de URL que coincide con el *id* de un elemento con la clase *menuP*, se aplica esta regla para cambiar el aspecto del menú, mostrando su contenido.

```
@media (max-width :840px) {
	...
    .menuP:target{
        clip-path: circle(150% at top right);
    }
    ...
}
```

Establece el elemento *<a>* como un bloque y agrega un relleno en todos sus lados.

```
@media (max-width :840px) {
	...
    .menuP a {
        display: block;
        padding: 15px;
    }
    ...
}
```

Se define un estilo para elementos con la clase *closeMenu*. Presenta un texto con un tamaño de fuente grande, en gris, y sin subrayado.

```
@media (max-width :840px) {
	...
    .closeMenu {
        display: flex;
        color: #d9d9d9;
        font-size: 3rem; 
        text-decoration: none;
    }
    ...
}
```

Posiciona un pseudo-elemento después del contenido de los elementos con la clase *closeMenu*.

```
@media (max-width :840px) {
	...
    .closeMenu::after{
        position: absolute;
        top: 0px;
        right: 0px; 
    }
    ...
}
```

Se indica que los elementos con la clase *down* deben tener un diseño de cuadrícula con una única columna que ocupa todo el ancho disponible.

```
@media (max-width :840px) {
	...
    .down {
        grid-template-columns: 100%;
    }
    ...
}
```

Se define un espacio entre las filas y columnas, según corresponda, del 2%.

```
@media (max-width :840px) {
	...
    .gap {
        gap: 2%;
    }
    ...
}
```

Se aplica a elementos que tengan la clase *smallProduct*, y ajusta su ancho al 40% del contenedor principal.

```
@media (max-width :840px) {
	...
    .smallProduct {
        width: 40%;
    }
    ...
}
```

Se especifica un tamaño fijo de 150x150 píxeles para cada elemento con esta clase.

```
@media (max-width :840px) {
	...
    .smallImage {
        width: 150px;
        height: 150px;
    }
}
```

