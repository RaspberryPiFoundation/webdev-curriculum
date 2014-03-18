---
title: Styling og formatering av tekst
level: Lesson 5
language: nb-NO
embeds: "*.png"
materials: "ressurser"
stylesheet: web
...

## __Introduksjon:__ { .intro }
I denne sesjonen skal vi lære hvordan man kan style tekst med forskjellige skrifttyper, farger og størrelser. Vi vil også lære hvordan du legger til bakgrunnsfarger og pyntekanter. Vi skal bruke det samme prosjektet du jobbet med sist gang, så sørg for at du åpner index.html fra Felix mappen.

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

Ikke alle skrifttyper finnes på alle datamaskiner, så vi trenger å gi __fall-back font__ også. Disse er ganske generiske som "sans serif", "serif". 

La oss prøve å endre skrifttype på overskriften ved hjelp av `font-family` egenskapen.

```CSS
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

```CSS
p {
	font-family:georgia, 'times new roman', serif;
}
```

## __LAGRE__ filen og se på den i nettlerseren {.save}

Prøv noen av de forskjellige skrifttypene for å se hvilke du liker best. Legg merke til hvordan vi skiller mellom hver font med et komma, og hvis skriften har et navn med mer enn ett ord trenger vi å sette det i anførselstegn. 

Hvilke av skriftene vi nevnte tror du ser best ut? Hvilken tror du er lettest å lese? 

Har du andre skrifter på datamaskinen enn de som er nevnt? (det har du sannsynligvis). Prøv å åpne et program som Word eller Pages, alle skrifter som er lagret på datamaskinen kan vanligvis finnes der.

![screenshot](fonts.png)

Finn en skrift du liker å prøv den på websiden!

Du kan gjøre teksten __fet__, *kursiv* eller begge deler med `font-style`. La oss endre email teksten (husk den er inne i en `<a>` tag). 

```CSS
a {
	font-style:bold;
}
```

## __LAGRE__ filen og se på den i nettlerseren {.save}

Teksten har blitt fet! La oss se hvordan den ser ut i kursiv. Kursiv på engelsk er `italic`.

```CSS
a {
	font-style:italic;
}
```
## __LAGRE__ filen og se på den i nettlerseren {.save}

Det finnes også en `font-style` verdi som heter ‘oblique’. Hvordan ser den ut?

Vi kan til og med si hvor fet tekst bør bruke eiendommen `font-weight`. Det tar verdiene `normal`, `bold`, `bolder`, `lighter`. Du kan også bruke tall, 100, 200, 300, 400, 500, 600, 700, 800 og 900, hvor 100 er den tynneste teksten og 900 er den tykkeste. Normal tekst er det samme som 400, "bold" er det samme som 700. Men ikke alle skriftene har alle disse, så det er tryggere å bare bruke normal og bold. Overskrifter er normalt bold som standard. Hvis vi ønsket `h2` overskiften vår å ikke være fet, må vi skrive:

```CSS
h2 {
	font-weight:normal;
}
```

Prøv da vel!

#Steg 2: Pyntekanter! {.activity}

La oss legge til en ramme rundt bildet

```CSS
img {
	border-color:green;
	border-width:5px;
	border-style:solid;
}
```
## __LAGRE__ filen og se på den i nettlerseren {.save}

Prøv å endre fargen (`border-color`), bredden (`border-width`) og pyntekanten `border-style` til du er fornøyd. Noen verdier for `border-syle` er `dashed`, `dotted`, `double`, `groove`, `ridge`, `inset`, `outset`. 

Du kan sette kanter rundt alle typer elementer, hvorfor ikke prøve noen flere.

#Steg 3: IDer og klasser {.activity}

We want to make the contact paragraph __highlighted__.  We can’t use the `<p>` tag because that would change all the paragraphs. To make a style apply only to one element, we use something called IDs. We need to edit the html to this:

Vi ønsker å utheve kontakt-avsnittet. Vi kan ikke bruke `<p>` taggen fordi det ville endre alle avsnittene. For å gjøre slik at en stil gjelder bare for ett element, bruker vi noe som kalles ID. Vi trenger å redigere html filen til dette:

```html
<p id ="uthevet">Har du sett Felix? <em>Vennligst</em> kontakt eieren hans på <a href="mailto:eierentilfelix@email.com">eierentilfelix@email.com</a</p>
```
så kan vi style den IDen som så:

```CSS
#uthevet {
	color:red;
}
```
## __LAGRE__ filen og se på den i nettlerseren {.save}
En ID er unik og kan bare brukes én gang per side. Så hva hvis vi ønsket at to av avsnittene har en større font-størrelse? Vi kan gjøre det ved hjelp av klasser. Først må vi gi klassenavn til de avsnittene vi ønsker å endre.

```HTML
<p class="stor">Han forvant fra hagen i går.</p>
<p class="stor"><strong>Takk!</strong><p>
```
we styler en klasse som dette (med en `.` istedet for `#`):

```CSS
.stor {
	font-size:24px;
}
```

## Ting du kan prøve {.try}

+ Hvordan ville du endre siden slik at den ser bedre ut? Hvorfor ikke prøve å bruke dine favoritt fonter, farger osv. 
+ Hvis du er ferdig tidlig kan du gå designe sider vi gjorde i tidligere leksjoner. 
+ Forresten, visste du at `background` egenskapen ikke bare tar verdier som er farger, men også bilder?
