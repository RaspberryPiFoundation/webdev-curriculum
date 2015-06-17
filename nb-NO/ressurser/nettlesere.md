---
title: Hvorfor er det så mange nettlesere?
language: nb-NO
---

__Introduksjon:__ Du har allerede lært at en nettleser er bare et fancy program som tar __HTML filer__ (som er rene tekstfiler som bruker HTML-tagger), __CSS filer__ og tilhørende medier, som bilder eller videoer, og viser dem i henhold til instruksjoner skrevet i koden. Men det er så mange å velge mellom! Hva gjør de annerledes? Tross alt, bør de ikke alle gjør hva koden din forteller dem?

#Møt nettlesere
De mest populære nettlesere som brukes på stasjonære og bærbare datamaskiner er Internet Explorer, Google Chrome, Mozilla Firefox og Safari. På mange tabletter og telefoner som kjører på en Android-system Opera Mini, Chrome eller Dolphin brukes ofte. iPhone-er og iPad-er bruker Mobile Safari.

#HTML og CSS forandrer seg hele tiden, og det gjør også nettlesere
HTML og CSS er ikke statisk: nye ting du kan gjøre med dem blir bestemt og lagt til språkene hele tiden. Dette gjøres ved å bli enige om hva som er en standard, og hva er det ikke. Disse beslutningene er gjort av World Wide Web Consortium (__W3C__), en gruppe mennesker, inkludert programmerere, nettleser leverandører og andre som er interessert i fremtiden for web (du kan også søke om å bli medlem). Når det er besluttet hvilke funksjoner som skal legges til, fjernes eller endres, vil nettleser leverandørene deretter bygge nettlesere som kan gjenkjenne de nye tingene du kan nå gjøre med kode.

Dette er grunnen til at nye versjoner av nettlesere kommer ut ofte: slik at de nye programmene kan korrekt gjengi de nye funksjonene som folk begynner å bruke. Hvis du bruker en gammel nettleser, vil det ikke være i stand til å forstå dem. Husker du da du gjorde feil, og leseren bare ignorerte linjene den ikke visste hva den skulle gjøre med? Dette er tilsiktet. Det betyr at selv en gammel nettleser kan vise så mye som mulig ettersom HTML og CSS gradvis utvikler seg .

Hva slags ting blir __lagt til__ til HTML ? For eksempel, bare nylig `<audio>` og `<video>` tagger ble lagt til. Før det måtte nettleser leverandørene bruke plugins for å tillate lyder eller videoer skulle spilles i nettleseren. Fordi du ofte ikke kan installere plugins på mobiltelefoner og nettbrett ble det klart at det var et behov for å legge til nye koder. Hvis du åpner en side som inneholder `<audio>` tag i __Internet Explorer 8__ for eksempel , vil lyden ikke spille - leseren vet ikke hvordan de skal. Men neste versjon opp, __Internet Explorer 9__, vil ikke ha et problem med det. Den mer oppdatert nettleseren din er, jo mer kan du dra nytte av forbedringer i HTML og CSS.

## Så nye funksjoner ble lagt til HTML og CSS, hva nå?
Når nye funksjoner er lagt til publiserer W3C en spesifikasjon (__spec__). Spec er et dokument som beskriver hvordan nettlesere skal håndtere den nye koden, og hva den skal gjøre.
Deretter kan nettleser leverandørene finne ut hvordan man kan realisere dette. Noen ganger vil nye funksjoner bli gjennomført før det er enighet om hvordan man skal implementere dem, slik at nettsamfunnet kan finne ut hva som er den beste måten å håndtere det på.

## Uendelige måter å håndtere viser sider
Hvorfor er det så mange nettlesere å velge mellom? Det er fordi mange organisasjoner eller bedrifter tror deres implementering gjør nettleseren deres et bedre produkt og gir en __bedre brukeroppleveslse__.

Når du skriver kode, er det alltid mange måter å gjøre det du vil på, så det er ikke et "riktig svar". Tilsvarende nettleser leverandørene tar ulike tilnærminger til å skrive det som kalles en __layout engine__ - bit av nettleseren som finner ut hvordan den kan vise koden din visuelt.

Nettlesere er aldri perfekte - mange feil sniker seg inn i de versjonene som du ender opp med å bruke. Forskjellige nettlesere, fordi de er skrevet på en annen måte, vil ha forskjellig feil. Noen ganger vil disse påvirke hvordan sidene vises, så noen ganger kan du merke at en side som ser flott ut i __Firefox__ ser ikke helt rett ui i __Internett Explorer__.

## Så hvilken er best?
Det kommer an på hva du mener med best: mener du den __raskeste__ , mest __pålitelige__ , den som implementerer de fleste av de nye funksjonene i HTML ( du kan sjekke det [her](http://html5test.com/).
Du bør prøve noen og se hvordan du liker dem. Her i Kodelklubben liker vi å bruke __Chrome__ og deres utviklerverktøy og __Firefox__ med Firebug (utvikler verktøy).
