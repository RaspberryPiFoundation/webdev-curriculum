---
title: Povezane Sobe
level: HTML & CSS 2
language: hr-HR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# Uvod {.intro}

U ovom projektu napravit ćeš niz povezanih soba. Svaka soba je, ustvari, druga web stranica koju možeš uređivati u HTML-u. 

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ba5d27ec68?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="rooms-hall-finished.png">
</div>

__Upute__: Za promjenu sobe klikni vrata.

# Korak 1: Povezivanje s drugom web stranicom u istom projektu. {.activity}

Web projekt može biti napravljen od više povezanih HTML datoteka.

## Zadatci { .check}

+ Klikom na poveznicu: <a href="http://jumpto.cc/web-rooms" target="_blank">jumpto.cc/web-rooms</a> otvori sučelje za izradu stranice. Čitaš li ovaj dokument online možeš koristiti i ugrađeni prozor koji se nalazi ispod ovog teksta: 

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ef608f0733" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ Projekt bi se trebao pokrenuti sam i smjestiti te u hodnik (hall):

	![screenshot](rooms-hall-start.png)

+ Pogledaj kartice s datotekama uključenim u projekt. Pronađi karticu `tvroom.html` i klikni na nju.

	![screenshot](rooms-tvroom-html.png)

	To je druga html datoteka istog projekta. 


+ Da bi došli do datoteke `tvroom.html` potrebno je dodati poveznicu(link) u datoteku `index.html`. 

	Oznaci `<div>` s klasom `room` dodaj označeni kôd: 

	![screenshot](rooms-link-tvroom.png)

+ Provjeri rezultat klikom na poveznicu __TV Room__. Otvorit će se stranica `tvroom.html`.

	Primijeti da `tvroom.html` datoteka također ima svoju `tvroom.css` datoteku koja određuje izgled ove stranice. 

	![screenshot](rooms-tvroom-unstyled.png)

	
##Izazov: Dodaj poveznicu {.challenge}

Oznakom `<a>` dodaj poveznicu na stranicu `tvroom.html` koja će te vratiti natrag nicu da biste dosli nazad do web stranice Hodnik koja se zove `index.html`. Tekst poveznice neka bude 'Hall'.

Stranica TV Room sada treba imati poveznicu kao na slici: 

![screenshot](rooms-hall-link.png)

Provjeri kôd. Klikom na poveznice trebaš se pomicati iz hodnika (Hall) u TV sobu (TV Room) i natrag. .


## Spremi projekt {.save}

# Korak 2: Dodaj drugu sobu {.activity}

Dodajmo sada sobu za igru, __Games Room__. 

+ Klikni gumb __+__ kako bi se dodala nova stranica:

	![screenshot](rooms-add-page.png)

	Ime stranice neka bude `gamesroom.html`:

  	![screenshot](rooms-games-html.png)

+ HTML kôd sobe za igru (__Games Room__) je sličan kôdu stranice`tvroom.html` pa __kopiraj__ kôd sa stranice  `tvroom.html` __zalijepi__ ga u datoteku `gamesroom.html`.
	
	Promijeni istaknute nazive tako da piše Games umjesto TV:

	![screenshot](images/rooms-games-html2.png)	

+ Datoteka `gamesroom.html` sada koristi datoteku  `gamesroom.css` koja još ne postoji. 

	Klikom na gumb __+__ kreiraj datoteku `gamesroom.css` . 


+ CSS kôd za __Games Room__ je sličan kôdu iz datoteke `tvroom.css`. __Kopiraj__ kôd iz datoteke `tvroom.css` i __zalijepi__  ga u datoteku `gamesroom.css`.

	![screenshot](rooms-add-games-css.png)

+ Dodaj poveznicu iz hodnika (Hall) u sobu za igru (Games room):

	![screenshot](rooms-hall-games.png)

+ Provjeri rezultat klikom na poveznicu Games Room. 

	Stranica __Games Room__ treba izgledati ovako: 

	![screenshot](rooms-games-before.png)

	Nije previše zanimljiva, ali to možeš popraviti u sljedećem izazovu. 

## Spremi promjene u projektu {.save}

##Izazov: Uredi i poveži sobu za igru (Games Room) {.challenge}

Uredi HTML i CSS kôd stranice __Games Room__ tako da ona izgleda ovako: 

![screenshot](rooms-games-challenge.png)

Pomoć: Morat ćeš promijeniti boju pozadine, boju slova i boju obruba u datoteci `gamesroom.css`. Svijetlo zelena se naziva `chartreuse`.  

Pomoć: Morat ćeš dodati poveznicu oznakom `<a>` u datoteku `gamesroom.html` koja vodi do datoteke  `index.html`.

## Spremi promjene u projektu {.save}

# Korak 3: Neka poveznice izgledaju kao vrata {.activity}

Poveznice ne moraju biti samo tekstovi. Pomoću oznake `<div>` napravit ćemo vrata na koja je moguće kliknuti .

## Zadatci { .check}

+ Otvori datoteku `index.html` i oko teksta za povezivanje __TV Room__ dodaj oznaku `<div>`. Da bi se na nju moglo kliknuti mora biti unutar oznake `<a>`.

  Dodaj `id="hall2tv"` kako bi ga mogao posebno urediti. 

  ![screenshot](rooms-tvroom-div.png)  

+ Klikom na `style.css` kartica, idi do kraja i dodaj sljedeći CSS kôd kojim ćeš promijeniti boju i veličinu vrata:

	![screenshot](rooms-door-css1.png)

+ Testiraj svoju web-stranicu klikom na bilo koji dio vrata, ne samo na tekst.

+ Da bi poveznica i izgledala kao vrata, s tri strane dodat ćemo obrub.

	![screenshot](rooms-door-css2.png)

+ Dodaj sljedeći CSS kôd kako bi tekst na vratima izgledao bolje.

	![screenshot](images/rooms-door-css3.png)

+ Vjerojatno primjećuješ da vrata izgledaju kao da lebde. To ćemo popraviti tako da vrata premjestimo unutar sobe.

	![screenshot](rooms-door-position.png)	

+ Testiraj stranicu klikom na vrata.

## Spremi promjene u projektu {.save}

##Izazov: Dodaj više vrata {.challenge}

Pretvori ostale poveznice u projektu u vrata na isti način. 

Za svaka vrata ćeš morati:

+ Urediti poveznicu vrata da pomoću oznake `<div>` s nazivom (id) kao što je`hall2games` kako bi se naknadno mogla urediti.

	Na primjer: 

	`<a href="gamesroom.html"><div id="hall2games">Games Room</div></a>`

+ Dodaj CSS kôd definirani id u `.css` datoteku. Za uštedu vremena slobodno koristi mogućnosti _kopiraj_ i _zaplijepi_. Slobodno svaka vrata uredi drugačije. 

+ Promijeni mjesto vrata koristeći `bottom:` i `left:` ili `right:`.

Hodnik (Hall) bi mogao izgledati ovako:

![screenshot](rooms-hall-doors.png)

TV soba (TV Room) može izgledati ovako:

![screenshot](rooms-tvroom-door.png)	


# Korak 4: Dodavanje slike u pozadinu {.activity}

Uredimo hodnik tako što ćemo mu dodati sliku u pozadinu.

## Zadatci{ .check}

+  Dodaj sljedeći kôd datoteku `style.css`. Njime će se dodati slika u pozadinu hodnika:

	![screenshot](rooms-hall-decorated.png)	

	Slika će se ponoviti da bi popunila sobu. 


## Spremi projekt {.save}

##Izazov: Dodaj pozadinsku sliku u Games Room {.challenge}

Možeš li urediti sobu za igru s pozadinskom slikom?

Možeš koristiti `space-invader.png`. Ona je već učitana u projekt. 

Trebat ćeš:

+ Dodati sliku pomoću `background-image:` u stil `.room` u css datoteku za Games Room. 

Uređena soba bi trebala izgledati ovako :

![screenshot](rooms-games-finished.png)	

##Spremi projekt {.save}

##Izazov: Načini je svojom! {.challenge}

Dodaj još soba u svoj projekt. Za uštedu vremena slobodno koristi mogućnosti __kopiraj__ i __zalijepi__, te promijeni one elemente koje želiš. 

Za svaku sobu ćeš trebati:

+ Napraviti `.html` datoteku
+ Dodati poveznice za vrata __u__ i __iz__ nove 'sobe'
+ Za novu sobu napraviti `.css` datoteku sa stilom. 

Pomoću `background-color:` možeš promijenit boju pozadine svake sobe. Klikni na ikonu za dodavanje slike i provjeri koje pozadinske slike možeš koristiti:

![screenshot](rooms-images.png)	

## Spremi projekt {.save}

