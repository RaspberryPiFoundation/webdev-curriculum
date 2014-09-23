---
title: Att bygga enkla webbsidor
level: Nivå 1
language: sv-SE
embeds: "*.png"
materials: "kod och bilder"
stylesheet: web
...

## Uppgiften { .intro}

Nu kan du en del __HTML__ -taggar, så det är dags att skapa din första webbsida! Låt oss komma igång direkt. 

# Steg 1: Öppna dokumentet som heter about_me { .activity}

## Checklista { .check}

+ Öppna en textredigerare.
+ Öppna filen `about_me.html`. Filen innehåller bara en liten del HTML kod för att komma igång, men du kommer att skriva resten själv. 

# Steg 2: Skapa en sida om dig själv { .activity}

**Om misstag**

Misstag kan hända ofta. Det är väldigt lätt att göra misstag i HTML för att man måste komma ihåg att stänga varje tagg, och öppnande och avslutande taggarna ser lite oilka ut. Låt oss göra några misstag för att se hur webbläsaren försöker lista ut vår kod, även om vi inte har skrivit koden perfekt.

## Checklista { .check}

+ Låt oss ta listan över saker som vi gillar som exempel. Ett misstag som händer ofta är att man glömmer den _avslutande taggen_, så låt oss prova att ta bort `</ul>` för att se hur det påverkar sidan. Spara filen och uppdatera den i webbläsaren.

Vad hände? Vissa saker under listan har flyttats lite åt höger. Om du inspekterar webbsidan kan du se att det som följde på listan nu finns inuti listan, och därför har det flyttats till höger. När vi tog bort den avslutande taggen så vet inte webbläsaren att listan över objekt har upphört.

+ Lägg tillbaka `</ul>` taggen och spara. När du nu uppdaterar sidan så kommer resten av taggarna inte att finnas kvar inuti `<ul>` längre.
+ Taggarna behöver vara stavande korrekt för att webbläsaren ska förstå dem. Vad skulle hända om vi stavade fel på något?  
+ Hitta `<h1>` taggen. Låt oss ändra den till `<d1>`. Spara dokumentet och uppdatera det i webbläsaren.
 

Vad hände? Eftersom webbläsaren inte vet vad vi menar med denna tagg så kan den inte längre veta att det är en rubrik och då kommer den inte använda sig av en större text for att visa hur viktigt denna del av texten är. 

+ Ändra tillbaka `<d1>` till `<h1>` och spara igen.
+ Hitta en av `<img>` taggarna. Vi har precis provat att stava fel på taggnamnet och webbläsaren förstod inte vad den skulle göra. Men hur blir det om vi stavar fel på attributet? 

Inuti `<img>` -taggen har vi `href` och `alt` -attributen:
```{.language-markup}
<img href="kitten.jpg" alt="Det här är en kattunge." />
```

+ Prova att ändra `href` till något annat. Spara dokumentet och uppdatera webbläsaren.

Åh nej! Kattungen är borta! Plötsligt vet inte webbläsaren längre var den ska leta efter bilden som den ska visa – den letar efter filnamnet inuti 'href' attributet, men där finns det ju inte längre. 

+ Ändra tillbaka till `href` så att vi kan fortsätta titta på kattungen.
+ Ta nu bort det andra citatet (`" `) från` alt `-attributet på denna bild: den efter texten, så att du ser följande: 

```{.language-markup}
<img href="kitten.jpg" alt="Det här är en kattunge" />
```

+ Spara och uppdatera webbläsaren.

Nästa tagg försvann. Varför? Webbläsaren kommer att tro att allt efter `alt =" `och fram till nästa citat (` "`) är det mer text som hör till denna bild, även slutet på bildtaggen och nästa öppningstagg.

+ Fixa det genom att lägga till ett citattecken efter `alt` -texten.


Vi har gjort några vanliga misstag tillsammans, och ibland kan ett enkelt misstag göra att webbläsaren får kämpa för att förstå vad vi menar. Men för det mesta kommer den att försöka visa oss något, som när vi ändrade rubriktaggen till något annat, så förstod webbläsaren inte att den här texten var en rubrik, men den visade oss fortfarande texten. Så den är lite förstående, men vissa misstag kan göra webbläsaren mycket förvirrad.

# Steg 3: Skapa en annan sida och länka till den { .activity}

+ Låt oss skapa en annan sida. Öppna 'about_me_page_2.html'. Den har lite mindre kod än den sista sidan du arbetade med, men du kan säkert lista ut hur man lägger till nya taggar nu.

__Några tips och idéer:__

* Lägg till en rubrik som kommer att fungera som titeln på den här sidan.
* Du kan låta den här sidan handla om ditt husdjur, din favorithobby eller dina vänner och deras fritidsintressen.
* Lägg till en lista över saker ditt husdjur tycker om, om din sida handlar om husdjur.

__Är du klar? Toppen! Låt oss nu länka dessa två sidor som du har skapat.__

När vi har att länkat till delar av samma sida, kan vi peka länkar till ett specifikt id på en sida, som det här:

```{.language-markup}
<a href="#kitten">Klicka för att se kattungen</a>
```

Som sedan visade något som det här: 

```{.language-markup}
<div id="kitten">
	<img src="kitten.jpg" alt="Det här är en kattunge." />
</div>
```

För att länka till en annan sida behöver vi inte inkludera hash-symbolen (`#`), istället behöver vi beskriva vilken fil vi vill att länken ska ta oss till. 

Att länka från `about_me_page_2.html` till `about_me.html` skriv då följande: 

```{.language-markup}
<a href="about_me.html">Gå till sidan om mig</a>
```

Du kan ändra texten till något annat, som till exempel titeln på sidan om du har ändrat den. 

För att länka tillbaka från `about_me.html` till `about_me_page_2.html` behöver du skriva följande: 

```{.language-markup}
<a href="about_me_page_2.html">Gå till min andra sida</a>
```

Grattis! Du har precis skapat din alldeles egna webbsida.

# Att lägga din websida på webben (extra aktivitet) { .activity}


Nu när du har skapat din egen webbsida vill du ju visa den, eller hur?

Om du helt enkelt kopierat adressen till webbsidan från din webbläsare och sedan skickat den till någon, skulle de inte se den. Det beror på att denna adress beskriver en plats på din dator, och dina vänner inte har tillgång till det. Även om de hade tillgång, vad händer om de ville titta på webbsidan när datorn inte är påslagen?

Kommer du ihåg servrar från den första lektionen? Servrar är datorer som alltid är på och anslutna till internet, och de konfigureras så att folk kan besöka webbplatser som lever på dessa datorer.

För att göra det kommer vi att använda __Cyberduck__ - det är ett program för att flytta filer från din dator till en server.

+ Klicka på `Öppna Anslutning`.
+ Lägg till servernamn, användarnamn och lösenord enligt anvisningar från CodeClub-ledaren.
+ Klicka på `Anslut`. Du kommer då att se alla mappar och filer på servern - troligtvis kommer servern att vara tom, eftersom du inte har lagt till dina filer ännu.
+ Dra dina filer från din dator till server-fönstret. Uppladdningen kommer nu att börja.
+ När filerna har laddats upp, kan du besöka din webbsida på adressen som du får av CodeClub-ledaren.


## Saker att prova { .try}

* Hur kan du länka till en annan sida på nätet? (Tips: prova att lägga `http://` och sedan adressen till den webbsida du vill länka till)

* I likhet med förslaget ovan, hur skulle du lägga upp en bild från någonstans på nätet i stället för en bild från din dator? (Tips: igen, prova att lägga `http://` och adressen till bilden)
