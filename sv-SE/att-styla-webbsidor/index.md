---
title: Att styla webbsidor
level: Nivå 2
materials: "kod och material"
layout: project
---

## Uppgiften { .intro}

Nu ska vi göra vår webbsida snyggare genom att styla den lite. I den här och nästa lektion ska vi lära oss hur man byter färg, text, storlek och en massa annat!

Vi stylar HTML-sidor genom att använda ett språk som kallas för __CSS__ (det står för __Cascading Style Sheets__). Det är ett jätteenkelt språk att lära sig. Låt oss sätta igång.

#Steg 1: Förberedelser { .activity}

Det finns många sätt att styla din HTML: i texten, i head-taggen eller som ett separat .css-dokument som vi sedan länkar till från head-taggen. Men idag ska vi fokusera på att styla 'head-tagg'-delen av vår html-sida så att vi inte behöver oroa oss för att hantera en massa olika filer.

## Checklista för aktiviteten { .check}

+ Öppna index.html från Felix-mappen som vi gjorde förra lektionen.
+ I head-taggen behöver vi ha en __style-tagg__.
```html
<style>
</style>
```
Alla våra stylingar kommer att ligga mellan dessa två delar. Enkelt. Generellt så ser css-kod ut så här:

```css
selector {
	property: value;
}
```

+ Kan du hitta ‘{‘ och ‘}’ tangenterna på ditt tangentbord?
+ Kan du hitta ‘:’ och ‘;’ då?

Selectors kan vara HTML-element så som `h1`, `p`, `img`, `a`. Men det kan också vara andra saker som vi ska lära oss senare.

# Steg 2: Att lägga till färger { .activity}

Nu lägger vi till lite färg med hjälp av färgpaletten! På engelska heter färgpaletten color property. Color utan ett u, det är lite förvirrande eftersom att det är den amerikanska stavningen, även om CSS faktiskt uppfanns av en norsk snubbe. Men du kommer att vänja dig, glöm bara inte u:et på engelskalektionen!

Låt oss göra så att`h1` blir röd istället för svart.

```css
h1 {
	color: red;
}
```

## __SPARA__ din fil och __ÖPPNA__ den i din webbläsare { .save}

Nu är texten röd, w00t! Det finns olika sätt att berätta värdet på färgen. Det finns 16 grundläggande namn på färger, de är aqua, black, blue, fuchsia, gray, green, lime, maroon, navy, olive, purple, red, silver, teal, white, och yellow.

+ Försök att ändra färgen till något annat!
De flesta webbläsare stödjer ytterligare 130 färger, hela listan i alfabetisk ordning hittar du här [http://www.w3.org/TR/css3-color/#svg-color](http://www.w3.org/TR/css3-color/#svg-color) - finns din favoritfärg med i listan?

+ Man vi kan använda ännu fler färger genom att använda __hexkoder__ istället för färgnamnet. En hexkod är en # följt av 6 siffror, siffrorna kan vara mellan 0-9 eller bokstäverna A, B, C, D, E, F. Genom att använda hexkod kan vi få fram mer är 16 miljoner färger!
+ På Code Club är vår favoritfärg `#58AB57`. Kan du gissa vilken färg det är? Försök ändra en bit av texten till den färgen och granska det i webbläsaren för att se.

## __SPARA__ din fil och __ÖPPNA__ den i din webbläsare { .save}

#Steg 3: Färglägga specifika delar { .activity}

Men om vi nu skulle vilja göra ordet ‘orange’ i ‘hans päls är orange’ orange? Inte hela paragrafen, bara det ordet.

Ett sätt att göra det är att sätta `<span>` taggar på båda sidor om ordet, så här:

`<span>orange</span>`

Sedan kan vi styla span-taggen i head-taggen.

```css
span {
	color: orange;
}
```

## __SAVE__din fil och __VIEW__ den i din webbläsare { .save}

#Steg 4: Bakgrund { .activity}

Vi kan lägga till färger till bakgrunden också, inte bara till texten. Till exempel:

```css
body {
	background-color: #D2FAFC;
}
```

Det här gör hela bakgrunden ljusblå. Du kan välja vilken färg du vill från listan på [www.colourpicker.com](http://www.colourpicker.com) som genererar de nummer du behöver, detta nummer kan du sedan kopiera och klistra in i din kod.

Försök med:

```css
h1 {
	background-color: black;
}
```

Eftersom att vi redan definierat, eller förklarat, `h1` kan vi bara skriva in färgen tillsammans med background-color, vi behöver alltså inte skriva ut allt igen.

```css
h1 {
	background-color: black;
	color: red;
}
```


## __SPARA__din fil och __ÖPPNA__ den i din webbläsare { .save}


## Kul med text

Kanske ska den ‘försvunna’ rubriken vara __större__ och alla ord inledas med stora bokstäver? Vi kan bestämma storleken på texten genom att använda `font-size`. Värdena kan variera men de vanligaste är 12, 14, 16, 32, 48 och 72 pixlar. Just nu kan vi prova 72px. (px betyder pixel).

```css
h1 {
    background-color: black;
    color: red;
    font-size: 72px;
}
```

Försök nu att göra rubrikens inledande bokstäver stora bara genom att använda `text-transform:uppercase;` Vi kan också göra den understruken genom att använda `text-decoration:underline;`

## __SPARA__din fil och __ÖPPNA__ den i din webbläsare { .save}

Nu syns den väl mycket mer, eller hur? 

### Endast om du har en Firefox eller Chrome som webbläsare.

Det finns faktiskt ett annat värde för att dekorera text som kallas för blink. Vi kommer inte berätta för dig vad det gör, du får undersöka saken själv. `text-decoration: blink;` (det blir lite irriterande efter ett tag, du kan återgå till understruket om du vill).

# Steg 6. Centrera text (och bilder) horisontellt { .activity}

All vår text ligger åt vänster. Vi kan ändra det genom att använda `text-align:center` (det går även att använda ‘right’, ‘left’ är nämligen utgångsläget).

+ Vi vill att all vår text på just den här webbsidan ska vara centrerad, därför skriver vi som i rutan här nedanför. Lägg dock märke till att vi använder den amerikanska stavningen för ordet center.

```css
body {
    background-color: #F8FAF4;
    text-align: center;
}
```
Lade du märke till att allt på sidan flyttade sig åt mitten när du skrev ‘text-align: center’ i body-sektionen? Anledningen är att allt inne i body-sektionen får samma stil. Det här händer när ett element ligger inuti ett annat, som i det här exemplet:

```html
<p>Har du sett Felix? <em>snälla</em> kontakta hans ägare</p>
```

Ordet ‘snälla’ kommer ha stilen som de får av `<p>` elementet tillsammans med stilen som det får från `<em>` elementet. Element kan nämligen liksom "ärva" stilar som deras föräldrar har. Men var försiktig, en del stilar är inte ärftliga. Vi kommer lära oss om dessa senare.

## __SPARA__din fil och __ÖPPNA__ den i din webbläsare { .save}

##Pröva också { .try}

+ Hur skulle du ändra sidan för att göra den snyggare? Varför inte försöka med att använda alla dina favoritfärger? Har de egna namn eller måste du använda en hexkod?
+ Om du blir klar tidigare kan du gå tillbaka och lägga till stilar till den HTML-koden som vi gjort under de tidigare lektionerna.
