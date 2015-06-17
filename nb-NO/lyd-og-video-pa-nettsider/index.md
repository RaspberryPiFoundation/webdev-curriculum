---
title: Lyd og video på nettsider
level: Lesson 8
language: nb_NO
embeds: "*.png"
materials: "ressurser"
stylesheet: web
...

# Introduksjon { .intro}

Det finnes flere måter å legge til video eller lyd til sidene dine. La oss ta en nærmere titt på dem sammen.

# Legge til video fra YouTube { .activity}

Å legge til videoer fra YouTube er egentlig ganske enkelt.

+ Gå til siden på YouTube hvor videoen er.
+ Under videospiller kan du finne `Dele`-knappen. Klikk på den.
+ For å få koden du kan bruke på nettsiden din, klikk `Innbygg`.

Det vil se omtrent slik ut:

```
<iframe width="560" height="315" src="http://www.youtube.com/embed/FxhGIajRsq4"
   frameborder="0" allowfullscreen></iframe>
```

Denne spesifikke kodefragment ville legge en CodeClub video til din side. Bare kopier og lim inn koden der du ønsker at videoen skal vises.

Legg merke til `width` (bredde) og `height` (høyde) attributtene. De lar deg kontrollere hvor stor videoen vil være på siden, så du kan gjerne endre dem.


# Add a video from Vimeo. { .activity}

+ Gå til en videoside på Vimeo.
+ Klikk på `Dele`-knappen på videospilleren.
+ På høyre side er det en `embedd` boks. Klikk på den for å velge koden og kopiere den. Det vil se litt ut som dette:

```
<iframe src="http://player.vimeo.com/video/44738167" width="600" height="338"
   frameborder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>
```

+ Bare kopier og lim inn koden der du ønsker at videoen skal vises. Legg merke til `width` (bredde) og `height` (høyde) attributtene. De lar deg kontrollere hvor stor videoen vil være på siden, så du kan gjerne endre dem.

# Legg til en videofil fra datamaskinen {.activity}

Hvis du har en video du har laget, kan du legge den på siden din uten å måtte laste det opp til YouTube eller Vimeo.

+ For å plassere en video på siden din må du legge til en `video` tag. Akkurat som `<img>` taggen peker `src` attributtet til filen:

```
	<video src="spaceship_landing.mp4">
	</video>
```

Dessverre kan ikke alle nettlesere spille alle videoformater. Du blir nødt til å lagre den i minst `.mp4` og `.ogv` formater, som vil fungere i de fleste nettlesere.

For å la nettleseren vite at vi har mer enn ett format av video klar, skriver vi slik:

```
	<video>
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ For å legge inn et bilde som vil bli sett før videoen spilles av, kan du bruke en `poster` (plakat) attributt:

```
	<video poster="spaceship_landing.jpg">
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ Hvis du ønsker å spille av videoen automatisk, kan du legge til `autoplay` atributt, slik som dette:

```
	<video poster="spaceship_landing.jpg" autoplay>
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ For å vise video kontroller, som spill knapp, volum kontroll osv, kan du legge til `controls` atributt.

```
	<video poster="spaceship_landing.jpg" controls>
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ Du kan også kontrollere størrelsen på videon med `width` (bredde) og `height` (høyde) attributer. Skriv:

```
	<video poster="spaceship_landing.jpg" width="600" height="400">
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

# Legg til en lydfil fra datamaskinen {.activity}

Måten å legge lydfiler til siden din fra datamaskinen din er omtrent som med videofil.

+ For å plassere lyden på siden, skirv dette:

```
	<audio src="spaceship.mp3">
	</audio>
```

Legg merke til `src` atributtet som peker til filen.

Akkurat som med video, kan ikke alle nettlesere spille hver type lydfil, så for å sørge for at så mange som mulig kan høre lyden du har til å legge filen i mer enn ett format, i hvert fall i `.mp3` og `.oga`.

```
	<audio>
 		<source src="spaceship.mp3" type='audio/mp3'>
 		<source src="spaceship.ogg" type='audio/ogg; codecs=vorbis'>
	</audio>
```

+ For å legge til kontrollene trenger du å legge til `controls` nøkkelordet:

```
	<audio controls>
 		<source src="spaceship.mp3" type='audio/mp3'>
 		<source src="spaceship.ogg" type='audio/ogg; codecs=vorbis'>
	</audio>
```

+ Hvis du vil at lyden skal spille så snart som siden lastes, kan du legge den `autoplay` nøkkelord, slik som dette:

```
	<audio controls autoplay>
 		<source src="spaceship.mp3" type='audio/mp3'>
 		<source src="spaceship.ogg" type='audio/ogg; codecs=vorbis'>
	</audio>
```
