---
title: Ricetta
description: "Crea una pagina web della tua ricetta preferita, in modo che i tuoi amici possano realizzarla!"
layout: project
notes: "Recipe - notes.md"
---

# Introduzione {.intro}

In questo progetto, imparerai a creare una pagina web della tua ricetta preferita.

![screenshot](images/recipe-final.png)

# Passo 1: Decidi una ricetta { .activity}

Prima di iniziare a programmare, devi scegliere una ricetta.

## Lista di controllo delle attività { .check}

+ Pensa un ricetta che vuoi condividere con gli amici. Può essere:
	+ Una ricetta che hai trovato online;
	+ Il tuo piatto preferito;
	+ Qualcosa che hai fatto!

La ricetta di esempio che trovi in questo progetto è un frappè di banana. Puoi copiare questa ricetta se non riesci a trovarla da solo.

# Passo 2: Ingredienti { .activity}

Ecco gli ingredienti necessari per la ricetta.

## Lista di controllo delle attività { .check}

+ Apri questo modello trinket: [jumpto.cc/html-template](http://jumpto.cc/html-template).

	Il progetto dovrebbe avere questo aspetto:

	![screenshot](images/recipe-starter.png)

+ Per l’elenco di ingredienti, userai un __elenco non ordinato__ con il tag `<ul>`. Vai alla linea 8 del modello e aggiungi questo HTML, sostituendo il testo nel titolo `<h1>` con il nome della tua ricetta.

```
<h1>Frappè di banana</h1>

<h3>Ingredienti:</h3>

<ul>

</ul>
```

+ Visualizza la pagina web e dovresti vedere due intestazioni.

![screenshot](images/recipe-headings.png)

Non vedrai ancora il tuo elenco poiché non hai ancora aggiunto nessun elemento!

+ Il prossimo passo è aggiungere elementi al tuo elenco utilizzando il tag `<li>`. Aggiungere il codice seguente nell’etichetta `<ul>`:

```
<li>1 banana</li>
```
![screenshot](images/recipe-ul.png)

Dato che l’elenco non è ordinato non ci sono numeri accanto agli elementi dell’elenco, solo punti.

##Sfida: Altri ingredienti {.challenge}
Puoi aggiungere tutti gli ingredienti la __tua__ ricetta?

La pagina web dovrebbe avere questo aspetto:

![screenshot](images/recipe-more-ingredients.png)

## Salva il progetto {.save}

# Passo 3: Metodo { .activity }

Ed ora spieghiamo come realizzare la ricetta.

## Lista di controllo delle attività { .check}

+ Ora utilizzeremo un altro elenco per scrivere il metodo, ma questa volta userai un __elenco ordinato__ con il tag `<ol>`.

Un elenco ordinato è un elenco numerato da utilizzare quando l’ordine dei passi è importante.

Aggiungi questo codice sotto all’elenco degli ingredienti, accertandoti che si trovi ancora all’interno del tag `<body>`:

```
<h3>Metodo:</h3>

<ol>

</ol>
```

![screenshot](images/recipe-method.png)

+ Ora devi solo aggiungere elementi dell’elenco nel nuovo elenco ordinato:

```
<li>Sbucciare la banana e metterla in un frullatore</li>
```

![screenshot](images/recipe-ol.png)

Nota che gli elementi dell’elenco sono numerati automaticamente!

##Sfida: Altri passi {.challenge}
Puoi aggiungere tutti i passi per realizzare la __tua__ ricetta?

Il metodo dovrebbe avere questo aspetto:

![screenshot](images/recipe-more-method.png)

## Salva il progetto {.save}

# Passo 4: Colori! { .activity}

Aggiungiamo un po’ di colore alla pagina web con la tua ricetta.

## Lista di controllo delle attività { .check}

+ Hai già imparato come aggiungere testo colorato a una pagina web. Aggiungi questo codice all’interno del file `style.css`per rendere blu tutto il testo nel corpo del sito web:

```
body {
    color: blue;
}
```

![screenshot](images/recipe-blue.png)

+ Il browser conosce colori come `blue` (blu), `yellow` (giallo) e anche `lightgreen` (verde chiaro), ma lo sapevi che in realtà conosce i __nomi__ di oltre 140 colori?

Ecco un elenco di tutti i nomi di colori che puoi usare: [jumpto.cc/colours](http://jumpto.cc/colours), che include nomi di colori come `tomato`(pomodoro), `firebrick` (mattone) e `peachpuff`(pesca).

Cambia il colore del testo da `blue` (blu) a `tomato` (pomodoro).

![screenshot](images/recipe-tomato.png)

+ Il tuo browser conosce i nomi di 140 colori, ma in realtà conosce i __valori__ di oltre 16 milioni di colori!


Per dire al browser quale colore visualizzare, basta sapere la quantità di rosso, verde e blu da usare.

Le quantità di rosso, verde e blu sono scritte come un numero compreso tra `0` e `255`.

![screenshot](images/recipe-rgb-img.png)

Aggiungi questo codice al CSS per cambiare il colore del corpo della pagina web e visualizzare uno sfondo giallo:

```
background: rgb(250,250,210);
```

![screenshot](images/recipe-rgb.png)

+ Se preferisci, puoi dire al browser quale colore mostrare utilizzando un codice esadecimale (o __hex code__). Funziona in modo simile al codice `rgb()` qui sopra, eccetto che i codici esadecimali iniziano sempre con una `#`, e utilizzano "numeri" esadecimali compresi tra `00` e `ff` per la quantità di rosso, verde e blu.

![screenshot](images/recipe-hex-img.png)

Sostituisci il codice `rgb()` nel CSS con questo codice esadecimale:

```
background: #fafad2;
```

![screenshot](images/recipe-hex.png)

Dovresti vedere la stessa tonalità giallo chiaro di prima!

## Salva il progetto {.save}

# Passo 5: Il tocco finale { .activity}

Aggiungiamo un po’ di HTML e CSS per migliorare la pagina web.

## Lista di controllo delle attività { .check}

+ Puoi aggiungere una linea orizzontale al termine della ricetta utilizzando il tag `<hr>`.

![screenshot](images/recipe-hr.png)

Nota: questo tag non ha un tag di fine, proprio come il tag `<img>`.

+ La linea che hai appena aggiunto non corrisponde allo stile del resto della pagina web. Correggiamo aggiungendo un po’ di codice CSS:

```
hr {
    height: 2px;
    border: none;
    background-color: tomato;
}
```

![screenshot](images/recipe-hr-css.png)

+ Puoi anche cambiare l’aspetto dei punti elenco con il codice CSS:

```
ul {
    list-style-type: square;
}
```

![screenshot](images/recipe-ul-css.png)

##Sfida: Altri colori! {.challenge}
Cambia i colori nel codice utilizzando i nomi dei colori, i valori `rgb()` e i codici esadecimali. C’è un elenco con moltissimi colori all’indirizzo <a href="http://jumpto.cc/colours" target="_blank">jumpto.cc/colours</a>, oppure puoi passare a <a href="http://jumpto.cc/colour-picker" target="_blank">jumpto.cc/colour-picker</a> e creare i tuoi colori personali!

Ecco alcuni esempi di colore:

+ Il rosso può essere scritto come:
	+ `red` (naturalmente!)
	+ `rgb(255,0,0)` (rosso intenso, senza verde né blu)
	+ `#ff0000`

+ Il verde oliva può essere scritto come:
	+ `olive`
	+ `rgb(128, 128, 0)` (un po’ di rosso e verde senza blu)
	+ `#808000`

Prova ad accertarti che i colori utilizzati stiano bene con la ricetta!

## Salva il progetto {.save}

##Sfida: Recensioni {.challenge}
Chiedi ad alcuni amici di lasciare una recensione per la tua ricetta. Avrai bisogno di un altro elenco per farlo.

![screenshot](images/recipe-reviews.png)

## Salva il progetto {.save}

##Sfida: Più stile {.challenge}
Riesci ad aggiungere un’immagine nella pagina web? Oppure a cambiare il tipo di carattere? Ecco come potrebbe apparire la tua pagina:

![screenshot](images/recipe-final.png)

Ecco del codice che può aiutarti:

```
font-family: Arial / Comic Sans MS / Courier / Impact / Tahoma;
font-size: 12pt;
font-weight: bold;

<img src="image-link-goes-here">
```

## Salva il progetto {.save}
