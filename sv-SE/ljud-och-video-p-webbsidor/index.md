---
title: Ljud och video på webbsidor 
level: Nivå 3
materials: "code and images"
layout: project
---

# Uppgiften {.intro}

Det finns olika sätt att lägga till film eller ljud på din webbsida. Låt oss titta närmare på dem tillsammans.

# Lägg till en film från YouTube {.activity}

Att lägga till filmer från YouTube är jättelätt.

+ Gå till filmsidan på YouTube.
+ Under filmen kan du hitta en knapp det står `Share` på. Klicka på den.
+ För att få fram koden som du kan använda på din hemsida, klicka på `Embed`.

Det kommer se ut ungefär såhär:

```html
<iframe width="560" height="315" src="http://www.youtube.com/embed/FxhGIajRsq4"
   frameborder="0" allowfullscreen></iframe>
```

Just det här fragmentet med kod skulle lägga till en Code Club-film till din webbsida. Det är bara att kopiera och klistra in det på det stället på webbsidan där du vill att filmen ska ligga.

Lägg märke till attributen `width` och `height`. De gör så att du kan bestämma hur stor del av sidan som filmrutan ska täcka, därför kan du ändra dem till de mått som du tycker passar. 

# Lägg till en film från Vimeo. {.activity}

+ Gå till filmsidan på Vimeo.
+ Klicka på `Share`-knappen på filmspelaren.
+ På höger sida finns en Embed-ruta. Klicka på den för att markera koden och kopiera den sedan. Det kommer se ut ungefär såhär:

```html
<iframe src="http://player.vimeo.com/video/44738167" width="600" height="338"
   frameborder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>
```

+ Klistra in koden på det stället på webbsidan där du vill att filmen ska ligga. Lägg märke till `width` och `height` attributen. De gör så att du kan bestämma hur stor del av sidan som filmrutan ska täcka, därför kan du ändra dem till de mått som du tycker passar.

# Lägg till en film från din dator {.activity}

Om du har en film som du själv har spelat in kan du lägga upp den på din hemsida utan att första lägga upp den på YouTube eller Vimeo.

+ För att lägga upp en film på din sida behöver du lägga till en `video`-tagg. Precis som `<img>`-taggen har den ett `src`-attribut som pekar mot filen:

```html
	<video src="spaceship_landing.mp4">
	</video>
```

Tyvärr är det irriterande med att lägga upp en film att inte alla webbläsare kan spela upp alla videoformat. Du behöver spara din egen film i formaten `.mp4` och `.ogv` minst, eftersom att de formaten i alla fall fungerar i de flesta webbläsare.

För att se till att webbläsaren förstår att det finns mer än ett videoformat tillgängligt, skriv så här:

```html
	<video>
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ För att lägga till en bild som visas innan filmen spelas upp kan du använda dig av ett `poster`-attribut:

```html
	<video poster="spaceship_landing.jpg">
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ Om du vill att filmen spelas automatiskt kan du lägga till nyckelordet `autoplay`, såhär:

```html
	<video poster="spaceship_landing.jpg" autoplay>
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ För att visa filmreglagen, som till exempel knapparna för play och volym kan du lägga till nyckelordet `controls`:

```html
	<video poster="spaceship_landing.jpg" controls>
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ Du kan också bestämma storleken på filmen genom att använda `width` och `height` attributen. Skriv såhär:

```html
	<video poster="spaceship_landing.jpg" width="600" height="400">
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

# Lägg till en ljudfil från din dator {.activity}

Så som du lägger upp ljudfiler på din webbsida från din dator är liknande det sättet som använder för att lägga upp filmfiler.

+ För att lägga upp ljudet på en sida, skriv såhär:

```html
	<audio src="spaceship.mp3">
	</audio>
```

Lägg märke till `src`-attributet som pekar mot filen.

Precis som med filmfiler så kan inte alla webbläsare spela upp alla typer av ljudfiler, så för att se till att så många som möjligt ska kunna höra ljudet måste du lägga upp ljudfilen i så många olika format som möjligt, du bör åtminstone lägga upp `.mp3` och `.oga`.

```html
	<audio>
 		<source src="spaceship.mp3" type='audio/mp3'>
 		<source src="spaceship.ogg" type='audio/ogg; codecs=vorbis'>
	</audio>
```

+ För att lägga till reglagen använd dig av nyckelordet `controls`:

```html
	<audio controls>
 		<source src="spaceship.mp3" type='audio/mp3'>
 		<source src="spaceship.ogg" type='audio/ogg; codecs=vorbis'>
	</audio>
```

+ Om du vill att ljudet ska spelas så fort webbsidan har laddat kan du använda nyckelordet `autoplay`, så här:

```html
	<audio controls autoplay>
 		<source src="spaceship.mp3" type='audio/mp3'>
 		<source src="spaceship.ogg" type='audio/ogg; codecs=vorbis'>
	</audio>
```
