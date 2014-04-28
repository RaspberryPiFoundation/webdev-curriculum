---
title: the web
level: Lesson 1
language: nb_NO
embeds: "*.png"
materials: "ressurser"
stylesheet: web
...

# Introduksjon { .intro}

Har du noen gang lurt på hvordan internett virker? Klart du har det! Idag kommer du til å lære hvordan man lager nettsider slik at du også kan hjelpe til med å bygge det. Nettsider blir skrevet ved å bruke __HTML__, som er en forkortelse for __HyperText Markup Language__ på engelsk. Du kommer til å finne ut mer om dette ettersom du bygger siden din.

# Steg 1: Hva er nettsider? { .activity}

## Aktiviteter { .check}

1. Åpne et __tekstprogram__.
2. Lag et nytt dokument.
3. Skriv noe! For eksempel: `Hei! Jeg heter …`
4. Lagre filen. Kall den `hei.txt`.
5. Nå kan du finne filen din og prøve å åpne den. Den åpnes i et tekstprogram, og det er jo ikke så gøy.
6. Endre filtypen i filnavnet (det som kommer etter punktumet) til `.html`, sånn at filen nå heter `hei.html`.
7. Åpne filen på nytt.

Hvilket program ble filen åpnet i denne gangen? Nettleseren er et spesielt program som vet hvordan man skal tolke tekstfiler som er skrevet ved hjelp av __HTML språket__. Vi har ikke laget noe __HTML__ enda, vi bare la inn litt tekst, men det bryr ikke nettleseren seg noe om! Så lenge du gir den en `.html` fil, kommer den til å gjøre sitt beste for å vise deg hva som er i filen.

Dette er veldig nyttig: selv når en nettside inneholder feil, vil nettleseren prøve å finne ut av hvordan den skal vise den fram uansett.

__Hvordan kan vi se disse filene?__

Når du skriver en adresse inn i nettleseren din, blir forespørselen din sendt avgårde til en datamaskin som alltid står på og er innstilt for å la deg se nettsidene som lever inni den. Denne datamaskinen kalles en server. Når den mottar en forespørsel fra din datamaskin, ser den etter alle de nødvendige filene, som for eksempel `.html`-filen, og sender deg den sammen med alt det andre nettsiden trenger, for eksempel bilder og videoer.

// diagram som viser hvordan nettet fungerer - på toppen burde det stå: Kan jeg få denne siden takk? Og på bunnen: Her, værsågod

# Steg 2: Hva er HTML? { .activity}

HTML er et __markeringsspråk__ - det betyr at det brukes til å beskrive hva ting er.

Selv om nettleseren prøver å gjøre sitt beste for å vise ting, hjelper det at den vet hva disse tingene er.

For å fortelle nettleseren det, bruker vi `tagger`.

Tagger ser sånn ut:
`<p>Dette er litt tekst.</p>`

`<p>` er en forkortelse for __paragraf__.

Den har en åpnings-tag, som er denne:
`<p>`
og en tilsvarende avslutnings-tag, med skråstrek:
`</p>`
Nettleseren vet da at alt imellom de to taggene er en paragraf med tekst.

Tagger kan også ha attributter, som er nyttig informasjon om elementet.

La oss kikke på link-taggen:
`<a href="http://kodeklubben.no/">Besøk nettsiden til Kodeklubben</a>`
`<a>` betyr __anker__, som er det linker ble kalt før.

Den har åpnings-taggen:
`<a>`
og avslutnings-taggen:
`</a>`
men vi la til en attributt til åpnings-taggen:
`<a href="http://kodeklubben.no/">`
`href` er attributten, og `http://kodeklubben.no/` er attributten sin verdi.
`href` står for _hypertekst referanse_. En tekst som linket til andre tekster ble en gang kalt _hypertekst_, fordi den kunne ha bilder og lyd, og kunne linke videre til andre tekster. Det gjorde den til litt annerledes enn annen vanlig tekst.
`href` forteller nettleseren hvor linken skal føre deg, og teksten imellom taggene vil bli synlig som en link.

## Aktiviteter { .check}

1. Åpne filen `side.html`.
2. Spør den frivillige om du kan bruke X-Ray Goggles eller utvikler-verktøyene for å se på koden (en utvikler er en som lager ting med kode).

#### Hvis du kan bruke X-Ray Goggles:
3. Klikk på X-Ray Goggles-bokmerket.
4. Beveg musen rundt på siden. Da kan du se deler av siden lyse opp, og se hvilke tagger delene er laget av. Så kan du trykke på hver boks for å se kode-snutten som boksen er laget av.

#### Hvis du bruker utvikler-verktøyene:
3. Beveg musen rundt på siden. Høyreklikk på noe interessant, og trykk så på `Inspiser element`. Da vil det åpne seg et panel som vil vise deg koden til siden samtidig som du kan se på siden.
4. Beveg musen over forskjellige deler av koden. Når du har musepilen over en del av koden, vil du se at den delen av siden som er laget av den koden blir lyst opp, slik at du kan se hvilken kodesnutt som gjør hva.
5. Prøv å inspiser flere deler av siden. Da finner du masse forskjellige tagger:

Vi kan allerede `<p>` og `<a>`.
`<ol>` - sortert liste
`<ul>` - usortert liste
`<li>` - et punkt i en liste
`<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>` - overskrifter
`<hr>` - horisontal linje
`<div>` - en boks for å gruppere ting
`<img>` - dette er et litt spesielt element, fordi i motsetning til de fleste andre elementer så har ikke dette en avslutnings-tagg. Vi bruker det til å sette inn bilder på siden.

Det finnes også noen tagger som vi alltid må ha med i HTML dokumenter:
`<html>` - forteller nettleseren at her kommer det HTML-kode
`<head>` - inne i `<head>` skriver vi ting som kan være nyttig for nettleseren, men som ikke vil dukke opp som tekst på selve siden. I dette eksempelet har vi satt en `<title>`-tagg her, og det som er inni den vil dukke opp i toppen av nettleser-vinduet.
`<body>` - her putter vi det vi vil skal dukke opp på siden.

## Aktiviteter { .check}

+ Legg merke til hvordan tagger kan stå på innsiden av andre tagger. Vi har `<a>` taggen, som er inni `<p>` taggen, som igjen er inni `<div>`, som er plassert i `<body>`.

Når det skjer sier vi at taggen som er på innsiden er _barnet_ og taggen som er på utsiden er en __forelder__. Det er nesten som et slektstre!

+ For nettleseren er alle tagger av samme type like, men du kan skille de fra hverandre ved å bruke klasser og ID'er.
For eksempel, noen av paragrafene kan være introduksjoner, så du kan gi de en klasse som du kaller `introduksjon`. Se om du finner noen klasser i `side.html` .

+ ID'er brukes for å markere unike elementer på siden din. Se om du kan finne `div` taggen med en `ID` lik `katt` på siden.

+ Hva skjer hvis du flytter ting rundt? La oss gå tilbake til tekstprogrammet. Finn en `<ol>` tagg i koden og velg den og alt som er inne i den, slik som dette:

```{.language-markup}
<ol>
	<li>Katter</li>
	<li>Bløtkake</li>
	<li>Sove lenge</li>
	<li>Spille spill</li>
</ol>
```

Så kopierer du det og flytter det et annet sted. Lagre siden, og oppdater den i nettleseren. Hvordan påvirker rekkefølgen av koden rekkefølgen på det som vises i nettleseren?

## Ting du kan prøve { .try}

* Lag din egen paragraf med tekst.
* Lag en link som peker til en annen del av siden (hint: det har noe med ID å gjøre - se etter en link som peker til katten).
* Legg til dine egne overskrifter der du syns de kan passe. Hva skjer hvis du endrer tallet i overskrift-taggen, for eksempel fra `<h3>` til `<h4>`?
* Hva må du gjøre for å linke til en annen side?
* Hvis du bruker utvikler-verktøyene: når du åpner panelet med kode, prøv å dobbeltklikk på en kode som ser interessant ut. Se om du kan endre den. Da får du direkte en forhåndsvisning på hva som skjer når du endrer koden, uten at du trenger å bytte mellom nettleseren og tekstprogrammet. Kult, ikke sant? Så oppdaterer du siden. Hva skjedde? Når du redigerer kode på denne måten blir det ikke lagret, så du kan teste hva som skjer uten å ødelegge filen. Sånn kan du eksperimentere masse, men alltid ha muligheten til å gå tilbake.
