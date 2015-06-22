---
title: en hjemmeside
materials: "ressurser"
layout: project
---

## Introduksjon { .intro}

Du kjenner en del __HTML__ tagger, så nå er det på tide å lage din første hjemmeside! La oss begynne med en gang.

# Steg 1: Åpne siden som heter om meg { .activity}

## Activitet { .check}

1. Åpne et __tekstprogram__.
2. Åpne filen som heter `om_meg.html`. Filen inneholder bittelitt HTMl kode for å hjelpe deg med å komme igang, men du må skrive resten selv.


# Steg 2: Lag en hjemmeside om deg selv { .activity}

### Om å gjøre feil

Feil skjer ofte. Det er veldig lett å gjøre dem i HTML fordi du må huske å lukke hver tag, og åpnings-taggen og avslutnings-taggen er litt annerledes. La oss prøve å gjøre noen feil for å se hvordan nettleseren prøver å forstå meningen av koden vår, selv om vi ikke har skrevet den perfekt.

## Activitet { .check}

+ La oss ta listen av ting vi liker som et eksempel. En av feilene som ofte skjer, er å glemme __ avslutnings-taggen__, så la oss fjerne `</ ul>` for å se hvordan det påvirker siden. Lagre filen og oppdater den i nettleseren.

Hva skjedde? Noen ting under listen ble flyttet litt til høyre. Hvis du inspiserer siden med X-Ray Goggles kan du se at ting som fulgte listen, nå er inne i den, det er derfor de har flyttet seg til høyre. Etter at vi fjernet avslutnings-taggen vet nettleseren rett og slett ikke at listen er avsluttet.

Legg avslutnings-taggen `</ ul>` igjen og lagre siden. Når du oppdaterer siden igjen er ikke resten av kodene inne i listen lenger.

+ Tagger må være stavet riktig for at nettleseren skal forstå dem. Hva skjer hvis vi gjør en skrivefeil?

Finn `<h1>` taggen. La oss se hva som skjer hvis vi forandrer den til `<d1>`. Lagre filen og oppdater siden i nettlesern.

Hva sjedde? Siden nettleseren ikke vet hva du mener med denne taggen så kan den ikke lenger forstå at det skal være en overskrift, så den bruker ikke lenger en større tekst til å vise hvor viktig akkurat den teksten er.

Bytt `<d1>` tilbake til `<h1>` og lagre igjen.


+ Finn en av `<img>` taggene. Vi har akkurat prøvd å feilstave en tagg og nettleseren var ikke sikker på hva den skal gjøre med det. Men hva hvis vi feilstaver attributtet?

Inne i `<img>` taggen har vi `href` og `alt` attributter:

```html
<img href = "kattunge.jpg" alt = "Dette er en kattunge." />
```

Prøv å endre `href` til noe annet. Lagre dokumentet og oppdater i nettleseren.

Å nei! Kattungen er borte!

Plutselig vet ikke nettleseren hvor den skal se etter bildet den skal vise - den ser etter filnavnet i `href` atributten som ikke lenger er der.

Endre det tilbake til `href` så vi kan fortsette å se på kattungen.

+ Nå fjern det andre anførselstegnet (`" `) fra `alt` attributtet av dette bildet: den etter teksten, slik at du ender opp med dette:

```html
<img href="kattunge.jpg" alt="Dette er en kattunge. />
```

Lagre og oppdater i nettleseren.

Den neste taggen forsvant. Hvorfor? Nettleseren vil tro at alt etter `alt =" `og før neste sitatmerke (` "`) er ekstra tekst for dette bildet, inkludert slutten av bildekoden og neste åpnings-taggen.

Fiks det igjen ved å legge til et anførselstegn etter `alt` teksten.

Vi har nå gjort noen vanlige feil sammen, og har sett at noen ganger kan en enkelt feil gjøre slik at nettleseren ikke forstår hva vi mener. Men mesteparten av tiden vil den prøve å vise oss noe uansett, så når vi har endret overskrift-koden til noe annet, forsto den ikke at teksten var en overskrift, men viste oss fortsatt teksten. Så den prøver så godt den kan, men noen feil kan gjøre den ganske forvirret.

# Steg 3: Lag en ny side og link til den { .activity}

La oss lage en ny side. Åpne `omg_meg_side_2.html`.  Den har litt mindre kode en den andre siden du jobbet med, men jeg er sikker på at du kan legge til mer kode selv nå.


__Noen tips og ideer:__

* Legg til en overskrift som vil fungere som tittelen på denne siden.
* Denne siden kan handle om kjæledyret ditt, din favoritt hobby eller vennene dine og deres hobbyer.
* Lag en liste over ting kjæledyret liker, hvis siden er om et kjæledyr.

__Er du ferdig? Flott! La oss nå linke de to sidene du har laget sammen.__

Når vi har linket til deler av den samme siden, kunne vi bare peke linken til en bestemt id på siden, som dette:

```html
<a href="#kattunge"> Klikk for å se en kattunge </ a>
```

Som da tok deg til noe sånt som dette:

```html
<div id="kattunge">
<img src = "kattunge.jpg" alt = "Dette er en kattunge." />
</ div>
```
Hvis du vil koble til en annen side, trenger vi ikke å inkludere hashsymbolet (`#`), men i stedet må vi si hvilken fil vi vil linken skal ta oss til.

Så for å linke fra `om_meg_side_2.html` til `om_meg.html` skriver vi slik:

```html
<a href="om_meg.html"> Gå til Om Meg siden </ a>
```

Du kan endre anker teksten til noe annet, som tittelen på siden hvis du har endret det.

For å linke tilbake fra `om_meg.html` til `om_meg_side_2.html` må du skrive det slik:

```html
<a href="om_meg_side_2.html"> Gå til min andre side </ a>
```

Gratulerer! Du har laget ditt eget nettsted.

# Publiser nettsiden din på Internett (ekstra aktivitet) { .activity }

Nå har du laget ditt eget nettsted. Du ønsker vel å vise det frem, gjør du ikke?

Hvis du bare kopierer adressen til websiden fra nettleseren din, og deretter sender den til noen, ville de ikke se den. Det er fordi denne adressen beskriver et sted på datamaskinen din, og vennene dine ikke har tilgang til den. Selv om hadde hatt det, hva om de ønsket å se på den når datamaskinen din er skrudd av?

Husker du servere fra den første økten? Servere er datamaskiner som alltid er på og koblet til Internett, og de er satt opp slik at folk kan besøke nettsteder som lever på disse datamaskinene.

For å gjøre dette vil vi bruke __Cyberduck__ - det er et program for å flytte filer fra din datamaskin til en server.

1. Klikk `Åpne Tilkobling`.
2. Legg inn servernavn, brukernavn og passord som instruert av Kodeklubben-hjelperen.
3.  Klikk `Tilkoble`. Du vil da se alle mappene og filene på serveren - mest sannsynlig vil serveren være tom, om du ikke har lagt filene dine ennå.
4. Dra nettsted-filene fra datamaskinen din til servervinduet. Opplastingen vil begynne.
5. Når det er lastet opp, kan du besøke nettstedet ditt på adressen gitt til deg av Kodeklubben-hjelperen.

## Ting du kan prøve { .try}

* Hvordan kan du linke til en annen side på nettet? (Hint: prøv å legge `http://` og deretter adressen til nettstedet du vil koble til)
* I likhet med forslaget ovenfor, hvordan ville du legge til et bilde fra et sted på nettet i stedet for fra datamaskinen? (Hint: igjen, prøve å legge `http://` og adressen til bildet)




