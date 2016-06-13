---
title: Amanecer — Notas para los líderes del Club
language: es-MX
embeds: "*.png"
materials: [""]
...

#Introducción:
En este proyecto, los niños aprenderán como hacer una simple escena de animación usando CSS. Usarán la regla @keyframes de CSS para animar varirias propiedades de imagenes y divs.

#Recursos Online

Recomendamos usar [trinket](https://trinket.io/) para realizar páginas online usando HTML y CSS. Este proyecto contiene los siguientes *trinkets*:

+ ['Sunrise' starting point](https://trinket.io/html/web-sunrise)

También hay disponible un *trinket* que contiene una solución de ejemplo a los ejercicios:

+ ['Sunrise' Finished](https://trinket.io/html/abcc0284a3)

#Recursos Offline
Este proyecto puede ser [completado offline](https://www.codeclubprojects.org/en-GB/resources/webdev-working-offline/) (enlace en inglés) si se prefiere o no se dispone de una conexión a Internet. Puedes acceder a los recursos del proyecto haciendo clic en el enlace 'Materiales del Proyecto'. Este enlace contiene una sección de 'Recursos del Proyecto', la cual incluye los recursos que el niño necesitará para complar este proyecto aunque no disponga de conexión a Internet. Asegúrese de que cada niño tiene acceso a una copia de estos recursos. Esta sección contiene los siguientes archivos:

+ template/index.html
+ template/prefix.js
+ template/style.css
+ sunrise/index.html
+ sunrise/style.css
+ sunrise/prefixfree.js
+ sunrise/boat.png
+ sunrise/cloud.png
+ sunrise/helicopter.png
+ sunrise/rainbow.png
+ sunrise/sun.png

También puedes encontrar una versión terminada de los ejercicios de ste proyecto en la sección 'Recursos para el Voluntario', que contiene los siguientes archivos:

+ index.html
+ style.css
+ prefixfree.js
+ boat.png
+ sun.png
+ rainbow.png

#Objetivos de aprendizaje
+ Estilo y animación con CSS:
	+ Introducción a reglas `@keyframes` para definir los pasos en una animación.
	+ Reforzar el uso de propiedades para definir el tamaño, forma, posición y color de los elementos en una página web.

#Retos
+ "Animación en diagonal" - editar las propiedades de la animación `@keyframe` para usar left:;
+ "Mejorar el cielo" - agregar mas keyframes y editar el background (fondo):.
+ "Mas animación" - animar mas imágenes o elementos usando una variedad de propiedades de CSS. 

#Preguntas frecuentes.

+ Este pro hace uso de la librería de javascript `prefixfree.js`, para permitir la compatibilidad de animación entre browsers (Navegadores). si esta librería no es usada, entonces los niños usando navegadores viejos necesitarán declarar una animación para su navegador, por ejemplo:

```
animation: sky 10s infinite; 		  	//for all newer browsers
-webkit-animation: sky 10s infinite;  	// For Webkit browsers(Chrome, Safari...)
-moz-animation: sky 10s infinite;     	// For Mozilla browsers
-o-animation: sky 10s infinite;       	// For Opera browsers
-ms-animation: sky 10s infinite;		// For Microsoft browsers 
```
