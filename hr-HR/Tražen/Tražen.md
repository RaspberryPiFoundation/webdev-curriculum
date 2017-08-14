---
title: Tražen!
level: HTML & CSS 1
language: hr-HR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# Uvod { .intro}

U ovom projektu naučit ćemo napraviti plakat.

![screenshot](wanted-final.png)

# Korak 1: Uređivanje plakata { .activity}

Započnimo uređivanjem CSS koda za plakat.

## Zadatci { .check}

+ Otvori Trinket sučelje klikom na poveznicu <a href="http://jumpto.cc/web-wanted" target="_blank">jumpto.cc/web-wanted</a>. Čitaš li ovaj dokument online, možeš koristiti i prozor koji se nalazi ispod ovog teksta. 

<div class="trinket">
	<iframe src="https://trinket.io/embed/html/58318bee1f" width="100%" height="550" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
	</iframe>
</div>

+ Odaberi karticu "style.css". Primijeti  da već postoje neka CSS svojstva za oznaku `div` koju sadrže različiti dijelovi plakata.

	```
	div {
	    text-align: center;
	    overflow: hidden;
	    border: 2px solid black;
	    width: 300px;
    }	
	```

+ Započet ćemo tako šo ćemo promijeniti svojstvo `text-align`:

	```
	text-align: center;
	```
	
	Što će se dogoditi kada promjeniš riječ s `center` na `left` ili `right`?

+ Promotrimo sada svojsvo `border`:

	```
	border: 2px solid black;
	```

	`2px` u kôdu iznad označava 2 piksela. Promijeni svojstvo `border` na sljedeći način: umjesto `2px solid black` upiši `4px dotted red`. Što se dogodilo?

+ Sada promijeni svojstvo `width` na `400px`. Što se dogodilo s plakatom?

+ Promijenimo boju pozadine plakata. Idi na kraj 5. reda svog kôda i pritisni tipku enter. Sada imaš novi prazan red.

	![screenshot](wanted-newline.png)

	U novom redu upiši sljedeći kôd: 

	```
	background: yellow;
	```

	Provjeri je li upisani kôd _jednak_ kôdu iznad. Primijeti da je pozadina dijela stranice koji se nalazi unutar oznake `<div>` sada žuta.

	![screenshot](wanted-background.png)

##Izazov: Poboljšaj svoj plakat {.challenge}

Stilu oznake `div` dodaj sljedeće CSS svojstvo:

```
border-radius: 40px;
```

Što radi ovo svojstvo? Što će se dogoditi ako promjeniš broj u kôdu iznad?

## Spremi projekt {.save}

# Korak 2: Uređivanje slika { .activity}

Poboljšajmo izgled slike.

## Zadatci { .check}

+ Trenutačno za oznaku `<img>` nema niti jednog CSS svojstva. Dodajmo neke!

	Za početak, ispod kôda za oznaku `div` dodaj sljedeći kôd:

	```
	img {

	}
	```

	![screenshot](wanted-img-css.png)

+ Sada između vitičastih zagrada `{` i `}` dodajemo CSS svojstva za slike.

	Na primjer, između vitičastih zagrada dodaj sljedeći kôd. Njime određuješ širinu slike.

	```
	width: 100px;
	```

	Vidjet ćeš da se veličina slike promijenila. Sada je njezina širina 100 pixela.

	![screenshot](wanted-img-width.png)

+ Kôdom ispod dodaj obrub oko slike:

	```
	border: 1px solid black;
	```

+ Primjećuješ li da nema puno mjesta između slike i obruba?

	![screenshot](wanted-img-border.png)

	Ovo možemo popraviti svojstvom 'padding':

	```
	padding: 10px;
	```

	'Padding' je prostor između sadržaja (u ovom slučaju slike) i njegovog obruba.

	![screenshot](wanted-img-padding.png)

	Što misliš da će se dogoditi ako promjeniš padding na `50px`? Slobodno provjeri.

##Izazov: Poboljšaj sliku {.challenge}
Možeš li postaviti boju pozadine slike? Ili zaobljeni obrub?

## Spremi promjene u projektu {.save}

# Korak 3: Uređivanje naslova { .activity .new-page }

Poboljšajmo sada izgled `<h1>` naslova.

## Zadatci { .check}

+ Dodaj sljedeći kôd ispod CSS-a za slike:

	```
	h1 {

	}
	```

	Tu ćeš dodati CSS svojstva za glavni `<h1>` naslov.

+ Za promjenu fonta `<h1>` naslova, između vitičastih zagrada, dodaj sljedeći kôd:

	```
	font-family: Impact;
	```

+ Također možeš promijeniti veličinu naslova:

	```
	font-size: 50pt;
	```

+ 	Primjećuješ li da postoji veliki razmak između naslova `<h1>` i elemenata oko njega?

	![screenshot](wanted-h1-margin.png)

	To se događa zbog toga što oko naslova postoji margina. Margina je razmak između elementa (u ovom slučaju naslova) i ostalih stvari oko njega.

	Marginu smanji sljedećim kôdom:

	```
	margin: 10px;
	```

	![screenshot](wanted-h1-margin-small.png)

+ Naslov možeš i podcrtati. Za to iskoristi sljedeći kôd: 
	```
	text-decoration: underline;
	```

##Izazov: Napravite zakon plakat! {.challenge}

Dodaj više CSS kôda i uredi naslov `<h3>` i odlomke. 

![screenshot](wanted-final.png)

Ovo je lista CSS svojstava koje možeš koristiti:

```
color: black;
background: white;
font-family: Arial / Comic Sans MS / Courier / Impact / Tahoma;
font-size: 12pt;
font-weight: bold;
text-decoration: underline overline line-through;
margin: 10px;
padding: 10px;
width: 100px;
height: 100px;
```

## Spremi promjene u projektu {.save}

##Izazov: Reklamiraj događaj! {.challenge}
Možeš li napraviti plakat za neki događaj u školi? To može biti igrokaz, sportski događaj, ili plakat koji reklamira Code Club!

## Spremi projekt {.save}
