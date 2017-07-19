---
title: Tell a Story 
description: Erstelle eine Webseite, um eine Geschichte, einen Witz oder ein Gedicht zu erzählen.
layout: project
notes: "Tell a Story - notes.md"
project-type: sample
---

# Einführung { .intro}

In diesem Projekt lernst du, wie du deine eigene Webseite erstellst, um eine Geschichte, einen Witz oder ein Gedicht zu erzählen.

![screenshot](images/story-final.png)

# Schritt 1: Denk dir eine Geschichte aus { .activity}

Bevor du mit dem Programmieren beginnst, musst du dir eine Geschichte ausdenken, bzw. auswählen, welche du erzählen willst.

## Aufgaben-Checkliste { .check}

+ Denke ein wenig über die Geschichte nach. Es könnte:
	+ eine berühmte Geschichte sein;
	+ eine Geschichte sein, die du erfunden hast;
	+ etwas sein, das entweder dir oder einem Freund/einer Freundin passiert ist.

	Es muss nicht unbedingt eine Geschichte sein. Es könnte auch ein Witz oder ein Gedicht sein oder etwas ganz anderes, das du erzählen willst!

# Schritt 2: Die Geschichte bearbeiten { .activity}

Lass uns damit beginnen, den HTML Inhalt und CSS Stil der Geschichten-Webseite zu bearbeiten.

## Aufgaben-Checkliste { .check}

+ Dieses Trinket öffnen: <a href="http://jumpto.cc/web-story" target="_blank">jumpto.cc/web-story</a>. 

	Das Projekt sollte so aussehen:
	
	![screenshot](images/story-starter.png)

+ Du wirst dich vielleicht noch an das 'Happy Birthday' Projekt erinnern: Der Webseiteninhalt kommt in den `<body>` (Body, bzw. Hauptteil) des HTML Dokuments.

	Gehe zu Zeile 7 des Codes und du solltest den Webseiteninhalt, der sich in den `<body>` und den `</body>` Tags befindet, sehen können.

	![screenshot](images/story-html.png)

+ Kannst du unterscheiden, welche Tags benutzt werden, um die verschiedenen Komponente der Webseite zu erstellen?

	![screenshot](images/story-elements.png)

	+ `<h1>` ist eine __Überschrift__. Du kannst die Zahlen von 1 bis 6 benutzen, um Überschriften in unterschiedlichen Größen zu erstellen;
	+ `<div>` ist eine Abkürzung für __Division__ (bzw. Teilung) und ist eine Methode, um Dinge zusammen zu gruppieren. Bei dieser Webseite wirst du es benutzen, um alle Dinge für jeden Aspekt deiner Geschichte zusammen zu gruppieren;
	+ `<img>` ist ein __Bild__ (bzw. „Image“);
	+ `<p>` ist ein __Absatz__ (bzw. „Paragraph“) von Text.

##Aufgabe: Nimm ein paar Veränderungen vor {.challenge}
Bearbeite den HTML und den CSS Code, um deine Webseite speziell und eigen anzufertigen.

![screenshot](images/story-changes.png)

Du kannst die Farben ändern, die auf der Webseite benutzt werden, und du kannst auch folgende Schriftgrößen benutzen <span style="font-family: Arial;">Arial</span>, <span style="font-family: Comic Sans MS;">Comic Sans MS</span>, <span style="font-family: Impact;">Impact</span> and <span style="font-family: Tahoma;">Tahoma</span>.

Du findest weitere CSS Farbnamen unter <a href="http://jumpto.cc/colours" target="_blank">jumpto.cc/colours</a>.

Falls du weitere Hilfestellung benötigst, kannst du dich auf das 'Happy Birthday' Projekt beziehen.

## Projekt speichern {.save}

# Schritt 3: Eine Geschichte erzählen { .activity}

Lass uns einen zweiten Teil zu deiner Geschichte hinzufügen.

## Aufgaben-Checkliste { .check}

+ Gehe zu Zeile 15 des Codes und füge ein weiteres Set von `<div>` und `</div>` Start- und End-Tags hinzu. Dies erstellt ein neues Kästchen für den nächsten Teil deiner Geschichte.

	![screenshot](images/story-div.png)

+ Füge einen Textabsatz innerhalb deines neuen `<div>` Tags hinzu.

	```
	<p>Noch mehr Text hier!</p>
	```

	![screenshot](images/story-paragraph.png)

+ Zum Schluss kannst du ein Bild zu deinem neuen Kästchen hinzufügen, indem du diesen Code innerhalb deines `<div>` Tags hinzufügst:

	```
	<img src="">
	```

	![screenshot](images/story-img-tag.png)

	Beachte bitte, dass die `<img>` Tags etwas anders als die anderen Tags sind, weil sie keinen End-Tag besitzen.

+ Bei HTML Bildern musst du die __Quelle__ des Bildes innerhalb der Anführungszeichen hinzufügen. 

	Klicke auf das Bildsymbol, um zu sehen, welche Bilder dir für deine Geschichte zur Verfügung stehen.

	![screenshot](images/story-see-images.png)

+ Finde den Namen eines Bildes, das du hinzufügen möchtest, z. B. `buildings.png` (Gebäude). Du kannst dann auf `index.html` klicken, um wieder zurück zu deinem Code zu gelangen.

	![screenshot](images/story-image-name.png)

+ Du kannst dann den Namen des Bildes zwischen den Anführungszeichen in deinem `<img>` Tag hinzufügen.

	```
	<img src="buildings.png">
	```

	![screenshot](images/story-image-name-add.png)

# Schritt 4: Finde deine eigenen Bilder { .activity}

Lass uns ein Bild aus dem Internet finden, um es zu deiner Geschichte hinzuzufügen.

## Aufgaben-Checkliste { .check}

+ Gehe zu <a href="http://jumpto.cc/html-images" target="_blank">jumpto.cc/html-images</a> und finde ein Bild, das du mit in deine Geschichte einbeziehen möchtest.

+ Klicke mit der rechten Maustaste auf das Bild und klicke auf 'Copy image URL' (Bild URL kopieren). Das __URL__ ist die Bildadresse.

	![screenshot](images/story-url.png)

+ Füge das URL zwischen den Anführungszeichen in deinem `<img>` Tag ein. Du solltest jetzt sehen können, wie dein Bild erscheint!

	![screenshot](images/story-image.png)

## Projekt speichern {.save}

# Schritt 5: Bilder hochladen { .activity}

__Wenn du ein Trinket Konto hast__, kannst du auch deine eigenen Bilder zur Webseite hochladen!

## Aufgaben-Checkliste { .check}

+ Klicke auf das Bildsymbol oberhalb deines Trinkets und klicke dann auf 'Add Image' (Bild hinzufügen).

	![screenshot](images/story-upload.png)

+ Finde dein Bild auf deinem Computer und ziehe es mit der Maus in dein Trinket.

	![screenshot](images/story-drag.png)

+ Du brauchst dann nur noch den Namen deines neuen Bildes zwischen die Anführungszeichen in deinem `<img>` Tag einzufügen, so wie hier dargestellt:

	```
	<img src="buildings.png">
	```

## Projekt speichern {.save}

##Aufgabe: Mach weiter so! {.challenge}
Benutze das, was du in diesem Projekt gelernt hast, um deine Geschichte zu Ende zu erzählen! Hier ist ein Beispiel:

![screenshot](images/story-final.png)

## Projekt speichern {.save}
