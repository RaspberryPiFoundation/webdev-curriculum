---
title: Ricercato!
description: Impara a creare il tuo poster.
layout: project
notes: "Wanted - notes.md"
---

# Introduzione {.intro}

In questo progetto, imparerai a creare il tuo poster.

![screenshot](images/wanted-final.png)

# Passo 1: Dai stile al tuo poster { .activity}

Iniziamo a modificare il codice CSS del poster.

## Lista di controllo delle attività { .check}

+ Apri questo trinket: <a href="http://jumpto.cc/web-wanted" target="_blank">jumpto.cc/web-wanted</a>. 

	Il progetto dovrebbe apparire così:
	
	![screenshot](images/wanted-starter.png)

+ Clicca sul tab "style.css". Noterai che ci sono già proprietà CSS per il 'div' contenente le diverse parti del poster.

	```
	div {
		text-align: center;
	    overflow: hidden;
	    border: 2px solid black;
	    width: 300px;
    }	
	```

+ Iniziamo ad alterare la proprietà 'text-align' (allineamento del testo):

	```
	text-align: center;
	```
	
	Che succede quando cambi la parola 'center' (centro) a 'left' (sinistra) o 'right' (destra)?

+ E la proprietà 'border' (bordo)?

	```
	border: 2px solid black;
	```

	'2px' nel codice sopra significa 2 pixel. Cosa succede quando cambi '2px solid black' (2px nero tinta unita) per '4px dotted red' (4px rosso a puntini)?

+ Cambia la 'width' (larghezza) del poster a '400px'. Cosa succede al poster?

+ Aggiungiamo alcuni CSS per stabilire il colore di sfondo del poster. Vai alla fine della riga 5 del tuo codice e premi il tasto di ritorno, in modo da avere una nuova linea vuota.

	![screenshot](images/wanted-newline.png)

	Digita il seguente codice sulla tua nuova linea vuota:

	```
	background: yellow;
	```

	Assicurati di digitare il codice_esattamente_come è sopra. Dovresti notare che lo sfondo del `<div>` è adesso giallo.

	![screenshot](images/wanted-background.png)

## Sfida: Migliorare il tuo poster {.challenge}
Aggiungi la seguente proprietà CSS al tuo stile 'div':

```
border-radius: 40px;
```

Cosa fa questa proprietà? Cosa succede se cambi il numero nel codice qui sopra?

## Salva il progetto {.save}

# Passo 2: Dai stile alle tue immagini { .activity}

Miglioriamo lo stile dell'immagine nel poster.

## Lista di controllo delle attività { .check}

+ Al momento, non ci sono proprietà CSS per il tuo tag `<img>`, dunque aggiungiamone alcune!

	Per prima cosa, aggiungiamo il seguente codice sotto il CSS per il tuo 'div':

	```
	img {

	}
	```

	![screenshot](images/wanted-img-css.png)

+ Ora possiamo aggiungere proprietà CSS per le immagini tra le parentesi graffe `{` e `}`.

	Per esempio, aggiungi questo codice tra le parentesi graffe per stabilire la larghezza dell'immagine:

	```
	width: 100px;
	```

	Vedrai che la misura dell'immagine cambia, in modo che la sua larghezza diventi di 100 pixel.

	![screenshot](images/wanted-img-width.png)

+ Puoi anche aggiungere un bordo attorno all'immagine con questo codice:

	```
	border: 1px solid black;
	```

+ Hai notato che non c'è molto spazio tra l'immagine e il bordo?

	![screenshot](images/wanted-img-border.png)

	Puoi risolvere il problema aggiungendo dell'imbottitura attorno all'immagine:

	```
	padding: 10px;
	```

	Padding (imbottitura) è lo spazio tra il contenuto (in questo caso un'immagine) e il suo bordo.

	![screenshot](images/wanted-img-padding.png)

	Cosa succederebbe, secondo te, se cambiassi l'imbottitura a '50px'?

## Sfida: Migliorare la tua immagine {.challenge}
Puoi dare un colore di sfondo alla tua immagine? O un bordo arrotondato?

Puoi trovare altri nomi di colori CSS a <a href="http://jumpto.cc/colours" target="_blank">jumpto.cc/colours</a>.

## Salva il progetto {.save}

# Passo 3: Dare stile all'intestazione { .activity .new-page }

Miglioriamo lo stile dell'intestazione `<h1>`.

## Lista di controllo delle attività { .check}

+ Aggiungiamo il seguente codice sotto il CSS della tua immagine:

	```
	h1 {

	}
	```

	Qui è dove aggiungerai proprietà CSS per la tua intestazione principale `<h1>`.

+ Per cambiare la fonte della tua intestazione `<h1>`, aggiungi il seguente codice tra parentesi graffe:

	```
	font-family: Impact;
	```

+ Puoi anche cambiare la misura dell'intestazione:

	```
	font-size: 50pt;
	```

+ Hai notato che c'è una grande spazio tra l'intestazione `<h1>` e il resto degli elementi attorno a essa?

	![screenshot](images/wanted-h1-margin.png)

	Questo succede perché c'è un margine attorno all'intestazione. Un margine è lo spazio tra l'elemento (in questo caso l'intestazione) e il resto delle cose attorno a esso.

	Puoi rimpicciolire il margine con questo codice:

	```
	margin: 10px;
	```

	![screenshot](images/wanted-h1-margin-small.png)

+ Puoi anche sottolineare la tua intestazione:

	```
	text-decoration: underline;
	```

## Sfida: Rendi bellissimo il tuo poster! {.challenge}
Aggiungi altri codici CSS per personalizzare le intestazioni `<h3>` e i paragrafi. 

![screenshot](images/wanted-final.png)

Ecco una lista di alcune delle proprietà CSS che puoi usare:

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

## Salva il progetto {.save}

## Sfida: Pubblicizza un evento! {.challenge}
Puoi creare un poster per un evento che avrà luogo nella tua scuola? Potrebbe essere uno spettacolo teatrale, un evento sportivo o perfino un poster che pubblicizzi il tuo Code Club!

## Salva il progetto {.save}
