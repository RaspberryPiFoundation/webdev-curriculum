---
title: Styling og formatering av tekst
level: Lesson 5
language: nb-NO
embeds: "*.png"
materials: "ressurser"
stylesheet: web
---

## __Introduksjon:__ { .intro }
I denne seksjonen skal vi lære hvordan man kan style tekst med forskjellige skrifttyper, farger og størrelser. Vi vil også lære hvordan du legger til bakgrunnsfarger og pyntekanter. Vi skal bruke det samme prosjektet du jobbet med sist gang, så sørg for at du åpner index.html i Felix mappen.

#Steg 1: Skrifttyper { .activity}

Vi kan endre utseendet på teksten ved å endre __skrifttypen__ ("font" på englesk). De mest vanlige skrifttypene heter:

* Arial
* Courier New, Courier
* Garamond
* Georgia
* Lucida Sans, Lucida Grande, Lucida
* Palatino Linotype
* Tahoma
* Times New Roman, Times
* Trebuchet
* Verdana

Ikke alle skrifttyper finnes på alle datamaskiner, så vi trenger å oppgi en  __fall-back font__ (en skrifttype vi kan falle tilbake på om førstevalget vårt ikke finnes på datamaskinen) også. Disse er ganske generiske som "sans serif", "serif".

La oss prøve å endre skrifttype på overskriften ved hjelp av `font-family`-egenskapen.

```css
h1 {
	color: red;
	background-color:black;
	font-size:72px;
	text-transform:uppercase;
	text-decoration:underline;
	text-decoration:blink;
	font-family:impact, sans-serif;
}
```
Og skriften i avsnittene...

```css
p {
	font-family:georgia, 'times new roman', serif;
}
```

## __LAGRE__ filen og se på den i nettleseren {.save}

Prøv noen av de forskjellige skrifttypene for å se hvilken du liker best. Legg merke til hvordan vi skiller mellom hver skrifttype med et komma, og hvis skrifttypen har et navn med mer enn ett ord trenger vi å sette det i anførselstegn.

Hvilken av skrifttypene vi nevnte tror du ser best ut? Hvilken tror du er lettest å lese?

Har du andre skrifttyper på datamaskinen enn de som er nevnt? (det har du sannsynligvis). Prøv å åpne et program som Word eller Pages, alle skrifttypene som er lagret på datamaskinen kan vanligvis finnes der.

![screenshot](fonts.png)

Finn en skrifttype du liker og prøv den på websiden!

Du kan gjøre teksten __fet__, *kursiv* eller begge deler med `font-style`. La oss endre email teksten (husk den er inni en `<a>`-tag).

```css
a {
	font-style:bold;
}
```

## __LAGRE__ filen og se på den i nettlerseren {.save}

Teksten har blitt fet! La oss se hvordan den ser ut i kursiv. Kursiv på engelsk er `italic`.

```css
a {
	font-style:italic;
}
```
## __LAGRE__ filen og se på den i nettlerseren {.save}

Det finnes også en `font-style`-verdi som heter ‘oblique’. Hvordan ser den ut?

Vi kan til og med si hvor fet en tekst skal være ved å bruke egenskapen `font-weight`. Den tar verdiene `normal`, `bold`, `bolder` og `lighter`. Du kan også bruke tall, 100, 200, 300, 400, 500, 600, 700, 800 og 900, hvor 100 er den tynneste teksten og 900 er den tykkeste. Normal tekst er det samme som 400 og "bold" er det samme som 700. Men ikke alle skrifttypene har alle disse, så det er tryggere å bare bruke normal og bold. Overskrifter er normalt bold som standard. Hvis vi ikke ønsker at `h2`-overskiften vår skal være fet, må vi skrive:

```css
h2 {
	font-weight:normal;
}
```

Prøv da vel!

#Steg 2: Pyntekanter! {.activity}

La oss legge til en ramme rundt bildet:

```css
img {
	border-color:green;
	border-width:5px;
	border-style:solid;
}
```
## __LAGRE__ filen og se på den i nettlerseren {.save}

Prøv å endre fargen (`border-color`), bredden (`border-width`) og pyntekanten (`border-style`) til du er fornøyd. Noen verdier for `border-style` er `dashed`, `dotted`, `double`, `groove`, `ridge`, `inset` og `outset`.

Du kan sette kanter rundt alle typer elementer, hvorfor ikke prøve noen flere.

#Steg 3: IDer og klasser {.activity}

Vi ønsker å __utheve__ kontakt-avsnittet. Vi kan ikke bruke `<p>`-taggen fordi det vil endre alle avsnittene. For å gjøre slik at en stil gjelder bare for ett element, bruker vi noe som kalles ID. Vi trenger å redigere HTML-filen slik:

```html
<p id ="uthevet">Har du sett Felix? <em>Vennligst</em> kontakt eieren hans på <a href="mailto:eierentilfelix@email.com">eierentilfelix@email.com</a</p>
```
så kan vi style den IDen som så:

```css
#uthevet {
	color:red;
}
```
## __LAGRE__ filen og se på den i nettlerseren {.save}
En ID er unik og kan bare brukes én gang per side. Så hva hvis vi ønsket at to av avsnittene skal ha en større tekststørrelse? Vi kan gjøre det ved hjelp av klasser. Først må vi gi klassenavn til de avsnittene vi ønsker å endre.

```html
<p class="stor">Han forvant fra hagen i går.</p>
<p class="stor"><strong>Takk!</strong><p>
```
Vi styler en klasse sånn (med en `.` i stedet for `#`):

```css
.stor {
	font-size:24px;
}
```

## Ting du kan prøve {.try}

+ Hvordan ville du endret siden slik at den ser bedre ut? Hvorfor ikke prøve å bruke dine favorittfonter, farger osv.
+ Hvis du er tidlig ferdig kan du style sidene vi lagde i tidligere leksjoner.
+ Forresten, visste du at `background`-egenskapen ikke bare tar verdier som er farger, men også bilder?
