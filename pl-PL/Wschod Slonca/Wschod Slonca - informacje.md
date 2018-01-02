---
title: Wschód słońca — informacje
language: pl-PL
embeds: "*.png"
materials: [""]
...

#Wprowadzenie
Wykonując ten projekt dzieci nauczą się jak wykonywać proste animacje przy użyciu CSS. Będą używać reguły `@keyframes` do animowania różnych właściwości obrazków i elementów div.

#Źródła online
Do pisania kodu HTML i CSS online rekomendujemy użytkowanie edytora (https://trinket.io/).  
Do tego projektu udostępniony jest początkowy szablon:

+ ['Wschód słońca' - początek](https://trinket.io/html/web-sunrise)

Dostępny jest także projekt zawierający przykładowe rozwiązania wyzwań:

+ ['Wschód słońca' - skończony](https://trinket.io/html/abcc0284a3)

#Źródła offline
Projekt można również ukończyć offline. Materiały do projektu można pobrać, klikając w link "Pobierz materiały" na stronie z listą projektów. Pobrany plik zawiera katalog "Project Resources", w którym znajdują się zasoby potrzebne do wykonania tego projektu w trybie offline. Upewnij się, że każde dziecko ma dostęp do tych materiałów. Katalog zawiera następujące pliki:

+ template/index.html
+ template/style.css
+ sunrise/index.html
+ sunrise/style.css
+ sunrise/prefixfree.js
+ sunrise/boat.png
+ sunrise/cloud.png
+ sunrise/helicopter.png
+ sunrise/rainbow.png
+ sunrise/sun.png

Ukończona wersja zadań z tego projektu znajduje się w sekcji "Club Leader Resources", która zawiera:

+ sunrise-finished/index.html
+ sunrise-finished/style.css
+ sunrise-finished/prefixfree.js
+ sunrise-finished/boat.png
+ sunrise-finished/sun.png
+ sunrise-finished/rainbow.png

#Cele dydaktyczne
+ Stylowanie i animacja z użyciem CSS:
	+ Wprowadzenie reguły `@keyframes` do definiowania kroków animacji.
	+ Utrwalenie użycia właściwości do definiowania rozmiaru, kształtu, pozycji i koloru elementów na stronie internetowej.

#Wyzwania
+ "Animacja ukośna" - edycja reguły `@keyframes` poprzez użycie właściwości `left`.
+ "Ulepsz niebo" - dodanie klatek i ustawianie koloru tła.
+ "Jeszcze więcej animacji" - animowanie kolejnych obrazków i elemntów przy użyciu różnych właściwości CSS.


#Najczęściej zadawane pytania (FAQ)

+ Ten projekt używa biblioteki javascript `prefixfree.js`, aby użyta animacja była kompatybilna na różnych przeglądarkach. Bez użycia tej biblioteki, dzieci używające starszych wersji przeglądarek będą musiały zamiast tego deklarować animację w sposób dostosowany do ich przeglądarek, na przykład:

```
animation: sky 10s infinite; 		  	//dla wszystkich nowszych przeglądarek
-webkit-animation: sky 10s infinite;  	// przeglądarki z silnikiem Webkit (Chrome, Safari...)
-moz-animation: sky 10s infinite;     	// przeglądarki Mozilla
-o-animation: sky 10s infinite;       	// przeglądarki Opera
-ms-animation: sky 10s infinite;		// przeglądarki Microsoft
```
