---
title: Sunrise
level: HTML & CSS 2
language: es-MX
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# Introducción { .intro}

En este proyecto, aprenderas como usar CSS para crear un amanecer animado.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/abcc0284a3?outputOnly=true&start=result" width="600" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="sunrise-final.png">
</div>

# Paso 1: Creando el Sol { .activity}

Empecemos agregando una imagen del sol y posicionándolo con CSS.

## Lista de actividades { .check}

+ Arbir este trinket: <a href="http://jumpto.cc/web-sunrise" target="_blank">jumpto.cc/web-sunrise</a>. Si estas viendo esto online, también puedes usar la version incrustada de este trinket de abajo.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/5085f92143" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ Ver dentro del `body` de tu archivo `index.html` y encontrarás los elementos `div` para el cielo y el mar.

    ```
    <div id="sky">
    </div>
    
    <div id="sea">
    </div>
    ```
+ Se ha incluido una imagen del sol en este proyecto.. 

	Agregar la imagen del sol dentro del `div` incluyendo un id para que puedas aplicarle estilo.:

    ![screenshot](sunrise-sun-image.png)

+ Huy, la imagen es enorme. Ve a `style.css` y agrega el CSS para aplicarle altura a la imagen:

    ![screenshot](sunrise-sun-height.png)

	Nota que el ancho es actualizado automáticament para mantener las proporciones iguales.

+ Finalmente, agreguemos algo de codigo para posicionar el sol:

    ![screenshot](sunrise-sun-position.png)


## Guarda tu proyecto {.save}

# Paso 2: Animando el amanecer { .activity}

Para animar el amanecer, necesitas definir como se mueve el sol y el tiempo que se necesita para levantarse.

Para hacer esto define una lista de __key frames__. Cada key frame define las propiedades CSS de un elemento en un punto particular de la animación. 

## Lista de actividades { .check}

+ Primer, necesitas usar `@keyframes` para crear una animación llamada amanecer (sunrise). 

    Agregar este codigo CSS al final de tu archivo `style.css`:

    ```
    @keyframes sunrise {
        0% {top: 90%;}
        100% {top: 0;}
    }
    ```

	Este código le dice al sol donde posicionarse al inicio (`0%`) y al final (`100%`) de la animación.

	Proque el sol está dentro del `div` sky, las posiciones `top`(arriba) y `left`(izquierda) estan dentro del sky(cielo), con `top: 100%` siendo el fondo del cielo, no de la página.

+ Ahora que has creado una animación de amancer `sunrise`, solo necesitas decierle al solo que la use! 

    Agregar el código destacado al CSS de tu sol:

    ![screenshot](sunrise-sunrise.png)

    Esto le dice al sol que tarde 10 segundos en animar el amancer.
	
+ Para volver a correr de nuevo el Trinket, has click en **Autorun**. 

## Guarda tu proyecto {.save}

##Reto: Animació Diagonal{.challenge}
Puedes agrefar código a tu animación `sunrise`(amancer)para hacer que tu sol empiece abajo a la izquierda del cielo y moverlo diagonalmente a su posición aproximadamente arriba el centro?

Puedes usar la propiedad `left` para hacer esto, por ejemplo:

```
left: 40%;
```

![screenshot](sunrise-left.png)

## Guarda tu proyecto {.save}


# Paso 3: Animación infinita { .activity}

Hagamos una animación que se repita parasiempre.

## Lista de actividades { .check}

+ Si quieres que el sol salga y luego se ponga,  solo necesitas agregar mas keyframes a tu animación:

    ```
    @keyframes sunrise {
        0%   {top:90%; left:0;}
        33%  {top:0; left:40%; }
        66%  {top:0; left:40%; }
        100% {top:90%; left:80%; }
    }
    ```
	Esto significa que la animación empieza y termina con el sol al fondo del cielo, y se queda en la parte superior desde el 33% hasta el 66% de la animación.
  
+ Ahora solo tienes que agregar la palabra `infinito` a la animación para hacerla un ciclo parasiempre:

    ![screenshot](sunrise-infinite.png)
  
+ Prueba tu animación. El sol se mantiene saliendo y se poniéndose? 


## Guarda tu proyecto {.save}

# Paso 4: Animando el Cielo { .activity}

La animación no solo es acerca del movimiento. Vamos a animar el cielo para que se oscurezca en la noche.

## Lista de actividades { .check}

+ Agregar una animación llamada `sky` a tu CSS:

    ```
    @keyframes sky {
        0% {background: black}
        100% {background: lightblue}
    }
    ```
	Nota que esta vez estás animando el color del cielo, y no la posición.

+ Agregar el código a tu cielo, para decirle que use la nueva animación:

    ```
    animation: sky 10s;
    ```

    ![screenshot](sunrise-sky.png)

+ Dar Click en **Autorun** para probar tu animación. 

## Guarda tu proyecto {.save}

##Reto: Mejora el cielo {.challenge}

Puedes cambiar la animación del cielo para emparejar con el sol y se quede azul durante el día y regrese a negro cuando el sol se oculte? Hazlo un ciclo infinito también.

![screenshot](sunrise-sky-challenge.png)

##Reto: Mas animación {.challenge}

Puedes animar otra imágen? Puedes animar su posición, color, forma, tamaño y opacidad(ver atravez de ella) o  cualquier otra cosa que se te ocurra, Prueba también cambiar la duración de tus animaciones.

Para cada elemento que quieras animar, necesitaras:

+ Incluirlo en tu HTML con un Id
+ Agregar un estilo (style) para ese ID
+ crear una regla @keyframes
+ Usar `animation:` en el stilo para usar la animaci que definiste con @keyframes 

Dar click en ícono para ver las imagenes que son incluidas en tu proyecto:

![screenshot](sunrise-images.png)

Puedes también subir tus propias imágenes si gustas.

No olvides que puedes poner elementos en el mar asi como en el cielo:

![screenshot](sunrise-boat.png)


En el ejemplo el arcoiris usa opacity(opacidad) para dar un efecto de desvanecimiento:

```
@keyframes fade {
  0%   {opacity: 0;}
  50%  {opacity: 100;}
  66%  {opacity: 0;}
  100%   {opacity: 0;}
}
```

El bote usa una posición de inicion negativa para que no lo puedas ver por una parate de la animación:

```
 @keyframes left-right {
  0%    {left:-50%;}
  100%  {left:200%;}
}
```

## Guarda tu proyecto {.save}
