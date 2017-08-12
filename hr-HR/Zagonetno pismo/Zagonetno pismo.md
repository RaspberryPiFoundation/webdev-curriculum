---
title: Zagonetno pismo
level: HTML & CSS 1
language: hr-HR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# Uvod {.intro}

U ovom projektu napravit ćeš zagonetno pismo koje izgleda kao da je svako slovo izrezano iz različitih novina, magazina, stripa ili nekog drugog izvora.  

![screenshot](letter-final.png)

# Korak 1: Odaberi poruku {.activity}

Zagonetna pisma koriste se u filmovima i knjigama za slanje tajnih poruka. 

## Zadatci { .check}

+ Razmisli o tajnoj poruci dužine 11 do 12 riječi. Ako se ne možeš dosjetiti poruke, iskoristi ovu iz primjera: 'Sljedeći trag je u sefu. Kod za otvaranje sefa je 6553.'

+ Zapiši ili upamti odabranu poruku.  

# Korak 2: Uređivanje poruke {.activity}

Postavimo poruku na web stranicu. 

## Zadatci { .check}

+ Otvori sučelje koje se nalazi na poveznici: <a href="http://jumpto.cc/web-letter" target="_blank">jumpto.cc/web-letter</a>. Čitaš li ovo online, možeš koristiti i ugrađenu verziju sučelja za ovaj projekt koja se nalazi ispod ovog teksta. 

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/b5fbcf112e" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ S oznakom  za odlomak `<p>` smo se upoznali u projektu 'Sretan rođendan'. Oznaku `<span>` koristimo za grupiranje manjih dijelova teksta unutar odlomka, kako bi ih mogli različito oblikovati. 

![screenshot](letter-placeholder.png)

## Zadatci { .check}

+ Promijeni riječi poruke stavljajući jednu riječ unutar svake `<span>` oznake. Ako je tvoja poruka različite dužine od predložene, ukloni ili dodaj oznake `<span>`. 

![screenshot](letter-message.png)

## Zadatci { .check}

+ Klkni na gumb Run i provjeri rezultat.

	Pogledaš li slova možeš uočiti da su oblikovana tako da izgledaju kao da su zaglavila na stranici. 

# Korak 3: Uporaba klasa {.activity}

## Zadatci { .check}

+ Primjećuješ li tekst `class=""` koji se nalazi unutar oznake `<span>`? Možeš ga koristiti za oblikovanje više elemenata na isti način.  

+ Upotrijebi klasu `magazine1` na nekoliko `<span>` oznaka i provjeri rezultat. 

![screenshot](letter-magazine1.png)

## Zadatci { .check}

+ Na jedan element je moguće primijeniti više klasa. Potrebno je samo ostaviti razmak između njihovih naziva. Dodaj klasu `big` u jednu `<span>` oznaku u kojoj već imaš primjenjen stil magazine1. Provjeri rezultat. 

![screenshot](letter-big.png)

## Spremi projekt {.save}

## Izazov: Oblikuj svoju poruku {.challenge}

Iskoristi definirane stilove i oblikuj svoju poruku tako da izgleda kao zagonetno pismo. 

Dodaj sljedeće klase svojim `<span>` oznakama: 

+ `newspaper`, `magazine1`, `magazine2`

+ `medium`, `big`, `reallybig`

+ `rotateleft`, `rotateright`

+ `skewleft`, `skewright`

Nemoj dodavati više od jedne klase iz istog reda pojedinoj `<span>` oznaci.

Pogledaj primjer oblikovanog pisma:

![screenshot](letter-challenge1.png)

## Spremi promjene u projektu {.save}

# Korak 4: Uređivanje klasa {.activity}

## Zadatci { .check}

+ Odaberi karticu __'style.css'__. Pronađi stil za CSS klasu `newspaper`.

![screenshot](letter-newspaper.png)

+ Primijeti da se točka '.' nalazi ispred naziva klase u CSS datoteci, ali ne i unutar oznake `<span>` u HTML dokumentu.

+ Pogledaj ostale CSS klase korištene za oblikovanje zagonetnog pisma. Možeš li pronaći:

	+ Na koji način se u stilu `magazine1` tekst prikazuje velikim slovima?

	+ Kako se u stilu `magazine2` postavlja slika iza teksta?

![screenshot](letter-magazines.png)

+ Što se događa ako promijeniš `background-image` u stilu `magazine2` u `canvas.png`? Sviđa li ti se više `pink-pattern.png`, slobodno ga vrati.  

Želiš li, slobodno promijeni boje u magazine stilovima.

+ Pronađi CSS klase koje se koriste za okretanje i naginjanje riječi:

![screenshot](letter-rotate-skew.png)

Pokušaj mijenjati brojeve unutar tih stilova kako bi se postizali različiti efekti. Provjeri rezultat.  

# Korak 5: Izrada nove klase  {.activity}

Izradimo stil kojim ćemo oblikovati tekst tako da izgleda kao da je izrezan iz stripa. Na poveznici <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> možeš pronaći velik broj fontova besplatnih za uporabu. 

## Zadatci { .check}

+ U datoteci __style.css__, iza klase `magazine2` dodaj klasu `comic`. Ne zaboravi točku ispred imena klase. 

![screenshot](letter-comic1.png)

Ne brini se dobiješ li poruku 'The Rule is empty' (pravilo je prazno). To ćemo ubrzo popraviti. 

+ Dodaj CSS kôd u klasu comic. Slobodno koristi različite boje. Na sljedećoj poveznici možeš pronaći popis boja koje možeš koristiti: <a href="http://jumpto.cc/web-colours" target="_blank">jumpto.cc/web-colours</a>.

![screenshot](letter-comic2.png)

+ Upotrijebi stil comic u nekoj od `<span>` oznaka u HTML dokumentu i provjeri rezultat: 

![screenshot](letter-comic-output.png)

+ Sada možeš dodati neki zabavni font. Otvori novu karticu ili prozor preglednika. Slijedi poveznicu <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> i potraži font __'bangers'__:

![screenshot](letter-fonts1.png)

+ Klikni gumb 'Select this font (Odaberi ovaj font)':

![screenshot](letter-fonts2.png)

+ Na dnu stranice pojavit će se nova obavijest. Otvori ju kako bi se vidjelo sljedeće:

![screenshot](letter-fonts-link.png)

Kopiraj označen kôd. 

+ Zalijepi kopirani `<link>` kôd u zaglavlje (`<head>`) svoje web stranice:

![screenshot](letter-fonts-head.png)

To će ti omogućiti da iskoristiš font Bangers na svojoj stranici. 

+ Vrati se na karticu 'Google fonts', pronađi i kopiraj sljedeći font-family kôd:

![screenshot](letter-fonts-bangers.png)

+ Vrati se u trinket sučelje i zalijepi kopirani kôd u datoteku __'style.css'__  u stil comic:

![screenshot](letter-fonts-comic.png)

+ Provjeri rezultat. Trebao bi izgledati poput:  

![screenshot](letter-fonts-output.png)

## Spremi promjene u projektu {.save}

## Izazov: Oblikuj tekst tako da izgleda kao stari prikaz na računalu {.challenge}

Kreiraj font izgleda staromodnog prikaza na računalu i primijeni ga na neke riječi:

![screenshot](letter-fonts-printout.png)

Trebat će ti:

+ `VT323` font sa stranice <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a>. Trebaš li podsjetnik za postupak kopiranja fonta vrati se na korak 5.

+ Pozadinska slika `computer-printout-paper.png`. Trebaš li se podsjetiti kako se koristi pozadinska slika vrati se na korak 4.  	

## Izazov: Napravi svoj stil {.challenge}

Napravi novi stil kojim ćeš svoju poruku napraviti još zanimljivijom. Koristi naučeno u prethodnim projektima, a ideju možeš potražiti i u __style.css__ datoteci. 

Pogledaj primjer:

![screenshot](letter-fonts-challenge3.png)

Dostupne slike pronaći ćeš klikom na karticu Slike trinket sučelja. Pokušaj postaviti za pozadinu jednu od sljedećih slika:  

+ `rough-paper.png`

+ `canvas.png`

Imaš li trinket račun možeš učitati i vlastite slike, kao u projektu 'Ispričaj priču'. 

Fontove potraži na poveznici <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a>, kopiraj njihovu oznaku `<link>` i pripadajući CSS kôd u trinket sučelje.  

## Spremi projekt {.save}
