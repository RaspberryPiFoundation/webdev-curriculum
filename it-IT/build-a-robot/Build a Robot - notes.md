---
title: Costruire un robot – Note per i volontari
---

#Introduzione:
In questo progetto, i bambini impareranno il posizionamento CSS costruendo il proprio robot.

#Risorse online

Si consiglia di utilizzare [trinket](https://trinket.io/) per scrivere in linguaggio HTML e CSS online. Questo progetto contiene i seguenti trinket:

+ [Punto di partenza per "Costruire un robot" -- jumpto.cc/web-robot](http://jumpto.cc/web-robot)

Per scrivere il proprio codice HTML e CSS, i bambini possono inoltre utilizzare il seguente trinket vuoto [(jumpto.cc/html-blank)](http://jumpto.cc/html-blank) oppure questo modello di trinket [(jumpto.cc/html-template)](http://jumpto.cc/html-template).

È disponibile anche un trinket con esempi di soluzioni alle sfide:

+ ["Costruire un robot" finito -- trinket.io/html/00736c0e18](https://trinket.io/html/00736c0e18)

#Risorse offline
Questo progetto può essere completato [offline](https://www.codeclubprojects.org/en-GB/resources/webdev-working-offline/) se preferito. È possibile accedere alle risorse del progetto facendo clic sul link "Project Materials" (Materiali per il progetto). Il link apre la sezione "Project Resources" (Risorse del progetto) che contiene le risorse necessarie ai bambini per completare il progetto offline. È bene assicurarsi che tutti i bambini abbiano accesso a una copia di queste risorse. Questa sezione contiene i seguenti file:

+ template/index.html
+ template/style.css
+ robot/index.html
+ robot/style.css
+ Lots of .png images

È inoltre presente una versione completata delle sfide di questo progetto nella sezione "Volunteer Resources" (Risorse per i volontari), che contiene:

+ robot-finished/index.html
+ robot-finished/style.css
+ robot-finished/Lots of .png images

(Tutte le risorse sopra indicate possono essere scaricate anche come file ".zip" di progetto e di volontario.)

#Obiettivi di apprendimento
+ Attributo id in HTML;
+ Scrittura di CSS:
	+ Selettore id `#`;
	+ posizionamento;
	+ in alto;
	+ a sinistra.

Questo progetto copre elementi contenuti nei seguenti filoni di [Raspberry Pi Digital Making Curriculum](http://rpf.io/curriculum):

+ [Progettazione di risorse 2D e 3D di base](https://www.raspberrypi.org/curriculum/design/creator).

#Sfide
+ "Progetta il tuo robot" - applicazione del posizionamento CSS per la creazione di un robot;
+ "Aggiungi le tue immagini" - aggiunta di altre immagini, con un attributo id in HTML e CSS associato.

#Completamento del progetto offline
Se i bambini completano il progetto offline, dovranno salvare le immagini che intendono utilizzare nella stessa cartella del file "Robot.html".

Possono quindi semplicemente aggiungere il nome del file nei tag `<img>`:

```
<img id="hat" src="hat.png" />
```