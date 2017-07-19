---
title: Sunrise - Notes for Club Leaders
---

#Einführung:
In diesem Projekt lernen die Kinder, wie man eine einfach Szene mit Hilfe von CSS animiert. Sie werden die CSS „@keyframes“ (Schlüsselbilder) Regel anwenden, um verschiedene Eigenschaften von Bildern und „div“ zu animieren.

#Online Ressourcen

Wir empfehlen [Trinket](https://trinket.io/) zu benutzen, um HTML und CSS online zu schreiben. Dieses Projekt enthält die folgenden Trinkets:

+ ['Sunrise' starting point](https://trinket.io/html/web-sunrise)

Die Kinder können auch von diesem leeren Trinket [(jumpto.cc/html-blank)](http://jumpto.cc/html-blank) Gebrauch machen, um ihren eigenen HTML und CSS Code zu schreiben, bzw. alternativ können sie dieses Vorlage-Trinket [(jumpto.cc/html-template)](http://jumpto.cc/html-template) benutzen.

Es gibt auch ein Trinket, dass eine Lösungsvorlage für die Aufgaben enthält:

+ ['Sunrise' Finished](https://trinket.io/html/abcc0284a3)

#Offline Ressourcen
Dieses Projekt kann [offline fertig gestellt werden](../offline.html), falls bevorzugt. Zugang zu den Projektressourcen ist durch Klicken auf den 'Download Project Materials' (Projektmaterialien herunterladen) Link für dieses Projekt möglich. Dieser Link enthält ein 'Project Resources' (Projektressourcen) Verzeichnis, das Ressourcen enthält, welche die Kinder benötigen, um dieses Projekt offline fertig stellen zu können. Achten Sie darauf, dass jedes Kind Zugang zu einer Kopie dieser Ressourcen hat. Dieses Verzeichnis enthält die folgenden Dateien:

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

Sie können eine fertig gestellte Version dieses Projekts im Abschnitt „Helfer Ressourcen“ finden, welcher u.a. Folgendes enthält:

+ sunrise-finished/index.html
+ sunrise-finished/style.css
+ sunrise-finished/prefixfree.js
+ sunrise-finished/boat.png
+ sunrise-finished/sun.png
+ sunrise-finished/rainbow.png

#Lernziele
+ Grafische Gestaltung und Animation mit CSS:
	+ Einführung der `@keyframes` (Schlüsselbilder) Regel zur Definierung von einzelnen Schritten in einer Animation.
	+ Bekräfitigung der Nutzung von Eigenschaften, um die Größe, Form, Position und Farbe von Elementen auf einer Webseite zu definieren.

Dieses Projekt deckt Elemente aus den folgenden Bereichen des [Raspberry Pi Lehrplans zur digitalen Produktion](http://rpf.io/curriculum):

+ [Design Grundlagen: 2D und 3D Assets](https://www.raspberrypi.org/curriculum/design/creator).

#Aufgaben
+ „Diagonale Animation“: Eine Animation mit Hilfe von `@keyframe` (Schlüsselbild) Eigenschaften bearbeiten, um „links“ zu benutzen:;
+ „Verbessere den Himmel“: Füge weitere Keyframes und Einstellungshintergründe hinzu:.
+ „Noch mehr Animationen“: Animiere noch mehr Bilder oder Elemente mit Hilfe von einer Vielzahl an CSS-Eigenschaften. 

#Häufig gestellte Fragen (FAQ)

+ Dieses Projekt nutzt die JavaScript `prefixfree.js` (Präfix-frei) Bibliothek, um die Kompatibilität der Animation zwischen den Browsern zu ermöglichen. Falls diese Bibliothek nicht benutzt wird, dann werden die Kinder, die ältere Browser benutzen statt dessen eine Animation für ihren Browser angeben müssen, zum Beispiel:

```
Animation: Himmel 10s unendlich; 		  	//für alle neueren Browser
-Webkit-Animation: Himmel 10s unendlich;  	// Für Webkit Browser(Chrome, Safari...)
-Moz-Animation: Himmel 10s unendlich;     	// Für Mozilla Browser
-O-Animation: Himmel 10s unendlich;       	// Für Opera Browser
-MS-Animation: Himmel 10s unendlich;		// Für Microsoft Browser 
```
