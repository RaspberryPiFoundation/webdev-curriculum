---
title: Salas Enlazadas
description: Crea un nuevo proyecto web con varias “habitaciones” unidas.
layout: project
notes: "Linked Rooms - notes.md"
---

# Introducción {.intro}

En este proyecto vamos a crear varias salas enlazadas, cada una de las cuales será una página web diferente que podrás decorar con HTML.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ba5d27ec68?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="rooms-hall-finished.png">
</div>

__Instrucciones__: Haz clic en las puertas para moverte entre las salas.

# Paso 1: Crear un enlace a otra página web en el mismo proyecto {.activity}

Los proyectos web pueden estar formados por un montón de archivos HTML enlazados entre si.

## Lista de tareas de la actividad { .check}

+ Abre este trinket: <a href="http://jumpto.cc/web-rooms" target="_blank">jumpto.cc/web-rooms</a>. Si estás leyendo este proyecto en línea, también puedes usar el siguiente trinket incrustado:

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ef608f0733" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ El trinket debería ejecutarse automáticamente, y tú deberías encontrarte en el vestíbulo:

	![screenshot](images/rooms-hall-start.png)

+ Fíjate en la lista de pestañas de este trinket. ¿Ves la pestaña`tvroom.html`? Haz clic en ella.

	![screenshot](images/rooms-tvroom-html.png)

	Este es otro archivo html dentro del mismo proyecto.


+ Para poder llegar a `tvroom.html` tienes que añadir un enlace en `index.html`.

	Añade el código subrayado al `<div>` que contiene la categoría ("class") `room`:

	![screenshot](images/rooms-link-tvroom.png)

+ Prueba tu trinket haciendo clic en el enlace __Sala TV__ para ver la página web `tvroom.html`.

	Fíjate que `tvroom.html` también tiene su propio archivo de estilo `tvroom.css`, que define el diseño de esta página.

	![screenshot](images/rooms-tvroom-unstyled.png)


##Desafío: Añadir otro enlace {.challenge}

Añade un enlace `<a>` a la página web `tvroom.html` para poder volver a la página web del vestíbulo, que se llama `index.html`. El texto del enlace debería ser 'Vestíbulo'.

Para ello, la página web de la sala de TV debería tener un enlace como este:

![screenshot](images/rooms-hall-link.png)

Asegúrate de comprobar el código. Deberías de poder moverte del vestíbulo a la Sala de TV y volver haciendo clic en los enlaces.  


## Guarda tu proyecto {.save}

# Paso 2: Añadir otra sala {.activity}

Ahora vamos a añadir otra sala, una __Sala de juegos__.

+ Haz clic en el botón de añadir página __+__:

	![screenshot](images/rooms-add-page.png)

	Llama a la nueva página `gamesroom.html`:

  	![screenshot](images/rooms-games-html.png)

+ El HTML para la __Sala de juegos__ es muy parecido al de `tvroom.html`, así que __copia__ el código y __pégalo__ en `gamesroom.html`.

	Modifica los elementos subrayados para que aparezca juegos en lugar de TV:

	![screenshot](images/rooms-games-html2.png)

+ La página `gamesroom.html` está usando `gamesroom.css`, que aún no existe.

	Crea `gamesroom.css` haciendo clic en el botón de añadir página __+__.


+ El CSS de la __Sala de juegos__ es muy parecido al de `tvroom.css`, así que __cópialo__ y __pégalo__ en `gamesroom.css`.

	![screenshot](images/rooms-add-games-css.png)

+ Crea un enlace en el vestíbulo a la Sala de juegos:

	![screenshot](images/rooms-hall-games.png)

+ Prueba tu proyecto haciendo clic en el enlace de la Sala de juegos.

	La __Sala de juegos__ debería de parecerse a esta:

	![screenshot](images/rooms-games-before.png)

	No parece muy interesante, pero podemos arreglarlo en el próximo desafío.

## Guarda tu proyecto {.save}

##Desafío: Dar estilo y enlazar la Sala de juegos {.challenge}

Modifica el HTML y el CSS de la __Sala de juegos__ para que la página web se parezca a esta:

![screenshot](images/rooms-games-challenge.png)

Pista: Tendrás que cambiar el color de fondo, color de fuente y color de borde en `gamesroom.css`. El color verde chillón se llama `chartreuse`.  

Pista: Tendrás que incluir un enlace `<a>` en `gamesroom.html` que lleve a `hall.html`.

## Guarda tu proyecto {.save}

# Paso 3: Haz que los enlaces parezcan puertas {.activity}

Los enlaces no tienen por que ser sólo texto. Vamos a crear una puerta en la que podamos clicar usando un `<div>`.

## Lista de tareas de la actividad { .check}

+ Abre `index.html` y añade un `<div>` alrededor del texto del enlace __Sala TV__. Tiene que estar dentro de la `<a>` para que podamos hacer clic en él.

  Añade `id="vestatv"` para etiquetarlo como la puerta que va del vestíbulo a la Sala TV, y así podamos darle estilo.

  ![screenshot](images/rooms-tvroom-div.png)  

+ Haz clic en la pestaña `style.css`, sitúate en el final de la página y añade el siguiente CSS para cambiar el tamaño y el color la de la puerta:

	![screenshot](images/rooms-door-css1.png)

+ Prueba la página web haciendo clic en cualquier parte de la puerta, no sólo en el texto.

+ Ahora haremos que se parezca más a una puerta añadiendo un marco en tres de sus lados:

	![screenshot](images/rooms-door-css2.png)

+ También añadiremos algo de CSS para hacer que el texto de la puerta sea más atractivo:

	![screenshot](images/rooms-door-css3.png)

+ Seguramente te has dado cuenta de que la puerta está suspendida en el aire. Vamos a arreglarlo situando la puerta dentro de la sala.

	![screenshot](images/rooms-door-position.png)

+ Prueba tu página web haciendo clic en la puerta para entrar en la __Sala TV__.

## Guarda tu proyecto {.save}

##Desafío: ¡Añadir más puertas! {.challenge}

Convierte el resto de enlaces del proyecto en puertas siguiendo el mismo método.

Para cada puerta tendrás que:

+ Modificar el enlace de la puerta para usar un `<div>` con un id, como por ejemplo `vestajuegos`, para que puedas darle estilo.

	Por ejemplo:

	`<a href="gamesroom.html"><div id="vestajuegos">Sala de Juegos</div></a>`

+ Añade CSS al id de la puerta en el archivo `.css` de la habitación. Usa _copiar_ y _pegar_ para ir más rápido. Si quieres, puedes hacer que cada puerta sea diferente.

+ Escoge la posición de la puerta usando `bottom:` (abajo), y `left:` (izquierda) o `right:` (derecha).

El vestíbulo podría parecerse a este:

![screenshot](images/rooms-hall-doors.png)

La sala de TV debería de parecerse a esta:

![screenshot](images/rooms-tvroom-door.png)


# Paso 4: Añadir una imagen de fondo {.activity}

Vamos a decorar el vestíbulo con una imagen de fondo.

## Lista de tareas de la actividad { .check}


+  Modifica `style.css` para añadir una imagen de fondo al vestíbulo:

	![screenshot](images/rooms-hall-decorated.png)

	La imagen se repetirá para cubrir la sala entera.


## Guarda tu proyecto {.save}

##Desafío: Empapelar la Sala de juegos {.challenge}

¿Puedes decorar la sala de juegos con una imagen de fondo?

Puedes usar la imagen de fondo `space-invader.png`, que está incluida en tu proyecto.

Tendrás que:

+ Añadir `background-image:` en el CSS `.room` de la Sala de juegos.

La sala decorada debería de parecerse a esta:

![screenshot](images/rooms-games-finished.png)

## Guarda tu proyecto {.save}

##Desafío: ¡Hazlo tuyo! {.challenge}

Añade más salas a tu proyecto. Recuerda que puedes usar __copiar__ y __pegar__ para ir más rápido, y después cambiar los elementos que tienen que ser diferentes.

Para cada sala tendrás que:

+ Crear un archivo `.html
+ Añadir enlaces en las puertas hacia y desde la nueva 'sala'
+ Crear un archivo `.css` con los estilos para la nueva sala y sus puertas

Puedes cambiar el `background-color:` (color de fondo) de las salas. Haz clic en el icono de imágenes para ver las imágenes de fondo que puedes escoger:

![screenshot](images/rooms-images.png)

## Guarda tu proyecto {.save}
