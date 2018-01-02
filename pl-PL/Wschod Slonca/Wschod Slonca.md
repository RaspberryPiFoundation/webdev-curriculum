---
title: Wschód słońca
level: HTML & CSS 2
language: pl-PL
embeds: "*.png"
materials: ["Club Leader Resources/sunrise-finished/*.*", "Project Resources/sunrise/*.*", "Project Resources/template/*.*"]
stylesheet: web
...

# Wstęp {.intro}

Wykonując ten projekt nauczysz się, jak za pomocą CSS stworzyć animację ze wschodem słońca.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/abcc0284a3?outputOnly=true&start=result" width="600" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="sunrise-final.png">
</div>

# Krok 1: Słońce {.activity}

Zacznijmy od dodania obrazka ze słońcem i ustawieniu go w odpowiednim miejscu za pomocą CSS.

## Lista zadań {.check}

+ Otwórz edytor: <a href="http://jumpto.cc/web-sunrise" target="_blank">jumpto.cc/web-sunrise</a>. Jeśli pracujesz online, możesz również posłużyć się wersją wyświetloną poniżej.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/5085f92143" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ W środku znacznika `body` w pliku `index.html` znajdziesz dwa elementy `div`: niebo (ang. sky) i morze (ang. sea).

    ```
    <div id="sky">
    </div>

    <div id="sea">
    </div>
    ```

+ Obrazek ze słońcem jest już dodany do projektu.

    Wewnątrz elementu `div` z identyfikatorem `sun` dodaj kod, który wyświetli obrazek. Nadaj mu identyfikator, aby go za chwilę ostylować:

    ![screenshot](sunrise-sun-image.png)

+ Ho, ho, obrazek słońca jest ogromny. Przejdź do pliku `style.css` i dodaj kod CSS, aby ustawić jego wysokość:

    ![screenshot](sunrise-sun-height.png)

    Zauważ, że szerokość dopasuje się automatycznie w taki sposób, aby proporcje obrazka zostały zachowane.

+ Na koniec dodamy jeszcze trochę kodu, aby ustawić słońce w odpowiednim miejscu:

    ![screenshot](sunrise-sun-position.png)


## Zapisz swój projekt {.save}

# Krok 2: Animowany wschód słońca {.activity}

Aby stworzyć animację ze wschodem słońca, musisz zdefiniować, w jaki sposób słońce ma się poruszać i jak długo ma wschodzić.

Aby to zrobić zdefiniuj listę __klatek__. Każda klatka definiuje właściwości CSS danego elementu w konkretnym momencie animacji.

## Lista zadań {.check}

+ Najpierw musisz użyć `@keyframes`, aby zdefiniować nową animację, którą nazwiemy "sunrise" (z angielskiego: wschód słońca).

    Dodaj ten kod CSS na końcu pliku `style.css`:

    ```
    @keyframes sunrise {
        0% {top: 90%;}
        100% {top: 0;}
    }
    ```

    Ten kod mówi słońcu, w którym miejscu ma się znajdować na początku (`0%`) i na końcu (`100%`) animacji.

    Ponieważ słońce jest wewnątrz elementu `div` z niebem, dlatego pozycje `top` i  `left`, które wpisaliśmy odwołują się do tego elementu `div`. To znaczy, że `top: 100%` znajduje się na samym dole nieba, a nie na dole całej strony.


+ Teraz, kiedy masz już gotową animację `sunrise`, musisz tylko powiedzieć słońcu, aby jej użyło!

    Dodaj podświetlony kod, do kodu CSS słońca:

    ![screenshot](sunrise-sunrise.png)

    Dzięki temu słońce będzie wschodzić przez 10 sekund.

+ Aby uruchomić animację ponownie w edytorze kliknij **Autorun**.

## Zapisz swój projekt {.save}

## Wyzwanie: Animacja ukośna {.challenge}
Czy potrafisz do swojej animacji `sunrise` dodać kod, dzięki któremu słońce zacznie wschód na dole po lewej stronie i będzie przesuwać się skośnie w prawo w taki sposób, aby skończyć u góry pośrodku nieba?

Możesz użyć do tego właściwości `left`, na przykład:

```
left: 40%;
```

![screenshot](sunrise-left.png)

## Zapisz swój projekt {.save}


# Krok 3: Nieskończona animacja {.activity}

Sprawmy teraz, że animacja będzie się powtarzać w kółko.

## Lista zadań {.check}

+ Jeśli chcesz, aby słońce wschodziło i zachodziło, dodaj kilka klatek do swojej animacji:

    ```
    @keyframes sunrise {
        0%   {top:90%; left:0;}
        33%  {top:0; left:40%; }
        66%  {top:0; left:40%; }
        100% {top:90%; left:80%; }
    }
    ```

    To znaczy, że na początku i na końcu animacji słońce będzie na dole nieba, a na górze pozostaje od 33% do 66% animacji.

+ Teraz musisz tylko dodać słowo `infinite` (ang. bez końca) do animacji słońca, aby powtarzała się ona w kółko:

    ![screenshot](sunrise-infinite.png)

+ Przetestuj swoją animację. Czy słońce ciągle wschodzi i zachodzi?


## Zapis swój projekt {.save}

# Krok 4: Animowanie nieba {.activity}

Animacja służy tylko do poruszania elementami. Sprawimy teraz, by niebo pociemniało w nocy.

## Lista zadań {.check}

+ Dodaj animację o nazwie `sky` do swojego kodu CSS:

    ```
    @keyframes sky {
        0% {background: black}
        100% {background: lightblue}
    }
    ```

    Zauważ, że tym razem podczas animacji zmieniamy kolor nieba, a nie jego pozycję.

+ Dodaj poniższy kod do nieba, aby zaczęło używać nowej animacji:

    ```
    animation: sky 10s;
    ```

    ![screenshot](sunrise-sky.png)

+ Kliknij **Autorun**, aby przetestować animację.

## Zapisz swój projekt {.save}

## Wyzwanie: Ulepsz niebo {.challenge}

Czy potrafisz zmienić animację nieba w taki sposób, aby pasowało do słońca i pozostawało niebieskie w czasie dnia, a zmieniało się w czarne, kiedy słońce zachodzi? Zmień też kod tak, aby zmieniało się bez końca.

![screenshot](sunrise-sky-challenge.png)

## Wyzwanie: Jeszcze więcej animacji {.challenge}

Czy potrafisz dodać animację do jeszcze innego obrazka? Podczas animacji możesz zmieniać pozycję, kolor, kształt, rozmiar, przezroczystość albo cokolwiek sobie wymyślisz. Spróbuj też zmienić czas trwania animacji.

Do każdego elementu, który będziesz animować, musisz:

+ Dodać w kodzie HTML identyfikator (atrybut `id`)
+ Dodać styl CSS dla elementu z tym identyfikatorem
+ Stworzyć dafinicje klatek przy użyciu `@keyframes`
+ Użyć właściwości `animation:` w stylach tego elementu, aby użyć animacji zdefiniowanej przy użyciu `@keyframes`

Kliknij na ikonkę z obrazkiem, aby zobaczyć, jakie obrazki zostały dołączone do projektu:

![screenshot](sunrise-images.png)

Możesz dodać też swoje obrazki, jeśli chcesz.

Nie zapomnij umieścić tych elementów na morzu lub na niebie:

![screenshot](sunrise-boat.png)

Przykładowo tęcza używa właściwości `opacity` (ang. nieprzezroczystość), aby uzyskać efekt pojawiania się i zanikania:

```
@keyframes fade {
  0%   {opacity: 0;}
  50%  {opacity: 100;}
  66%  {opacity: 0;}
  100%   {opacity: 0;}
}
```

Łódź używa ujemnej pozycji początkowej, aby nie było jej widać na początku animacji:

```
 @keyframes left-right {
  0%    {left:-50%;}
  100%  {left:200%;}
}
```

## Zapisz swój projekt {.save}
