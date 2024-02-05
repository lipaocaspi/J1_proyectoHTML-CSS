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

Se define el estilo de un enlace *a* con la clase *menuA*. Elimina el subrayado, establece el color del texto a blanco, alinea el texto a la derecha, ajusta el peso de la fuente, agrega relleno y aplica una transición suave.

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

Establece el elemento *a* como un bloque y agrega un relleno en todos sus lados.

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



## catalogueStyle.css

**Nota** : algunos estilos de esta hoja ya han sido explicados anteriormente, por lo que serán omitidos.

Da un estilo específico a los elementos con la clase *mark*, asegurando que tengan un fondo gris y un texto oscuro, y que esta regla tenga precedencia sobre otras reglas que podrían afectar esos estilos.

```
.mark {
    background-color: #d9d9d9;
    color: #1e1d2b!important;
}
```

Se establece el tamaño de la fuente en 1.5 rem.

```
.font15 {
    font-size: 1.5rem;
}
```

Si el contenido es más grande que el contenedor, se mostrará una barra de desplazamiento para permitir al usuario desplazarse y ver el contenido oculto.

```
.menuC {
    overflow: auto;
    width: 100%;
}
```

Oculta los elementos con la clase *headerC*.

```
.headerC {
    display: none
}
```

Se ocultan los elementos con las clases *menuHam* *navTarget* y *closeMenu*, se cambia el cursor a una mano, y se establece un orden de presentación de 1 para los elementos en un contenedor.

```
.menuHam, .navTarget, .closeMenu {
    display: none;
    cursor: pointer;
    order: 1;
}
```

Se define un contenedor flexible, y centra tanto horizontal como verticalmente los elementos hijos dentro del contenedor.

```
.catalogueTitle {
    display: flex;
    align-items: center;
    justify-content: center;
}
```

Estiliza y controla el tamaño y el desbordamiento de un menú desplegable.

```
.menuHam{
    width: 300px;
    height: 200px;
    overflow-y: hidden;
    overflow-x: hidden;
    background-color:#2c2b47;
    overflow-y: visible;
}
```

Elimina márgenes y rellenos predeterminados de las listas desordenadas. El margen a la izquierda de 5 píxeles puede proporcionar un espacio visual entre el borde izquierdo del contenedor padre y la lista.

```
ul {
    margin: 0;
    padding: 0;
    margin-left: 5px;
}
```

Se eliminan las viñetas.

```
li {
    list-style-type: none;
}
```

Elimina el subrayado de los enlaces dentro de la lista.

```
li > a {
    text-decoration: none;
}
```

Diseña y estructura un contenedor, organizando el contenido en dos columnas (60% y 40%) y aplicando estilos de borde y color de fondo.

```
.productDetails {
    display: grid;
    grid-template-columns: 60% 40%;
    background-color: #d9d9d9;
    border-radius: 5px;
    border: 2px solid;
    padding: 10px;
}
```

Crea un diseño de cuadrícula con dos columnas y cuatro filas, con márgenes exteriores y dimensiones específicas.

```
.pictureColumns {
    margin: 20px;
    display: grid;
    grid-template-columns: 15% 80%;
    grid-template-rows: repeat(4, 1fr);
    gap: 15px;
    width: 90%;
    height: 80%;
}
```

Asegura que las imágenes dentro de elementos con la clase *pictureColumns* ocupen todo su contenedor y tengan un cursor interactivo al pasar el ratón sobre ellas.

```
.pictureColumns img {
    width: 100%;
    height: 100%;
    cursor: pointer;
}
```

Establece un borde sólido de 2 píxeles alrededor de estos elementos.

```
.vista1, .vista2, .vista3, .vista4 {
    border: 2px solid;
}
```

Cambia la imagen de fondo y el ancho del elemento *pictureMain* cuando el elemento *vista1* está en estado de *:hover*.

```
.pictureColumns > .vista1:hover ~ .pictureMain {
    background: url('./../images/bx-sushi.svg') no-repeat center;
    background-size: cover;
    width: 100%;
}
```

Cambia la imagen de fondo y el ancho del elemento *pictureMain* cuando el elemento *vista2* está en estado de *:hover*.

```
.pictureColumns > .vista2:hover ~ .pictureMain {
    background: url('./../images/bx-sushi.svg') no-repeat center;
    background-size: cover;
    width: 100%;
}
```

Cambia la imagen de fondo y el ancho del elemento *pictureMain* cuando el elemento *vista3* está en estado de *:hover*.

```
.pictureColumns > .vista3:hover ~ .pictureMain {
    background: url('./../images/bx-sushi.svg') no-repeat center;
    background-size: cover;
    width: 100%;
}
```

Cambia la imagen de fondo y el ancho del elemento *pictureMain* cuando el elemento *vista4* está en estado de *:hover*.

```
.pictureColumns > .vista4:hover ~ .pictureMain {
    background: url('./../images/bx-sushi.svg') no-repeat center;
    background-size: cover;
    width: 100%;
}
```

Estiliza y posiciona el elemento *pictureMain* en una cuadrícula que tiene dos columnas, con una imagen de fondo específica.

```
.pictureMain {
    background: url('./../images/camisa.png') no-repeat center;
    background-size: contain;
    width: 100%;
    padding: 0;
    border: 2px solid;
    margin: 10px;
    grid-column: 2;
    grid-row: 1 / span 4;
}
```

Define el contenedor como un contenedor flexible, con dirección de columna, sus elementos centrados verticalmente y un relleno en píxeles.

```
.details {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 10px 25px 10px;
}
```

Se define un diseño para un botón con un fondo de color gris oscuro, texto blanco, esquinas redondeadas, y un ancho específicos.

```
.buyButton {
    background-color: #3f3e53;
    width: 100px;
    font-size: 1rem;
    padding: 5px 10px 5px 10px;
    border-radius: 5px;
    color: white;
}
```

Las siguientes reglas están relacionadas con el diseño responsivo, por lo que se aplican al momento que el ancho de la pantalla sea igual o menor 840px:



Se ocultan el elemento con la clase *menuC* .

```
@media (max-width :840px) {
    .menuC {
        display: none;
    }
	...
}
```

Se muestran los elementos de la clase *headerC* como una cuadrícula.

```
@media (max-width :840px) {
	...
    .headerC {
        display: grid;
    }
    ...
}
```

Se define un estilo para elementos con la clase *navTarget*. Los elementos se organizan en una disposición flexbox, se colocan en el extremo izquierdo del contenedor, se centran verticalmente y tienen un color de texto gris sin decoración de subrayado.

```
@media (max-width :840px) {
    ...
    .navTarget {
        display: flex;
        justify-content: start;
        align-items: center;
        color: #d9d9d9;
        font-size: 2rem; 
        text-decoration: none;
    }
    ...
}
```

Se define el estilo para un menú desplegable *menuHam*. Cuando el menú está cerrado, se presenta como un círculo que se expande suavemente para revelar su contenido cuando se activa.

```
@media (max-width :840px) {
    ...
    .menuHam {
        position: fixed;
        width: 80%;
        background: #2c2b47;
        left: 20px;
        top: 20%;
        display: flex;
        flex-direction: column;
        padding: 5px 10px 25px 25px;
        z-index: 1;        
        clip-path: circle(0% at top left);
        transition: clip-path 0.4s;
        overflow: auto;
    }
    ...
}
```

Al hacer clic en un enlace que tiene un fragmento de URL que coincide con el *id* de un elemento con la clase *menuHam*, se aplica esta regla para cambiar el aspecto del menú, mostrando su contenido.

```
@media (max-width :840px) {
	...
	.menuHam:target {
        clip-path: circle(150% at top left);
    }
	...
}
```

Establece el elemento *ul* como un bloque y agrega un relleno en todos sus lados.

```
@media (max-width :840px) {
	...
	.menuHam ul {
        display: block;
        padding: 15px;
    }
}
```



## mainProductStyle.css

**Nota** : algunos estilos de esta hoja ya han sido explicados anteriormente, por lo que serán omitidos.

Cambia el color del texto de los elementos con la clase *textColor* al tono de gris claro especificado.

```
.textColor {
    color: #d9d9d9;
}
```

Cambia el tamaño de fuente de los elementos con la clase *font20* a 20 píxeles.

```
.font20 {
    font-size: 20px;
}
```

Cambia el peso de la fuente de los elementos con la clase *font500* a 500.

```
.font500 {
    font-weight: 500;
}
```

Cambia el tamaño de fuente de los elementos con la clase *font2* a 2rem.

```
.font2 {
    font-size: 2rem;
}
```

Crea una estructura de encabezado con dos secciones: una que ocupa el 20% del ancho y otra que ocupa el 80% del ancho.

```
.header {
    display: grid;
    grid-template-columns: 20% 80%;
}
```

Estiliza un texto, cambiando su tamaño, posición y color.

```
.close {
    display: flex;
    justify-content: end;
    text-decoration: none;
    color: white;
    font-size: 4rem;
}
```

Crea una estructura con dos secciones: una que ocupa el 60% del ancho y otra que ocupa el 40% del ancho.

```
.pictureDetails {
    display: grid;
    grid-template-columns: 60% 40%;
    padding: 5%;
}
```

Crea un contenedor flexible centrado tanto vertical como horizontalmente, con un fondo gris claro y esquinas ligeramente redondeadas.

```
.picture {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #d9d9d9;
    width: 100%;
    border-radius: 1%;
}
```

Establece que el elemento ocupe el 75% del ancho de su contenedor principal.

```
.pictureContent {
    width: 75%;
}
```

Agrega un relleno del 10% alrededor de su contenido.

```
.mainDetails {
    padding: 10%;
}
```

Estiliza un botón con un fondo gris claro, texto negro, esquinas redondeadas y un tamaño de fuente de 1.5 rem.

```
.buyButton {
    background-color: #d9d9d9;
    font-size: 1.5rem;
    padding: 10px 20px 10px 20px;
    border-radius: 5px;
    color: black;
}
```

Organiza el contenido de los elementos con la clase *details* en una columna y agrega un pequeño relleno alrededor de ese contenido.

```
.details {
    display: flex;
    flex-direction: column;
    padding: 2%;
}
```

Agrega espacio alrededor del contenido del elemento con la clase *reviews*, proporcionando un relleno más amplio en los lados derecho e izquierdo y un relleno más estrecho en la parte superior e inferior.

```
.reviews {
    padding: 1% 5% 1% 5%;
}
```



## productStyles.css

**Nota** : algunos estilos de esta hoja ya han sido explicados anteriormente, por lo que serán omitidos.

Organiza y alinea los elementos secundarios en la clase *header* en una cuadrícula, con los elementos alineados hacia el extremo derecho de esa cuadrícula.

```
.header {
    display: grid;
    justify-content: end;
}
```

Estiliza los elementos con la clase *close* como texto sin subrayado, con color blanco y un tamaño de fuente grande.

```
.close {
    text-decoration: none;
    color: white;
    font-size: 4rem;
}
```

Estiliza los elementos con la clase *productDetails* como un contenedor de cuadrícula con una sola columna que ocupa el 100% del ancho, con un fondo gris, bordes redondeados y relleno.

```
.productDetails {
    display: grid;
    grid-template-columns: 100%;
    background-color: #d9d9d9;
    border-radius: 5px;
    border: 2px solid;
    padding: 10px;
}
```

Estiliza los elementos con la clase *pictureMain* como un contenedor flexible centrado tanto vertical como horizontalmente, con un relleno, un borde y un margen.

```
.pictureMain {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 10px;
    border: 2px solid;
    margin: 10px;
}
```

Limita el ancho de los elementos con la clase *picture* a 200 píxeles.

```
.picture {
    width: 200px;
}
```

Estiliza los elementos con la clase *details* como un contenedor flexible con dirección de columna, centrando los elementos verticalmente y agregando un relleno específico alrededor del contenido.

```
.details {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 10px 25px 10px;
}
```

Crea un diseño de cuadrícula para los elementos con la clase *registroCantidad*, dividiendo el espacio en dos columnas, una que ocupa el 75% y otra el 25%, con un espacio de separación del 1% entre ellas.

```
.registroCantidad {
    display: grid;
    grid-template-columns: 75% 25%;
    gap: 1%;
}
```

Se define un diseño para un botón con un fondo de color gris oscuro, texto blanco, esquinas redondeadas, y un ancho del 100%.

```
.buyButton {
    background-color: #3f3e53;
    font-size: 1rem;
    padding: 5px 10px 5px 10px;
    border-radius: 5px;
    color: white;
    width: 100%;
}
```



## style.css

**Nota** : algunos estilos de esta hoja ya han sido explicados anteriormente, por lo que serán omitidos.

Se define un contenedor de cuadrícula centrado verticalmente con una imagen de fondo que cubre el contenedor y márgenes específicos en cada lado.

```
.ad {
    display: grid;
    align-items: center;
    background-size: cover;
    margin: 5% 3% 5% 3%;
}
```

Estiliza imágenes, asegurándose de que ocupen todo el ancho disponible y tengan esquinas ligeramente redondeadas.

```
.adImage {
    width: 100%;
    border-radius: 1%;
}
```

Estiliza subtítulos, haciéndolos más grandes, centrados y con un color de texto blanco.

```
.subtitleMainPage {
    text-decoration: none;
    color: white;
    text-align: center;
    font-size: larger;
    font-weight: 600;
    font-size: 2rem;
}
```

Organiza los elementos con la clase *mainProducts* en una cuadrícula de tres columnas, centrando los elementos tanto vertical como horizontalmente en cada celda de la cuadrícula y agregando un espacio de relleno del 2%.

```
.mainProducts {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    align-items: center;
    justify-content: center;
    place-items: center;
    padding: 2%;
}
```

Crea un contenedor con estilo para los elementos con la clase *mainProduct*. El contenedor es flexible, centrando su contenido tanto horizontal como verticalmente, con un fondo de color gris claro, esquinas redondeadas y un ancho del 80%.

```
.mainProduct {
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    background-color: #d9d9d9;
    border-radius: 5%;
    padding: 20px 0px 20px 0px;
    width: 80%;
}
```

A todos los textos que tengan la clase *titleProduct* se centran y se define su tamaño como 15 píxeles.

```
.titleProduct {
    font-size: 15px; 
    text-align: center;
}
```

Aplica estilos específicos, como dimensiones, ajuste de contenido y relleno, a los elementos con la clase *mainProductImage*.

```
.mainProductImage {
    width: 200px;
    height: 200px;
    object-fit: cover;
    padding: 10px;
}
```

Al pasar el cursor por cualquier elemento que tenga la clase *mainProduct* , se aumenta la escala de mismo al 110% de su tamaño original, además de que su color cambia a blanco, mientras el cursor esté sobre él.

```
.mainProduct:hover {
    background-color: white;
    transform: scale(1.1);
}
```

Las siguientes reglas están relacionadas con el diseño responsivo, por lo que se aplican al momento que el ancho de la pantalla sea igual o menor 840px:



Establece el tamaño de la fuente del texto dentro de los elementos con la clase *descProduct* a 15 píxeles.

```
@media (max-width :840px) {
	...
	.descProduct {
        font-size: 15px;
    }
}
```
