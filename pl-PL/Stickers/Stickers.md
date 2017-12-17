---
title: Naklejki!
level: HTML & CSS 2
language: pl-PL
embeds: "*.png"
materials: ["Club Leader Resources/stickers-finished/*.*", "Project Resources/stickers/*.*", "Project Resources/template/*.*"]
stylesheet: web
...

# Wstęp {.intro}

W czasie tego projektu wykonasz wiele zabawnych naklejek, których możesz użyć do ozdobienia swoich stron internetowych. Nauczysz się, jak używać gradientu, żeby twoje naklejki fajnie wyglądały.

![screenshot](stickers-finished.png)

# Krok 1: Naklejka z liniowym gradientem {.activity}

Gradient to stopiowe przejście z jednego koloru w drugi. Gradienty mogą być używane, aby osiągnąć ciekawe efekty. Zaraz użyjesz ich do stworzenia naklejek, któych będzie można użyć na stronach internetowych.

+ Otwórz edytor: <a href="http://jumpto.cc/web-stickers" target="_blank">jumpto.cc/web-stickers</a>. Jeśli pracujesz online, możesz również posłużyć się wersją wyświetloną poniżej.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/af0ea6fa35" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ Zróbmy naklejkę 'I <3 Coding' (ang. "Uwieblbiam kodowanie")

  Użyj `<div>` z klasą `sticker` i identyfikatorem `coding`, aby później go ostylować:

	![screenshot](stickers-coding-error.png)


+ Hmm, zauważyłeś, że edytor pokazał błąd? A to dlatego, że "<" to w HTML-u znak specjalny. Zamiast "<" musisz użyć specjalnego kodu `&lt;`.

  Zmień swój kod i użyj `&lt;`, aby pozbyć się tego błędu.

	![screenshot](stickers-coding-fixed.png)

	`<br>` powoduje przejście do następnej linii.

+ Teraz zmieńmy naklejkę tak, aby była nieco ciekawsza.

  Przełącz się na plik `style.css`. Zauważ, że klasa `.sticker` jest już opisana w taki sposób, aby naklejka wyświetlała się na stronie i miała wyśrodkowaną zawartość.

  Pamiętaj, że do swojej naklejki dodałeś identyfikator `coding`. Na końcu pliku `style.css` dodaj poniższy kod, aby ostylować tekst:

	![screenshot](stickers-coding-font.png)

+ Teraz możesz dodać gradient jako tło naklejki. Liniowy gradient polega na zmianie koloru z jednego w drugi wzdłuż linii prostej.

  Taki gradient powoduje przejście z czerwonego na górze do purpurowego na dole. Dodaj poniższy kod do stylu `coding`:

	![screenshot](stickers-coding-gradient.png)

+ Możesz jeszcze ulepszyć efekt dodając odpowiednie odstępy i zaokrąglone narożniki.

	Dodaj podświetlony kod:

	![screenshot](stickers-coding-padding.png)

  Atrybut `padding` dodaje odstęp wielkości 50px na górze i dole oraz 30px z lewej i prawej strony.


## Zapisz swój projekt {.save}

# Step 2: Make a radial gradient sticker {.activity}

Gradients can also change colour from the centre out to the edges, this is called a radial gradient.

+ Let's create a sticker with the text `HTML & CSS.`  `&` is another character that needs encoding in HTML, the code is `&amp;`.

	Add the highlighted code to create a new sticker:

	![screenshot](stickers-web-html.png)

+ Now switch to your `style.css` file and add a style for your new sticker:

	![screenshot](stickers-web-font.png)

	The `text-shadow` code adds a shadow which extends 2px below and to the right of the text to make it stand out.

+ Now for the gradient. This time let's use a radial gradient. The colour will change from yellow in the centre through to orange and then red.

	![screenshot](stickers-web-gradient.png)

	Notice that gradients can include multiple colours, not just two.

+ The sticker will look much better with some padding and a rounded border.

	Add the highlighted code:

	![screenshot](stickers-web-padding.png)


## Save Your Project {.save}

##Challenge: Create your own gradient sticker {.challenge}

Now make your own gradient sticker. Try linear and radial gradients using multiple HTML colours.

You'll need to:

+ Add a `<div>` with your sticker text to `index.html` and give it the `sticker` class and a new `id`.
+ Add style for the `id` you chose in `style.css`. You could copy one of the sticker styles you have already made and edit that.

There’s a list of all the colour names you can use: [jumpto.cc/web-colours](http://jumpto.cc/web-colours), which includes colour names like `tomato`, `firebrick` and `peachpuff`.

If you want to change the text colour you can use `color:`.

Here's an example of what you can do with multiple colours in a linear gradient:

![screenshot](stickers-save-robots.png)

## Save Your Project {.save}

# Step 3: Make a gradient sticker with an image  {.activity}

You can also make a gradient sticker using an image. If you use an image with a transparent background then the gradient will show through.

+ First let's create an sticker that includes an image.

	Your project already includes an image called `purplerobot.png`.

	Add the highlighted code to `index.html`:

	![screenshot](stickers-purple-html.png)

	You can adjust the `height` to resize the image, the width will change automatically.

+ Now add the style code to create a gradient background for your image sticker:

	![screenshot](stickers-purple-css.png)


## Save Your Project {.save}

##Challenge: Make your own image sticker {.challenge}

Now make your own image sticker with a gradient.

You'll need to:

+ Add a new sticker `<div>` to `index.html` which includes an image.
+ Add the `sticker` class and a new id to your sticker div.
+ Create a style for your new id with a gradient and padding.

Your project already includes a set of robot images. Click on the images icon to see the available images.

![screenshot](stickers-images.png)

Here's an example image sticker with a linear gradient:

![screenshot](stickers-blue-robot.png)


## Save Your Project {.save}

# Step 4: Horizontal gradients  {.activity}

Gradients can be horizontal as well as vertical.

+ Let's create another image sticker.

	This time we'll use `greenrobot.png`. Add the following code to `index.html`:

	![screenshot](stickers-green-html.png)

+ Normally a linear gradient runs from top to bottom, but if we add `to right` then we can make it run from left to right.

	Add the highlighted code to `style.css` to add a horizontal gradient to your green robot sticker.

	![screenshot](stickers-green-style.png)

	Notice that the gradient runs from green on the left to yellow on the right.

+ This robot looks like he wants to say something. Let's also add some text to your sticker.

	Go to `index.html` and add the text 'Hello!' to your green robot sticker, put it inside a `<span>` with an id so that you'll be able to style it:  

	![screenshot](stickers-green-span.png)

+ The text will look better if you make it bigger and position it.

	To position the text you'll need to add `position: relative;` to `#greensticker` and `position: absolute` to `#greentext`. This is covered in more detail in the `Build a Robot` project.

	Add the highlighted code to `style.css`:

	![screenshot](stickers-green-text-style.png)

	Now the 'Hello!' text is positioned relative to the bottom right corner of the sticker.

## Save Your Project {.save}

# Step 5: Diagonal gradients  {.activity}

You can also create diagonal gradients that run from corner to corner.

+ Add a sticker to `index.html` using the `firerobot.png` image:

	![screenshot](stickers-fire-html.png)

+ With a diagonal gradient you give two directions. The example uses `to bottom left`.

	Add this style to `style.css` to give your new robot sticker a diagonal gradient and a fancy border:

	![screenshot](stickers-fire-gradient.png)

	Note that you can use `outline` to create another border outside the usual one.
	`outline-offset` gives the gap between the border and the outline.

+ Let's add some text to this sticker.

	Add a `<span>` containing the text "ROBOTS!" to `index.html` and give it an id.

	![screenshot](stickers-fire-span.png)

+ Now you can position the text by adding the following style:

	![screenshot](stickers-fire-text-style.png)

+ And for a final twist, let's rotate the text using `transform: rotate`.

	![screenshot](stickers-fire-rotate.png)

	Try changing the number of degrees that the text is rotated.


## Save Your Project {.save}

##Challenge: Make more stickers {.challenge}

Now try making more stickers using different gradient directions and adding images and text and using borders and outlines.

You can copy one of your examples and make changes to create a new sticker.

Here's an example using a diagonal gradient:

![screenshot](stickers-dog-robot.png)

## Save Your Project {.save}
