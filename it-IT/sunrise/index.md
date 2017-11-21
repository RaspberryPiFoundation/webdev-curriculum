---
title: Sorgere del sole
description: "Crea l'animazione del sorgere del sole." 
layout: project
notes: "Sunrise - notes.md"
...

# Introduzione {.intro}

In questo progetto, imparerai a usare il CSS per creare l'animazione del sorgere del sole.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/abcc0284a3?outputOnly=true&start=result" width="600" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="images/sunrise-final.png">
</div>

# Passo 1: Creazione del sole { .activity}

Iniziamo aggiungendo un'immagine del sole e posizionandola con il CSS.

## Lista di controllo delle attività { .check}

+ Apri questo trinket: <a href="http://jumpto.cc/web-sunrise" target="_blank">jumpto.cc/web-sunrise</a>.

    Il progetto dovrebbe avere questo aspetto:

	![screenshot](images/sunrise-starter.png)

+ Guarda nel `body` del file `index.html`e troverai gli elementi `div` per il cielo e il mare.

    ```
    <div id="sky">
    </div>

    <div id="sea">
    </div>
    ```

+ Un'immagine del sole è già inclusa nel progetto.

    Aggiungi l'immagine del `div` del sole includendo un id in modo da applicare uno stile:

    ![screenshot](images/sunrise-sun-image.png)

+ Aspetta, l'immagine è molto grande. Vai a `style.css` e aggiungi il CSS per impostare l'altezza dell'immagine:

    ![screenshot](images/sunrise-sun-height.png)

    Nota che l'altezza è aggiornata automaticamente per mantenere le stesse proporzioni.

+ Infine, aggiungiamo il codice per posizionare il sole:

    ![screenshot](images/sunrise-sun-position.png)


## Salva il progetto {.save}

# Passo 2: Animare il sorgere del sole { .activity}

Per animare il sorgere del sole, è necessario definire come si sposta e il tempo impiegato.

per farlo, è necessario definire un elenco di __key frames__. Ogni key frame (fotogramma chiave) definisce le proprietà CSS di un elemento in un punto particolare dell'animazione.

## Lista di controllo delle attività { .check}

+ Anzitutto è necessario usare `@keyframes` per creare una nuova animazione denominata sorgere del sole.

    Aggiungi questo codice CSS al termine del file `style.css`:

    ```
    @keyframes sunrise {
        0% {top: 90%;}
        100% {top: 0;}
    }
    ```

    Questo codice dice al sole dove posizionarsi all'inizio (`0%`) e alla fine (`100%`) dell'animazione.

    Dal momento che il sole è nel cielo`div`, le posizioni `top` (alto) e `left` (sinistra) date da te si trovano nel cielo, in cui `top: 100%` indica il fondo del cielo, e non della pagina web.


+Ora che hai creato l'animazione `sunrise` non ti rimane che dire al sole di usarla!

    Aggiungi il codice evidenziato al CSS del tuo sole:

    ![screenshot](images/sunrise-sunrise.png)

    In questo modo dici al sole di impiegare 10 secondi per l'animazione.

+ Per eseguire nuovamente l'animazione nel Trinket, fai clic su **Autorun**.

## Salva il progetto {.save}

##Sfida: Animazione diagonale {.challenge}
Puoi aggiungere codice alla tua animazione `sunrise`, per fare in modo che il sole sorga in basso a sinistra del cielo e si sposti in diagonale nella sua posizione, più o meno in alto al centro?

Puoi aggiungere la proprietà `left` (sinistra) per farlo, ad esempio:

```
sinistra: 40%;
```

![screenshot](images/sunrise-left.png)

## Salva il progetto {.save}


# Passo 3: Animazione infinita { .activity}

Facciamo in modo che l'animazione si ripeta all'infinito.

## Lista di controllo delle attività { .check}

+ Se vuoi che il sole sorga e poi tramonti, aggiungiamo altri key frame alla tua animazione:


    ```
    @keyframes sunrise {
        0%   {top:90%; left:0;}
        33%  {top:0; left:40%; }
        66%  {top:0; left:40%; }
        100% {top:90%; left:80%; }
    }
    ```

    Ciò significa che l'animazione inizia e finisce con il sole in fondo al cielo, e rimane nella parte superiore dal 33% al 66% dell'animazione.

+ Ora devi solo aggiungere la parola `infinite` (infinito) all'animazione `#sun` per fare in modo che si ripeta sempre:

    ![screenshot](images/sunrise-infinite.png)

+ Fai un test della tua animazione. Il sole continua a sorgere e tramontare?


## Salva il progetto {.save}

# Passo 4: Anima il cielo { .activity}

L'animazione non riguarda solo il movimento. Facciamo in modo che il cielo diventi scuro la notte.

## Lista di controllo delle attività { .check}

+ Aggiungi un'animazione chiamata `sky` (cielo) al CSS:

    ```
    @keyframes sky {
        0% {background: black}
        100% {background: lightblue}
    }
    ```

    Nota: questa volta stai animando il colore del cielo, e non la posizione.

+ Aggiungi codice al cielo, per dirgli di usare la nuova animazione:

    ```
    animation: sky 10s;
    ```

    ![screenshot](images/sunrise-sky.png)

+ Fai clic su **Autorun** per provare l'animazione.

## Salva il progetto {.save}

##Sfida: Migliora il cielo {.challenge}

Puoi cambiare l'animazione del cielo in modo che corrisponda al sole e rimanga azzurro durante il giorno e diventi scuro al tramonto. Fai in modo che si ripeta all'infinito.

![screenshot](images/sunrise-sky-challenge.png)

##Sfida: Altre animazioni {.challenge}

Riesci ad animare un'altra immagine? Puoi animare la posizione, il colore, la forma, le dimensioni, l'opacità (la possibilità di vedere attraverso) o qualsiasi altra cosa ti venga in mente. Puoi anche provare a cambiare la quantità di tempo in cui le animazioni vengono eseguite.

Per ciascun elemento che vuoi animare, dovrai:

+ Includerlo nell'HTML con un id
+ Aggiungere uno stile per l'id
+ Creare una regola @keyframes
+ Usare `animation:` nello stile per usare l'animazione definita con @keyframes

Fare clic sull'icona dell'immagine per vedere le immagini incluse nel progetto:

![screenshot](images/sunrise-images.png)

Puoi anche caricare una tua immagine, se vuoi.

Non dimenticare che puoi inserire elementi nel mare e nel cielo:

![screenshot](images/sunrise-boat.png)

Nell'esempio, l'arcobaleno impiega l'opacità per un effetto sfumato:

```
@keyframes fade {
  0%   {opacity: 0;}
  50%  {opacity: 100;}
  66%  {opacity: 0;}
  100%   {opacity: 0;}
}
```

La barca utilizza una posizione di partenza negativa in modo che tu non possa vederla per una parte dell'animazione:

```
 @keyframes left-right {
  0%    {left:-50%;}
  100%  {left:200%;}
}
```

## Salva il progetto {.save}
