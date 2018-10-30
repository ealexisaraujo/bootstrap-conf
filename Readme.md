# Bootstrap 4

Clase 4
## ¿Qué es un Framework Frontend?
- También conocidos como Frameworks CSS

Son una base para empezar un proyecto web permitiendo **flexibilidad en el diseño**

**Organización y estructura** de nuestros __HTML, CSS Y JavaScript__

### ¿Qué trae un framework frontend? 

Ahorrar mucho tiempo, Componentes visuales, Responsive design, el código anda. 
- Grilla
- Estilos para las fuentes
- Componentes visuales pre-armados

### Algunos Frameworks Fron-End
- Bootstrap
- Fundation
- Bulma
- Flexbox Grid


Clase 5

## Nuestro Proyecto: Hola Mundo de Bootstrap

Vamos al sitio web oficial de Bootstrap en getbootstrap.com . Existen 2 formas para utiliza bootstrap:
~~~
1. Mediante el **CDN**: En este primer ejemplo se copia la plantilla de inicio que, contiene la referencia a los css y a 3 archivos javascript. Dentro de los cJS están:
- - a. La referencia a JQuery (Sí, utiliza JQuery para las funciones que css, por obvias razones no podría implementar)
- - b. Referencia a Popper.JS: Esta herramienta nos sirve para crear los popUps (esos mensajes flotantes que se muestran al posicionar el cursor en un lugar predeterminado)
- - c. Finalmente llama al JS de bootstrap.

Por otro lado, noten que cada referencia contiene un .min dentro de sus nombres (por ejemplo; bootstrap.min.css, …jquery-3.3.1.slim.min.js, etc) que no es más que la versión minificada(sin espacios) de
cada archivo de código.

2. Descargando todos los archivos comprimidos:
- - Otra de las opciones es descargando todos los archivos que componen Bootstrap, esta opción es interesante ya que te permite trabajar sin conexión a internet, cosa que no puedes hacer con laa opción anterior.
~~~
Al abrir la pagina nos dirigimos a el boton **Get started**, pinchamos y nos dirijimos a el apartado __Starter template__ y copiamos toda la plantilla de __HTML5__

```
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
  </body>
</html>
```

Clase 6

## La grilla de Bootstrap

### Containers 

Los contenedores son el elemento de diseño más básico en Bootstrap y son **necesarios al usar nuestro sistema de grillas predeterminado** . Elija entre un contenedor receptivo de ancho fijo (es decir, sus max-widthcambios en cada punto de interrupción) o ancho de fluido (lo que significa que es 100%amplio todo el tiempo).

Mientras que los contenedores se pueden anidar, la mayoría de los diseños no requieren un contenedor anidado.

- conteiner
```
<div class="container">
  <!-- Nuestro contenido acá -->
</div>
```
- .container-fluid

Se usa .container-fluidpara un contenedor de ancho completo, que abarca todo el ancho de la ventana gráfica.
```
<div class="container-fluid">
  <!-- Nuestro contenido acá -->
</div>
```
### Grid
El sistema de grillas de Bootstrap usa una serie de contenedores, filas y columnas para diseñar y alinear el contenido. Está construido con flexbox y responde completamente. A continuación se muestra un ejemplo y una mirada en profundidad sobre cómo se junta la grilla.
```
<div class="container">
  <div class="row">
    <div class="col">
      Una columna aquí
    </div>
    <div class="col">
      Una columna aquí
    </div>
    <div class="col">
      Una columna aquí
    </div>
  </div>
</div>
```
El ejemplo anterior crea tres columnas de ancho igual en dispositivos pequeños, medianos, grandes y extra grandes usando nuestras clases de grillas predefinidas. Esas columnas están centradas en la página con el padre __.container__.
```
<div class="container">
  <div class="row">
    <div class="col">
      Una columna aquí
    </div>
    <div class="col">
      Una columna aquí
</div>
</div>
    <div class="col">
      Una columna aquí
    </div>
    <div class="col">
      Una columna aquí
    </div>
    <div class="col">
      Una columna aquí
    </div>
  </div>
</div>
```
Se agrega un estilo arriba de la etiqueta title
```
<style>
        .col { //columna
            border: 1px solid rebeccapurple; //borde de un 1px y color como morado
        }
    </style>
```
## Reto : Las grillas de Bootstrap
- retogrilla.html
- retogrilla1.html
- retogrilla2.html

Clase 9
## El footer
Vamos a crear el footer de nuestro website. 
Se creo
- index.css

Se añadio la etiqueta footer 
https://getbootstrap.com/docs/4.1/components/card/#header-and-footer

Practica de grilla de bootstrap

## El header de nuestro sitio
Conocemos el componente de Navbar de Bootstrap para crear el encabezado de nuestro website. Conoce más de su manejo en https://getbootstrap.com/docs/4.1/components/navbar/ 

### ¿Qué colocar dentro del Navbar?
- **.navbar-brand** para el nombre de tu compañía,
producto o proyecto
- **.navbar-nav** para un menú de navegación (que puede
tener sub-menúes)
- **.navbar-toggler** para usar con el plugin para colapsar
contenido
- **.form-inline** para incluir formularios
- **.navbar-text** para incluir texto centrado verticalmente
- **.collapse.navbar-collapse** para agrupar contenido
que se va a colapsar

Se agrega carpeta "assets/images"
- platzi-logo.png

Clase 10
## Creando carausel de imagenes

El carousel nos permite ver un conjunto de imágenes y mostrarlas de manera automática. Encuentra más información en https://getbootstrap.com/docs/4.1/components/carousel/

- Hay que agregar la clase **.active** a
alguno de los slides
- Asegurarse de que los controles e
indicadores tengan un atributo
elements **data-target** que coincida
con el id del elemento **.carousel**.

Se agrego img para vista

Clase 11
## Agregando texto informativo del evento

Ahora vamos a incluir un texto informativo sobre nuestro carousel de imágenes.

Cambiamos el id __CarouselExampleFade por carousel__  y agregamos al final de esta clase un nuveo div con la clase __overly__ 

clase 12
## Agregando botones
Encuentra más información de los botones en https://getbootstrap.com/docs/4.1/components/buttons/

Se pone dos formas de poner boton por la etiqueta a o por button con sus respectivas clases

Clase 12 
## Las cards de Bootstrap 4

Conoceremos el feature de Cards de Bootstrap. Para más información consulta: https://getbootstrap.com/docs/4.1/components/card/. 
 
 <--conferensistas-->

 Clase 13
 ## Pastillas de Texto
 Insignias
Documentación y ejemplos de insignias, nuestro pequeño componente de conteo y etiquetado.
https://getbootstrap.com/docs/4.1/components/badge/

Clase 14
## Pastillas de texto
Se acomodaron y agregaron las famosas pastillas en el index

Clase 15
## Agregando un contenedor de ancho completo
https://getbootstrap.com/docs/4.1/layout/overview/#containers
Contenedor fluido
<--Lugar y fecha-->
Aprendimos a utilizar contenedor de ancho fluido y seguimos trabajando con la grilla para diferentes dispositivos

Clase16
## Formulario de bootstrap 4
https://getbootstrap.com/docs/4.1/components/forms/

<--Conviertete en Conferensistas-->

clase 17
## Agregando un tooltip
En esta clase aprenderemos a incluir abreviaciones, que es un componente que le permite al visitante de tu página tener una definición inmediata de una palabra. Para más información checa este website: https://getbootstrap.com/docs/4.1/content/typography/#abbreviations y también agregaremos tooltips un plugin de jQuery que ya viene incluído en Bootstrap: https://getbootstrap.com/docs/4.1/components/tooltips/
Reto: Incorpora otro tooltip en tu sitio.
```
<abbr title="attribute">attr</abbr>
```


clase 18
## Scrollspy: Conociendo la ubicación del usuario en el header
El scrollspy le permite al usuario conocer la posición dentro del sitio. Revisa más sobre este componente en: https://getbootstrap.com/docs/4.1/components/scrollspy/


clase 19
## Agregando un modal para comprar tickets
En esta clase aprenderemos sobre los modals, que son básicamente mostrar un mensaje en una ventana emergente. Conoce más sobre los modals aquí: https://getbootstrap.com/docs/4.1/components/modal/

ojo con esto
````
data-toggle="modal" data-target="#modalCompra"
```

Clase 20
## Agregar formulario de compra

se agrega formulario y un alert!

### cargar modal dinamico con php y mysql 
https://programacion.net/articulo/como_cargar_contenido_dinamico_en_un_modal_de_bootstrap_1867
