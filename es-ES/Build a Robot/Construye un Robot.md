---
title: Construye un Robot
level: HTML & CSS 1
language: es-ES
embeds: "*.png"
materials: ["Recursos para el líder del Club/*.*","Recursos del Proyecto/*.*"]
stylesheet: web
...

# Introducción { .intro}

En este proyecto, aprenderás a cómo posicionar imágenes para crear tu propio robot.

![screenshot](robot-final.png)

# Paso 1: Poniendo ojos a tu robot { .activity}

¡Pongamos ojos al robot!

## Lista de Tareas de la Actividad { .check}

+ Abre este *trinket*: <a href="https://trinket.io/html/c14fcb3f4c" target="\_blank">jumpto.cc/web-robot</a>. Si dispones de conexión a Internet también puedes utilizar la versión insertada a continuación.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/b29b50e571" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ Cada imagen en este proyecto tiene su propio nombre (o __id__). Por ejemplo, el código HTML para las imágenes de la cara y los ojos (‘cara’, ‘ojos1’ y ‘ojos2’, a partir de la línea 8 del código) es como se muestra a continuación:

```
<img id="cara" ...>
<img id="ojos1" ...>
<img id="ojos2" ...>
```

+ Puedes utilizar el _id_ de cada imagen para darle su propio estilo utilizando el símbolo `#`, conocido como almohadilla. Esto te permitirá dar un estilo distinto a cada imagen.

Haz clic en el archivo `estilo.css`. ¿Notas que el tamaño de la cara del robot y las demás imágenes son distintos?

![screenshot](robot-id.png)

+ Añade este código CSS para cambiar la apariencia de los ojos del robot:

```
#ojos1 {
    width: 200px;
}
```

Fíjate que sólo estás cambiando el estilo de la imagen `ojos1` ya que has usado el selector `#ojos1` en tu CSS. Si lo prefieres puedes probar qué pasa si usas `#ojos2` u `#ojos3` en vez de `#ojos1` en tu CSS.

![screenshot](robot-eyes-width.png)

+ ¿Ves cómo cada imagen se muestra una después de la otra? Esto es lo que llamamos posicionamiento relativo, y para definirlo usaremos el atributo CSS __position: relative__. Si quieres indicar al explorador exactamente dónde quieres poner los ojos del robot, deberás usar posicionamiento absoluto, para ello tendrás que usar la propiedad __position: absolute__ en vez de __relative__.

Añade estas tres líneas de código al CSS que utilizamos para definir las propiedades de la imagen `ojos1`:

```
position: absolute;
top: 200px;
left: 100px;
```

Una vez hayas añadido estas líneas deberías ver cómo los ojos del robot se mueven al lugar correcto.

![screenshot](robot-eyes-position.png)

Este código CSS dice al explorador a qué distancia desde arriba (top) o desde la izquierda (left) de la página web tiene que estar la imagen.

![screenshot](robot-eyes-position2.png)

Puedes usar `bottom`, debajo en inglés, en vez de `top` para decirle al explorador a qué distancia desde debajo de la web tiene que estar la imágen. De la misma manera puedes usar `right` para indicar la distancia desde la derecha en vez de `left`.

# Paso 2: Poniendo boca a tu robot { .activity}

¡Hagamos que el robot tenga boca!

## Lista de Tareas de la Actividad { .check}

+ Añade el siguiente código CSS para empezar a cambiar el estilo de la imagen con id `mouth1`:

```
#boca1 {
    width: 50px;
    position: absolute;
    top: 200px;
    left: 200px;
}
```

+ La boca del robot parece demasiado pequeña, y no está donde debería estar.

![screenshot](robot-mouth.png)

¿Puedes arreglarlo cambiando el código CSS?

## Guarda tu Proyecto {.save}

##Reto: Diseña tu propio robot {.challenge}
Utiliza lo que has aprendido para terminar de diseñar tu propio robot. Aquí hay algunos ejemplos de cómo puede ser tu robot:

![screenshot](robot-examples.png)

## Guarda tu Proyecto {.save}

##Reto: Añade tus propias imágenes {.challenge}
¿Eres capaz de encontrar imágenes adicionales que añadir al robot y posicionarlas en la página? ¡Puedes incluso cambiar la cara del robot con la tuya propia!

```
<img id="cara" src="miCara.png">
```

## Guarda tu Proyecto {.save}
