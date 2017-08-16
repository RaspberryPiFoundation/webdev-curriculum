---
title: Napravi robota
level: HTML & CSS 2
language: hr-HR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# Uvod { .intro}

U ovom projektu naučit ćeš kako postavljanjem slika izraditi robota. 

![screenshot](robot-final.png)

# Korak 1: Oči { .activity}

Napravimo oči našem robotu!

## Zadatci { .check}

+ Klikom na poveznicu <a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a> otvori sučelje za izradu stranice. Čitaš li ovaj dokument online možeš koristiti i ugrađeni prozor koji se nalazi ispod ovog teksta: 

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/b29b50e571" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ Svaka slika u ovom projektu ima svoje vlastiti naziv (__id__). Na primjer, HTML kôd za slike lica i očiju  (‘face’, ‘eyes1’ i ‘eyes2’), koji počinje u osmoj liniji kôda, izgleda ovako:

```
<img id="face" ...>
<img id="eyes1" ...>
<img id="eyes2" ...>
```

+ Pomoću naziva (__id__) slike i simbola `#` moguće je svaku sliku oblikovati posebno. 

Klikom na karticu `style.css` otvori pripadajuću CSS datoteku. Primjećuješ li kako je veličina lica robota i ostalih slika različita? 

![screenshot](robot-id.png)

+ Dodaj sljedeći CSS kôd kojim ćeš oblikovati oči robota: 

```
#eyes1 {
    width: 200px;
}
```

Primijeti da smo, koristeći `#eyes1`, u CSS kôdu oblikovali samo sliku `eyes1`. Ako ti je draže možeš umjesto `#eyes1` koristiti `#eyes2` ili `#eyes3`. 

![screenshot](robot-eyes-width.png)

+ Primjećuješ li kako se slike na stranici prikazuju jedna pored druge? To se zove  __relativno__ pozicioniranje. Želiš li pregledniku reći na koje točno mjesto da postavi oči morat ćeš, umjesto relativnog, koristiti  __apsolutno__ pozicioniranje.

Dodaj sljedeće tri linije CSS kôda za sliku `eyes1`:

```
position: absolute;
top: 200px;
left: 100px;
```

Rezultat prethodnog kôda je pomicanje očiju na ispravno mjesto na licu robota. 

![screenshot](robot-eyes-position.png)

Taj CSS kôd govori pregledniku koliko daleko od vrha (top) ili lijevog ruba (left) stranice treba prikazati sliku.  

![screenshot](robot-eyes-position2.png)

Umjesto `top`  moguće je koristiti `bottom`. Na taj način gažemo pregledniku koliko daleko od __dna__ prozora  treba prikazati sliku. Isto tako umjesto `left` može se koristiti `right`.

# Korak 2: Usta { .activity}

Napravimo robotu usta!

## Zadatci{ .check}

+ Stilu za sliku `mouth1` dodaj sljedeći CSS kôd:

```
#mouth1 {
    width: 50px;
    position: absolute;
    top: 200px;
    left: 200px;
}
```

+ Usta su prilično mala i nisu na ispravnom mjestu. 

![screenshot](robot-mouth.png)

Možeš li to popraviti izmjenama u CSS kôdu?

## Spremi projekt {.save}

##Izazov: Dizajniraj svog robota {.challenge}
Iskoristi naučeno i dovrši svog robota. Pogledaj nekoliko primjera: 

![screenshot](robot-examples.png)

## Spremi promjene u projektu {.save}

##Izazov: Dodaj svoje slike {.challenge}
Možeš li pronaći dodatne slike za svog robota i postaviti ih na stranicu? Možeš čak i zamijeniti robota s vlastitim. 

```
<img id="face" src="myFace.png">
```

## Spremi projekt {.save} 