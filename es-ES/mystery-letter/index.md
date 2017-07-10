--
title: Carta Misteriosa
description: Create a mystery letter with lots of different styles.
layout: project
notes: "Mystery Letter - notes.md"
---

# Introducción {.intro}

En este proyecto vas a crear una carta misteriosa, en la que parezca que cada palabra se ha recortado de diferentes periódicos, revistas, cómics u otras fuentes. 

![screenshot](letter-final.png)

# Paso 1: Escoge tu mensaje {.activity}

Las cartas misteriosas se usan en películas y libros para enviar mensajes secretos. 

## Lista de tareas de la actividad { .check}

+ Piensa un mensaje misterioso. Una longitud adecuada para el mensaje sería de 12 palabras. Si no se te ocurre ningún mensaje, puedes usar este ejemplo: 'Tu próxima pista está en la caja fuerte. El código es 65536.'

+ Apunta el mensaje o recuérdalo. 

# Paso 2: Editar tu mensaje {.activity}

Vamos a publicar tu mensaje en una página web.

## Lista de tareas de la actividad { .check}

+ Abre este trinket: <a href="http://jumpto.cc/web-letter" target="_blank">jumpto.cc/web-letter</a>. Si estás leyendo este proyecto online, también puedes usar la versión incrustada de Trinket que encontrarás a continuación.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/b5fbcf112e" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ La etiqueta de párrafo `<p>` se explica en el proyecto 'Feliz cumpleaños'. La etiqueta `<span>` se usa para agrupar unidades más pequeñas de texto dentro de un párrafo y poderles dar estilo. 

![screenshot](letter-placeholder.png)

## Lista de tareas de la actividad { .check}

+ Cambia las palabras por las de tu mensaje, poniendo una palabra en cada `<span>`. Tendrás que añadir o eliminar etiquetas de `<span>` si tu mensaje tiene una longitud diferente. 

![screenshot](letter-message.png)

## Lista de tareas de la actividad { .check}

+ Haz clic en el botón "Run" para probar tu trinket.

	Si te fijas en las palabras, verás que ha cambiado su estilo para que parezca que han sido pegadas en la página.

# Paso 3: Usar estilos Class {.activity}

## Lista de tareas de la actividad { .check}

+ ¿Te has fijado en el texto `class=""` (significa "categoría") que está en las etiquetas `<span>`? Puedes usarlo para dar el mismo estilo a más de una cosa. 

+ Añade la categoría `magazine1` a algunas de tus etiquetas `<span>` y prueba tu página web.

![screenshot](letter-magazine1.png)

## Lista de tareas de la actividad { .check}

+ Puedes añadir más de una categoría a un elemento. Sólo tienes que dejar un espacio entre las dos. Añade la categoría `big` a una de tus etiquetas `<span>`. Prueba tu página web. 

![screenshot](letter-big.png)

## Guarda tu proyecto {.save}

## Reto: Cambiar el estilo de tu mensaje {.challenge}

Usa los estilos que te indicamos a continuación para hacer que tu mensaje parezca una carta misteriosa. 

Añade estas categorías a tus etiquetas `<span>`: 

+ `newspaper` (periódico), `magazine1` (revista1), `magazine2` (revista2)

+ `medium` (medio), `big` (grande), `reallybig` (muy grande)

+ `rotateleft` (rotar izquierda), `rotateright` (rotar derecha)

+ `skewleft` (inclinar izquierda), `skewright` (inclinar derecha)

No añadas más de una categoría de cada línea a un `<span>` en concreto.

Tu carta debería de parecerse a ésta:

![screenshot](letter-challenge1.png)

## Guarda tu proyecto {.save}

# Paso 4: Editar las categorías  {.activity}

## Lista de tareas de la actividad { .check}

+ Haz clic en la pestaña __'style.css'__. Busca el estilo de la categoría de CSS `newspaper` que has estado usando.

![screenshot](letter-newspaper.png)

+ Fíjate que hay un punto '.' antes del nombre de la categoría en el archivo de CSS, pero no en la etiqueta `<span>` de tu documento HTML.

+ Ahora busca las otras categorías de CSS que has usado para dar estilo a tu carta misteriosa. Intenta encontrar:

	+ Cómo el estilo `magazine1` cambia todo el texto a mayúsculas ("text-transform" significa transformar texto).

	+ Cómo el estilo `magazine2` coloca una imagen por detrás del texto ("background-image" significa imagen de fondo). 

![screenshot](letter-magazines.png)

+ ¿Qué pasa si cambias la imagen de fondo (`background-image`) de `magazine2` a `canvas.png`? Si te gusta más `pink-pattern.png`, puedes volver a dejarlo como estaba. 

También puedes cambiar los colores en los estilos magazine, si quieres.

+ Busca el CSS que se usa para rotar (rotate) e inclinar (skew) tus palabras:

![screenshot](letter-rotate-skew.png)

Intenta cambiar los valores para crear diferentes efectos y después prueba tu página. 

# Paso 5: Crear una nueva categoría {.activity}

Vamos a crear un estilo que parezca que ha sido recortado de un cómic. <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> ofrece un montón de fuentes que son de uso libre. 

## Lista de tareas de la actividad { .check}

+ Añade una categoría de `comic` en el archivo __style.css__. Después de `magazine2` es un buen sitio. No te olvides de poner un punto delante del nombre de la categoría. 

![screenshot](letter-comic1.png)

No te preocupes si te aparece un mensaje diciendo 'The Rule is empty' (La regla está vacía), arreglaremos eso enseguida. 

+ Ahora añade algo de CSS a la categoría de CSS comic. Si quieres, puedes usar diferentes colores. Puedes encontrar una lista con un montón de colores en <a href="http://jumpto.cc/web-colours" target="_blank">jumpto.cc/web-colours</a>.

![screenshot](letter-comic2.png)

+ Usa el estilo comic en algunas de las etiquetas `<span>` de tu documento HTML y prueba tu página:

![screenshot](letter-comic-output.png)

+ Ahora puedes añadir un tipo de letra divertido. Abre una nueva pestaña o ventana en el navegador. Ve a <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> y busca __'bangers'__:

![screenshot](letter-fonts1.png)

+ Haz clic en el botón de "Quick-use" (Uso rápido):

![screenshot](letter-fonts2.png)

+ Entonces se cargará una nueva página. Desplázate hacia abajo en la pantalla hasta que veas:

![screenshot](letter-fonts-link.png)

y copia el código marcado. 

+ Pega el código del `<enlace>` que acabas de copiar de Google fonts en la `<cabecera>` de tu página web:

![screenshot](letter-fonts-head.png)


Esto te permitirá usar el tipo de letra Bangers en tu página web. 

+ Vuelve a Google fonts, desplázate aún más hacia abajo en la pantalla, y copia el código del tipo de letra ("font-family"):

![screenshot](letter-fonts-bangers.png)

+ A continuación vuelve a tu archivo __'style.css'__ en trinket y pega el código del tipo de letra en el estilo comic:

![screenshot](letter-fonts-comic.png)

+ Prueba tu página web. El resultado debería de parecerse a éste: 

![screenshot](letter-fonts-output.png)

## Guarda tu proyecto {.save}

## Reto: Crear un estilo de impresión de ordenador {.challenge}

Crea un estilo que imite una impresión de ordenador a la antigua, y aplícalo a algunas de las palabras:

![screenshot](letter-fonts-printout.png)

Necesitarás:

+ El tipo de letra `VT323` de <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a>. Revisa el paso 5 si no recuerdas cómo usar Google fonts. 

+ La imagen de fondo `computer-printout-paper.png`. Revisa el paso 4 si necesitas recordar cómo usar las imágenes de fondo. 	

## Reto: Crear tus propios estilos {.challenge}

Crea tus propios estilos de categoría y haz que tu carta misteriosa sea aún más interesante. Usa el CSS que has aprendido en proyectos anteriores y fíjate en los ejemplos que hay en __style.css__, como nuevas ideas. 

Aquí tienes un ejemplo:

![screenshot](letter-fonts-challenge3.png)

Puedes ver las imágenes que hay disponibles en trinket, si haces clic en la pestaña "Images".
Intenta establecer fondos de imagen usando una de las imágenes incluidas: 

+ `rough-paper.png`

+ `canvas.png`

Si tienes una cuenta de trinket, puedes cargar tus propias imágenes, como hiciste en el proyecto 'Cuenta una historia'. 

Busca tipos de letra que te gusten en <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> y copia su `<enlace>` y código CSS en tu trinket para poder usarlos. 

## Guarda tu proyecto {.save}

## Community Contributed Translation { .challenge .pdf-hidden }

This project was translated by Montse Verdaguer. Our amazing translation volunteers help us give children around the world the chance to learn to code.  You can help us reach more children by translating a Code Club project via [Github](https://github.com/CodeClub/curriculum_documentation/blob/master/contributing.md) or by getting in touch with us at hello@codeclubworld.

