---
title: Izlazak sunca — Bilješke za volontere
language: hr-HR
embeds: "*.png"
materials: [""]
...

#Uvod:
U ovom projektu djeca će naučiti animirati pomoću CSS-a. Koristit će CSS @keyframes pravilo kako bi animirali slike.

#Online Resursi

Za pisanje HTML i CSS kôda preporučujemo korištenje oline sučelja [trinket](https://trinket.io/). Ovaj projekt sadrži sljedeće 'trinkete':

+ ['Sunrise' starting point](https://trinket.io/html/web-sunrise)

Ovdje možete pronaći primjer rješenja izazova:

+ ['Sunrise' Finished](https://trinket.io/html/abcc0284a3)

#Offline Resursi
Ovaj projekt moguće je izraditi i [offline](../offline.html). Potrebne datoteke je moguće preuzeti klikom na poveznicu projekta 'Download Project Materials'. Tu se nalazi mapa 'Project Resources', koja sadrži datoteke potrebne za izradu projekta offline.
Pobrinite se da svako djete ima pristup kopiji sljedećih datoteka: 
+ template/index.html
+ template/prefix.js
+ template/style.css
+ sunrise/index.html
+ sunrise/style.css
+ sunrise/prefixfree.js
+ sunrise/boat.png
+ sunrise/cloud.png
+ sunrise/helicopter.png
+ sunrise/rainbow.png
+ sunrise/sun.png

Gotova verzija izazova ovoga projekta nalazi se u mapi 'Club Leader Resources' koja sadrži datoteke:

+ index.html
+ style.css
+ prefixfree.js
+ boat.png
+ sun.png
+ rainbow.png

#Ciljevi učenja
+ Uređivanje i animiranje u CSS-u:
	+ Upoznavanje @keyframes` pravila za definiranje koraka u animaciji.
	+ Povečavanje korištenja svojstava koji definiraju veličinu, oblik, poziciju i boju elemenata na web stranici.

#Izazovi
+ "Dijagonalna animacija" - uređivanje `@keyframe` svojstva 
+ "Poboljšaj nebo" - dodavanje više keyframeova i postavljanje pozadine (background:).
+ "Više animacija" - animiranje više slika i elemenata korištenjem različitih CSS svojstava. 

#Odgovori na najčešće postavljana pitanja

+ Ovaj projekt koristi javascript biblioteku `prefixfree.js` kako bi se osigurala podudaranost animacije u različitim preglednicima. Ako ova biblioteka nije u uporabi, djeca koja koriste starije preglednike morat će prilagođavati animaciju svom pregledniku. Na primjer:

```
animation: sky 10s infinite; 		  	// Za sve novije preglednike
-webkit-animation: sky 10s infinite;  	// Za Webkit preglednike(Chrome, Safari...)
-moz-animation: sky 10s infinite;     	// Za Mozilla preglednike
-o-animation: sky 10s infinite;       	// Za Opera preglednike
-ms-animation: sky 10s infinite;		// Za Microsoft preglednike 
```