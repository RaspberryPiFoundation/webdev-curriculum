---
title: Alles Gute zum Geburtstag
level: HTML & CSS 1
language: de-AT
embeds: "*.png"
materials: ["Club LeiterUnterlagen/*.*","Project Unterlagen/*.*"]
stylesheet: web
...

# Einleitung { .intro}

In diesem Projekt wirst du die Grundlagen von HTML & CSS kennenlernen, indem du lernst eine individuelle Geburtstagskarte zu machen.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/e996dc0380?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="birthday-final.png">
</div>

# Schritt 1: Was ist HTML? { .activity}

HTML steht für __HyperText Markup Language__, und ist die Sprache um Webseiten zu machen. Schauen wir uns ein Beispiel an!

## Arbeits-Checkliste { .check}

+ Um HTML zu schreiben wirst du eine Website namens Trinket benutzen. Öffne dieses Trinket: <a href="http://jumpto.cc/web-intro" target="_blank">jumpto.cc/web-intro</a>. Wenn du das online liest, kannst du auch die eingebettete Version dieses Trinkets weiter unten benutzen.

<div class="trinket">
	<iframe src="https://trinket.io/embed/html/850a678202" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
	</iframe>
</div>

+ Der Code, den du auf der linken Seite des Trinket sehen kannst ist HTML. Auf der rechten Seite siehst du die Web-Seite, die der HTML-Code erzeugt hat.

	HTML verwendet __'tags'__ um Web-Seiten zu erzeugen. Siehst du das HTML in Zeile 8 deines Codes?

	```
	<p>Hi. My name is Andy.</p>
	```

	`<p>` ist ein Beispiel für einen 'tag', und es ist eine Abkürzung für __paragraph__ (das bedeutet Absatz). Du kannst einen Absatz mit `<p>` beginnen und mit `</p>` den Absatz beenden.

+ Findest du noch andere 'tags'? Ein anderer 'tag', den du gefunden haben könntest, ist `<b>` in Zeile 9 , das für __bold__ steht (Fettschrift):

	```
	<b>running</b>
	```

	Hier sind noch einige:

	+ `<html>` und `</html>` markieren den Start und das Ende des HTML-Dokuments;
	+ `<head>` und `</head>` ist der Platz für Dinge wie CSS (dazu kommen wir später!);
	+ `<body>` und `</body>` ist der Platz für den Inhalt deiner Web-Seite.

	![screenshot](birthday-head-body.png)

+ Ändere etwas in einem der Textabsätze in HTML (auf der linken Seite). Klicke 'Run' und du solltest die Änderung auf deiner Web-Seite sehen (auf der rechten Seite)!

	![screenshot](birthday-edit-html.png)

+ Wenn du einen Fehler gemacht hast und alle deine Änderungen rückgängig machen willst, kannst du die Schaltfläche 'Menü' klicken und auf 'Reset' klicken. Probier es mal!

	![screenshot](birthday-reset.png)

## Projekt speichern {.save}

__Du brauchst kein Trinket-Konto um deine Projekte zu speichern!__ 

Wenn du kein Trinket-Konto hast, klicke den Pfeil nach unten und klicke dort auf 'Link'. Das zeigt dir einen Link, den du speichern kannst, und mit dem du später zurückkommen kannst. Das musst du jedes mal machen, wenn du Änderungen gemacht hast, da der Link sich dadurch ändert!

![screenshot](birthday-link.png)

Wenn du ein Trinket-Konto hast, dann klicke einfach auf die Schaltfläche 'Remix' in der Kopfzeile des Trinket um deine Web-Seite zu speichern. Das speichert eine Kopie des Trinkets in deinem Profil.

![screenshot](birthday-remix.png)

##Aufgabe: Füge einen Absatz hinzu {.challenge}
Kannst du einen dritter Absatz unter den beiden anderen zu deiner Web-Seite hinzufügen? Denk daran, dass dein neuer Absatz mit einem `<p>` 'tag' beginnen muss, und mit `</p>` endet.

So sollte deine Web-Seite jetzt aussehen:

![screenshot](birthday-paragraph.png)

Kannst du __fetten__ und <u>unterstrichenen</u> Text zu deinem neuen Absatz hizufügen? Du solltest `<u>` und `</u>` für unterstrichenen Text verwenden.

## Projekt speichern {.save}

# Schritt 2: Was ist CSS? { .activity}

CSS steht für __Cascading Style Sheets__ (gestufte Gestaltungsbögen), und ist die Sprache um Web-Seiten zu gestalten und nett aussehen zu lassen. Im `<head>`-Abschnitt eines HTML-Dokuments kannst du es so mit einer CSS-Datei verlinken:

![screenshot](birthday-css-link.png)

## Arbeits-Checkliste { .check}

+ CSS listet alle __properties__ (Eigenschaften) eines gewissen 'tags' auf. Klicke auf den Reiter 'style.css' um das CSS für deine Web-Seite zu sehen.

	![screenshot](birthday-css-tab.png)

+ Finde diesen Code:

	```
	p {
		color: black;
	}
	```

	Dieser CSS-Code hat eine Eigenschaft für Absätze, die die Schriftfarbe auf schwarz setzt.

+ Ändere das Wort 'black' im CSS zu 'blue'. Nun solltest du sehen, dass die Farbe aller Absätze auf blau geändert wird.

	![screenshot](birthday-edit-css.png)

## Projekt speichern {.save}

##Aufgabe: Mehrere Stile hinzufügen {.challenge}
Kannst du die Textabsätze orange (orange) machen? Oder den Hintergrund grau (grey)?

![screenshot](birthday-more-style.png)

## Projekt speichern {.save}

# Schritt 3: Eine Gebutstagskarte machen { .activity}

Lass uns das, was du über HTML und CSS gelernt hast verwenden um deine individuelle Geburtstagskarte zu machen.

## Arbeits-Checkliste { .check}

+ Öffne dieses Trinket: <a href="http://jumpto.cc/web-card" target="_blank">jumpto.cc/web-card</a>, oder verwende die eingebettete Version weiter unten, falls du dies online liest.

<div class="trinket">
	<iframe src="https://trinket.io/embed/html/90506676c9" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
	</iframe>
</div>

Mach dir keine Sorgen, falls du nicht den gesamten Code verstehst. Diese Geburtstagskarte sieht ziemlich fade aus. Du solltest einige Änderungen an diesem HTML und am CSS machen.

+ Klicke die Schaltfläche auf der Vorderseite der Karte, und sie sollte sich öffnen und die Innenseite zeigen. 

	![screenshot](birthday-click.png)

+ Gehe zu Zeile 13 des Codes. Wie in dem früheren Beispiel kannst du jeden Text im HTML ändern um deine Karte anzupassen.

	![screenshot](birthday-card-html.png)

+ Findest du das HTML für das Roboter-Bild? (Tipp: es ist auf Zeile 16!) Ändere das Wort `robot` zu `sun`, und du siehst, dass sich das Bild ändert!

	![screenshot](birthday-card-sun.png)

	Du kannst jedes der Wörter `boy`, `diamond`, `dinosaur`, `flowers`, `girl`, `rainbow`, `robot`, `spaceship`, `sun`, `tea`, oder `trophy` probieren.

+ Du kannst auch das CSS der Geburtstagskarte ändern. Klicke auf den Reiter “style.css”. Es beginnt mit dem CSS für die `outside` (Außenseite) der Karte. Ändere die `background-color` (Hintergrundfarbe) auf `lightgreen` (hellgrün).

	![screenshot](birthday-card-outside.png)

+ Du kannst auch die größe eines Bildes ändern. Gehe zu Zeile 29 des CSS, und ändere die `width` (Breite) und `height` (Höhe) des Bildes auf der Außenseite zu `200px` (`px` steht for pixels - Bilpunkte).

	![screenshot](birthday-card-size.png)	

+ Die Schrift kann auch geändert werden. Gehe zu Zeile 24 und ändere die `font-family` (Schriftfamilie) zu `Comic Sans MS` und die `font-size` (Schriftgröße) zu `16pt`.

	![screenshot](birthday-card-font.png)

	Du kannst auch andere Schriften verwenden wie: <span style="font-family: Arial;">arial</span>, <span style="font-family: impact;">Impact</span> and <span style="font-family: tahoma;">Tahoma</span>. 

## Projekt speichern {.save}

##Aufgabe: Mache eine personalisierte Karte {.challenge}
Verwende alles, was du über HTML und CSS gelernt hast, um deine personalisierte Karte zu vollenden. Es muss auch keine Geburtstagskarte sein, jeder beliebige Anlass ist möglich.

Hier ist ein Beispiel:

![screenshot](birthday-final.png)

## Projekt speichern {.save}

Jetzt, wo du deine Karte fertig gestellt hast, kannst du sie teilen oder per e-mail an jemanden schicken.

![screenshot](birthday-share.png)
