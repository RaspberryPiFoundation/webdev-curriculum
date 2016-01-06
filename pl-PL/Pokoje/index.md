---
title: Pokoje
level: HTML & CSS 1
language: pl-PL
embeds: "*.png"
materials: ["volunteer-resources/*.*","project-resources/*.*"]
stylesheet: web
...

# Wstęp {.intro}

Wykonując ten projekt zbudujemy kilka połączonych pokojów - każdy pokój będzie osobną stroną internetową.

![screenshot](rooms-hall-finished.png)

# Krok 1: Linkowanie do innej strony w tym samym projekcie {.activity}

Strony intenetowe mogą być stworzone z wielu plików HTML połączonych ze sobą linkami.

## Lista zadań {.check}

+ Otwórz ten projekt: <a href="https://trinket.io/html/8fd770bec4">https://trinket.io/html/8fd770bec4</a>. Jeśli pracujesz online, możesz również posłużyć się wersją wyświetloną poniżej.

    <div class="trinket">
      <iframe src="https://trinket.io/embed/html/8fd770bec4" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
      </iframe>
    </div>

+ Uruchom projekt - powinieneś znaleźć się na korytarzu:

    ![screenshot](rooms-hall-start.png)

+ Spójrz na zakładki z nazwami plików w tym projekcie. Czy widzisz `salon.html`?

    ![screenshot](rooms-tvroom-html.png)

    To jest po prostu inny plik HTML w tym samym projekcie.

    Ten plik korzysta ze swoich stylów, które znajdują się w pliku `salon.css`.

+ Aby wyświetlić `salon.html` musisz dodać link w `index.html`:

    ![screenshot](rooms-link-tvroom.png)

    Przetestuj swój projekt klikając na link __Salon__, by zobaczyć stronę `salon.html`:

    ![screenshot](rooms-tvroom-unstyled.png)

## Wyzwanie: Dodaj kolejny link {.challenge}

Dodaj w link w pliku `salon.html`, który zabierze cię z powrotem na stronę korytarza (`index.html`).

Salon powinien mieć link, który możesz kliknąć:

![screenshot](rooms-hall-link.png)

## Zapisz swój projekt {.save}

# Krok 2: Dodaj inny pokój {.activity}

Dodajmy teraz inny pokój - __Pokój Zabaw__.

## Lista zadań {.check}

+ Kliknij na przycisk __+__, który służy do dodawania stron:

    ![screenshot](rooms-add-page.png)

    Jako nazwę strony wpisz `pokojzabaw.html`:

    ![screenshot](rooms-games-html.png)

+ Kod HTML dla __Pokoju Zabaw__ jest bardzo podobny do tego z pliku `salon.html`, więc możesz skopiować go i wkleić do pliku `pokojzabaw.html`.

    Zmień podświetlone elementy zamieniając "Salon" na "Pokój Zabaw", a `salon.css` na `pokojzabaw.css`:

    ![screenshot](rooms-games-html2.png)

+ Twój plik `pokojzabaw.html` używa teraz `pokojzabaw.css`.

    Stwórz plik `pokojzabaw.css` klikając na przycisk dodawania nowej strony __+__.

    ![screenshot](rooms-add-games-css.png)

+ Kod CSS dla __pokoju zabaw__ jest bardzo podobny do tego z pliku `salon.css`, więc skopiuj go i wklej do pliku `pokojzabaw.css`.

+ Dodaj link tak, by z korytarza można było przejść do pokoju zabaw:

    ![screenshot](rooms-hall-games.png)

+ Przetestuj swój projekt klikajć na link do pokoju zabaw.

    __Pokój Zabaw__ powinien wyglądać mniej więcej tak:

    ![screenshot](rooms-games-before.png)

    Niezbyt ekscytująco, ale możesz zmienić to podejmując poniższe wyzwanie.

## Zapisz swój projekt {.save}

## Wyzwanie: Ostyluj i podlinkuj pokój zabaw {.challenge}

Zmień kod HTML i CSS pokoju zabaw w taki sposób, by strona wyglądała tak:

![screenshot](rooms-games-challenge.png)

Podpowiedź: Jasnozielony kolor nazywa się `chartreuse`.

## Zapisz swój projekt {.save}

# Krok 3: Linki, które wyglądają jak drzwi {.activity}

Linki nie muszą być zwykłym tekstem. Stwórzmy klikalne drzwi używając tagu `<div>`.

## Lista zadań {.check}

+ Otwórz `index.html` i dodaj tag `<div>` wokół tekstu __Salon__. Tag `<div>` powinien znaleźć się wewnątrz `<a>`, aby cały był klikalny.

    Dodaj do niego `class="drzwi"`, aby za chwilę dodać kod CSS, który sprawi, że będzie wyglądał jak drzwi.

    Dodaj też `id="korytarz-salon"`, aby ustawić go w odpowiednim miejscu.

    ![screenshot](rooms-tvroom-div.png)  

+ Teraz kliknij na zakładkę `style.css` i dodaj poniższy kod CSS, aby zmienić rozmiar i kolor drzwi:

    ![screenshot](rooms-door-css1.png)

+ Przetestuj swoją stronę klikając drzwi w różnych miejcach, nie tylko w tekst.

+ Zmieńmy je tak, by wyglądały trochę bardziej jak drzwi. W tym celu dodamy ramkę z trzech stron:

    ![screenshot](rooms-door-css2.png)

+ Dodajmy też trochę kodu CSS, aby tekst na drzwiach wyglądał nieco lepiej:

    ![screenshot](rooms-door-css3.png)

+ Pewnie zauważyłeś, że drzwi wiszą w powietrzu. Naprawmy to ustawiając je w odpowiednim miejscu. Użyjemy do tego ich identyfikatora (id).

    ![screenshot](rooms-door-position.png)

+ Przetestuj stronę klikając w drzwi do __Salonu__.

## Zapisz swój projekt {.save}

## Wyzwanie: Jeszcze więcej drzwi! {.challenge}

Zamień pozostałe linki w projekcie w taki sam sposób - zrób z nich drzwi.

Każdy pokój ma swój własny plik CSS, więc nie zapomnij dodać styl drzwi do każdego z nich.

Salon powinien wyglądać mniej więcej tak:

![screenshot](rooms-tvroom-door.png)

# Krok 4: Dodajemy tło {.activity}

Udekorujemy teraz korytarz dodając obrazek tła.

## Lista zadań {.check}

+ W pliku `style.css` dodaj obrazek tła do korytarza:

    ![screenshot](rooms-hall-decorated.png)

    Obrazek będzie powtarzany, aby wypełnić cały pokój.

+ Przetestuj projekt.

## Zapisz swój projekt {.save}

## Wyzwanie: Dodaj tapetę do pokoju zabaw {.challenge}

Czy potrafisz udekorować pokój zabaw dodając obrazek jako tło?

Możesz użyć tapety z pliku `space-invader.png`.

Udekorowany pokój powinien wyglądać mniej więcej tak:

![screenshot](rooms-games-finished.png)

## Zapisz swój projekt {.save}

# Krok 5: Klucz jako wzkaźnik myszy {.activity}

## Lista zadań {.check}

+ Kolejnym fajnym elementem, który zrobimy będzie dodanie obrazka jako wskaźnika myszy (kursora). Otwórz `style.css` i dodaj wybrany kursor do klasy `.drzwi`, aby wskaźnik myszy zamieniał się w klucz, kiedy najedziesz myszką na drzwi.

    ![screenshot](rooms-key-cursor.png)

    Obrazek `key.png` jest już wbudowany w twój projekt.

    Kod CSS `, auto` oznacza, że jeśli nie będzie można wyświetlić wybranego obrazka, zamiast niego zostanie użyty zwykły kursor.

+ Dodaj kursor-klucz do plików `salon.css` i `pokojzabaw.css`.

+ Przetestuj projekt. Wskaźnik myszy powinien zamienić się w klucz zawsze, kiedy najedziesz myszką na drzwi. Sprawdź to w każdym pokoju.

## Zapisz swój projekt {.save}

## Wyzwanie: Zrób po swojemu! {.challenge}

Dodaj swoje pokoje do projektu.

Do dekoracji możesz użyć też obraka `tiles.png`.

## Zapisz swój projekt {.save}
