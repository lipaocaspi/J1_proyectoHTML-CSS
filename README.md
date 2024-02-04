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



### aboutStyle.css

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