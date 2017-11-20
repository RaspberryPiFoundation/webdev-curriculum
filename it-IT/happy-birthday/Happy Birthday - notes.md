---
title: Buon compleanno – Note per i volontari
---

#Introduzione:
In questo progetto, ai bambini verranno presentati i tag HTML e le proprietà CSS. Modificheranno inoltre i tag e le proprietà per creare il loro biglietto di auguri personalizzato.

#Risorse online

Si consiglia di utilizzare [trinket](https://trinket.io/) per scrivere in linguaggio HTML e CSS online. Questo progetto contiene i seguenti trinket:

+ [Punto di partenza per "Introduzione al linguaggio HTML e CSS" -- jumpto.cc/web-intro](http://jumpto.cc/web-intro)
+ [Punto di partenza per "Biglietto di auguri" -- jumpto.cc/web-card](http://jumpto.cc/web-card)

Per scrivere il proprio codice HTML e CSS, i bambini possono inoltre utilizzare il seguente trinket vuoto [(jumpto.cc/html-blank)](http://jumpto.cc/html-blank) oppure questo modello di trinket [(jumpto.cc/html-template)](http://jumpto.cc/html-template).

È disponibile anche un trinket con esempi di soluzioni alle sfide:

+ ["Biglietto di auguri" finito -- trinket.io/html/e996dc0380](https://trinket.io/html/e996dc0380)

#Risorse offline
Questo progetto può essere completato [offline](https://www.codeclubprojects.org/en-GB/resources/webdev-working-offline/) se preferito. È possibile accedere alle risorse del progetto facendo clic sul link "Project Materials" (Materiali per il progetto). Il link apre la sezione "Project Resources" (Risorse del progetto) che contiene le risorse necessarie ai bambini per completare il progetto offline. È bene assicurarsi che tutti i bambini abbiano accesso a una copia di queste risorse. Questa sezione contiene i seguenti file:

+ intro/index.html
+ template/template.html
+ template/style.css
+ birthday-card/index.html
+ birthday-card/style.css
+ birthday-card/script.js
+ birthday-card/10 x .png images

È inoltre presente una versione completata delle sfide di questo progetto nella sezione "Volunteer Resources" (Risorse per i volontari), che contiene:

+ birthday-card-finished/index.html
+ birthday-card-finished/style.css
+ birthday-card-finished/script.js
+ birthday-card-finished/rainbow.png
+ birthday-card-finished/dinosaur.png

(Tutte le risorse sopra indicate possono essere scaricate anche come file ".zip" di progetto e di volontario.)

#Obiettivi di apprendimento
+ Questo progetto rappresenta un’introduzione ai tag HTML e alle proprietà CSS, e consente ai bambini di modificare contenuto e stile.

Questo progetto copre elementi contenuti nei seguenti filoni di [Raspberry Pi Digital Making Curriculum](http://rpf.io/curriculum):

+ [Progettazione di risorse 2D e 3D di base](https://www.raspberrypi.org/curriculum/design/creator).

#Sfide
+ "Aggiungi un altro paragrafo" - aggiunta di un tag HTML a un documento;
+ "Aggiungi più stile" - modifica degli stili CSS;
+ "Crea un biglietto personalizzato" - modifica del codice HTML e CSS per creare un biglietto di auguri.

#Domande frequenti

+ Questo progetto utilizza la raccolta di javascript `prefixfree.js` per consentire la compatibilità delle animazioni tra browser. Qualora non fosse usata questa raccolta, i bambini che utilizzano browser di versioni precedenti dovranno dichiarare l’animazione del browser. Ad esempio:

```
animation: sky 10s infinite; 		  	//Per i browser più recenti
-webkit-animation: sky 10s infinite;  	//Per browser con Webkit (Chrome, Safari, ecc.)
-moz-animation: sky 10s infinite;     	//Per i browser Mozilla
-o-animation: sky 10s infinite;       	//Per i browser Opera
-ms-animation: sky 10s infinite;		//Per i browser Microsoft 
```
