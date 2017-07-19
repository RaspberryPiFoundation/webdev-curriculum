---
title: Baue einen Roboter
description: Lerne, wie du Bilder positionierst, um deinen eigenen Roboter herzustellen.
layout: project
notes: "Build a Robot - notes.md"
---

# Einführung { .intro}

In diesem Projekt lernst du, wie du Bilder positionierst und deinen eigenen Roboter herstellst!

![screenshot](images/robot-final.png)

# Schritt 1: Gib deinem Roboter Augen { .activity}

Lass uns deinem Roboter Augen geben!

## Aufgaben-Checkliste { .check}

+ Dieses Trinket öffnen: <a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a>.

    Das Projekt sollte so aussehen:

	![screenshot](images/robot-starter.png)

+ Jedes Bild in diesem Projekt hat seinen eigenen Namen (bzw. seine eigene __ID__). Zum Beispiel das HTML für die Bilder für Gesicht Augen („Gesicht“, „Auge1“ und „Auge2“ beginnend in Zeile 8 deines Codes) sieht so aus:

```
<img id="face" ...> (Gesicht)
<img id="eyes1" ...> (Auge1)
<img id="eyes2" ...> (Auge1)
```

+ Du kannst die ID eines Bildes benutzen, um ihm mit Hilfe des Rautensymbols `#` seinen eigenen Stil zu verleihen. Dies ermöglicht dir, jedes Bild einzeln zu stylen.

Klicke auf die `style.css` Datei. Siehst du, wie die Größe des Robotergesichts und die der anderen Bilder unterschiedlich ist?

![screenshot](images/robot-id.png)

+ Füge diesen CSS-Code hinzu, um die Augen des Roboters zu stylen:

```
#Auge1 {
    Breite: 200px;
}
```

Siehst du, dass du nur das `eyes1` (Auge1) Bild mit Hilfe von `#eyes1` (#Auge1)in deinem CSS-Code stylst? Wenn du magst, kannst du statt dessen `#eyes2` (#Auge2) oder `#eyes3` (#Auge3) benutzen! 

![screenshot](images/robot-eyes-width.png)

+ Siehst du, wie jedes Bild – eins nach dem anderen – dargestellt wird? Dies nennt sich __relative__ Positionierung. Wenn du dem Browser exakt sagen willst, wo die Augen deines Roboters platziert werden sollen, musst du statt dessen die __absolute__ Positionierung benutzen.

Füge diese 3 Zeilen an Code zum CSS für dein `eyes1` (Auge1) Bild hinzu:

```
Position: absolut;
oben: 200px;
links: 100px;
```

Du solltest sehen können, dass die Augen des Roboters sich nun zum richtigen Platz auf deinem Roboter bewegen.

![screenshot](images/robot-eyes-position.png)

Dieser CSS-Code teilt dem Browser mit, wie weit von oben / links von der Webseite, das Bild angezeigt werden soll.

![screenshot](images/robot-eyes-position2.png)

Du kannst auch `bottom` (unten) anstatt von `top` (oben) benutzen, um dem Browser mitzuteilen, wie weit von unten vom Bildschirm der Abstand sein soll, bzw. du kannst auch genauso gut `right` (rechts) anstatt von `left` (links) benutzen.

# Schritt 2: Gib deinem Roboter einen Mund { .activity}

Lass uns deinem Roboter einen Mund geben!

## Aufgaben-Checkliste { .check}

+ Füge den folgenden CSS-Code hinzu, um dein `mouth1` (Mund1) Bild zu bearbeiten:

```
#Mund1 {
    Breite: 50px;
    Position: absolut;
    oben: 200px;
    links: 200px;
}
```

+ Der Mund deines Roboters sieht sehr klein aus und ist nicht am richtigen Platz.

![screenshot](images/robot-mouth.png)

Kannst du das beheben, indem du die entsprechenden Änderungen an deinem CSS-Code vornimmst?

## Projekt speichern {.save}

##Aufgabe: Konzipiere deinen eigenen Roboter {.challenge}
Benutze das, was du gelernt hast, um deinen eigenen Roboter zu konzipieren. Hier sind ein paar Beispiele, wie dein Roboter aussehen könnte:

![screenshot](images/robot-examples.png)

## Projekt speichern {.save}

##Aufgabe: Füge deine eigenen Bilder hinzu {.challenge}
Kannst du weitere Bilder finden, die du zu deinem Roboter hinzufügen kannst, und kannst du sie entsprechend auf deiner Webseite positionieren? Du könntest auch das Gesicht des Roboters gegen dein eigenes austauschen!

```
<img id="face" src="myFace.png"> 
```

## Projekt speichern {.save} 
