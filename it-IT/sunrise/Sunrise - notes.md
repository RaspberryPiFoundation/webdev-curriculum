---
title: Sorgere del sole — Note per i leader del club
---

#Introduzione:
In questo progetto, i bambini apprenderanno come animare una semplice scena utilizzando il CSS. Useranno la regola CSS del @keyframes per animare diverse proprietà di immagini e divs.

#Risorse online

Consigliamo di usare [trinket](https://trinket.io/) per scrivere HTML e CSS online. Questo progetto contiene i seguenti trinket:

+ [Punto di partenza per "Sorgere del sole"](https://trinket.io/html/web-sunrise)

I bambini possono anche utilizzare questo trinket vuoto [(jumpto.cc/html-blank)](http://jumpto.cc/html-blank) per scrivere il proprio HTML e CSS oppure questo modello trinket [(jumpto.cc/html-template)](http://jumpto.cc/html-template).

È disponibile anche un trinket con esempi di soluzioni alle sfide:

+ ["Sorgere del sole" completato](https://trinket.io/html/abcc0284a3)

#Risorse offline
Questo progetto può essere [completato offline](../offline.html) se preferito. È possibile accedere alle risorse del progetto facendo clic sul link "Scarica materiali per il progetto". Il link apre la cartella "Risorse del progetto" che contiene le risorse necessarie ai bambini per completare il progetto offline. È bene assicurarsi che tutti i bambini abbiano accesso a una copia di queste risorse. Questa cartella contiene i seguenti file:

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

Una versione completa delle sfide di questo progetto è presente anche nella sezione "Risorse per i volontari", che contiene:

+ sunrise-finished/index.html
+ sunrise-finished/style.css
+ sunrise-finished/prefixfree.js
+ sunrise-finished/boat.png
+ sunrise-finished/sun.png
+ sunrise-finished/rainbow.png

#Obiettivi di apprendimento
+ Stile e animazione con il CSS:
	+ Introduzione della regola `@keyframes` per definire i passaggi di un'animazione.
	+ Rinforzare l'utilizzo delle proprietà per definire dimensioni, forma, posizione e colore degli elementi di una pagina web.

Questo progetto copre elementi contenuti nei seguenti filoni di [Raspberry Pi Digital Making Curriculum](http://rpf.io/curriculum):

+ [Progettazione di risorse 2D e 3D di base](https://www.raspberrypi.org/curriculum/design/creator).

#Sfide
+ "Animazione in diagonale" - modificare le proprietà dell'animazione `@keyframe` per usare left:;
+ "Migliorare il cielo" - aggiungere altri keyframes e impostare il background: (sfondo).
+ "Altre animazioni" - animare altre immagini o elementi utilizzando diverse proprietà CSS. 

#Domande frequenti

+ Questo progetto utilizza la libreria di javascript `prefixfree.js`, per consentire la compatibilità dell'animazione tra i browser. Se questa libreria non viene usata, i bambini che impiegano browser più vecchi dovranno dichiarare un'animazione per i browser, ad esempio:

```
animation: sky 10s infinite; 		  	//per tutti i browser più recenti
-webkit-animation: sky 10s infinite;  	// Per browser Webkit (Chrome, Safari...)
-moz-animation: sky 10s infinite;     	// Per browser Mozilla
-o-animation: sky 10s infinite;       	// Per browser Opera
-ms-animation: sky 10s infinite;		// Per browser Microsoft 
```
