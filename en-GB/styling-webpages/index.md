---
title: Styling web pages
level: HTML&CSS 1
language: en-GB
embeds: "*.png"
materials: "code and images"
stylesheet: web
...

## Introduction { .intro}

Let’s make our website look nicer with some styles. In this lesson and the next we are going to learn how to change colour, text, sizes and more!

We style HTML pages using a language called __CSS__ (which stands for __Cascading Style Sheets__). It is a very simple language to learn. Let’s get started.

#Step 1: Setting up to write some style { .activity}

There are many ways to add styles to your HTML: inline, in the head, or as a separate .css document that we link to from the head. But today, we’ll be using styles in the `head` element of our html page so we don’t have to worry about handling multiple files.

## Activity checklist { .check}

+ Open the index.html from the Felix folder we did last session.
+ In the head section, we need a __style tag__.
```html
<style>
</style>
```
All our styles will go between these two elements. Simplez. In general, css code looks like this:

```css
selector {
	property: value;
}
```

+ Can you find the ‘{‘ and ‘}’ keys on your keyboard?
+ How about ‘:’ and ‘;’?

Selectors can be html elements like `h1`, `p`, `img`, `a`. But they can also be other things which we will learn later.

# Step 2: Adding Colours { .activity}

Let’s add some colour with the color property! It’s color without the u. Yes we think it’s confusing too. It’s because it's using the American spelling of the word, despite the fact that CSS was invented by a Norwegian person. You'll get used to it soon enough, just don't forget the English spelling in your English lessons!

Let’s change the `h1` to be red instead of black.

```css
h1 {
	color: red;
}
```

## __SAVE__ your file and __VIEW__ it in your browser { .save}

The text is now red, w00t! There are different ways of saying the values for the color. There are 16 basic color names, they are aqua, black, blue, fuchsia, gray, green, lime, maroon, navy, olive, purple, red, silver, teal, white, and yellow.

+ Try changing the color to something else!
Most browsers support an additional 130 color names, a full alphabetical list of which is found at [http://www.w3.org/TR/css3-color/#svg-color](http://www.w3.org/TR/css3-color/#svg-color) - is your favourite colour in the list?

+ But we can use even more colors by using __hexidecimal code__ instead of color name. A hexcode is a # followed by 6 digits, the digits can be 0-9 or the letters A, B, C, D, E, F. Using hexcode we can use more than 16 million colours!
+ At Code Club, our favourite colour is `#58AB57`. Can you guess what colour it is? Why don’t you try changing some text to that colour and view it in a browser to see.

## __SAVE__ your file and __VIEW__ it in your browser { .save}

#Step 3: Colouring specific elements { .activity}

What if we wanted to make the word ‘orange’ in ‘his fur is orange’ orange? Not the whole paragraph, just that word.

One way of doing that is putting `<span>` tags around the word, like so:

`<span>orange</span>`

Then in the head, we can style the span.

```css
span {
	color: orange;
}
```

## __SAVE__ your file and __VIEW__ it in your browser { .save}

#Step 4: Background { .activity}

We can add colours to the background too, not just text. For instance:

```css
body {
	background-color: #D2FAFC;
}
```

This will make the entire background light blue. You can choose any colour you like from a list at [www.colourpicker.com](http://www.colourpicker.com) which generates the number you need which you can copy and paste into your code.

Now try:

```css
h1 {
	background-color: black;
}
```

Since we already had a `h1` declaration in there, we could just put in the background-color with the color, no need to write it all out again.

```css
h1 {
	background-color: black;
	color: red;
}
```


## Now __SAVE__ your file and see what it looks like. { .save}


## Fun with text

Maybe the ‘Missing’ header should be __bigger__ and also all capital letters. We can specify the size of the text using `font-size`. The values can be many things, but the most common are 12, 14, 16, 32, 48 and 72 pixels. For now lets try 72px. (px means pixel).

```css
h1 {
    background-color: black;
    color: red;
    font-size: 72px;
}
```

Now try making the heading capital letters only by using `text-transform:uppercase;` We can also make it underlined by using `text-decoration:underline;`

## Now __SAVE__ your file and see what it looks like. { .save}

It’s much more noticeable now right?

# Step 6. Centering text (and images) horizontally { .activity}

All our text is all the way over on the left. We can change that using `text-align:center` (it also takes ‘right’, ‘left’ is the default).

+ We want all our text to be centered for this particular webpage, so we can write: Note the American spelling of the word centre is center.

```css
body {
    background-color: #F8FAF4;
    text-align: center;
}
```
Did you notice that everything in the page went to the centre when we put ‘text-align: center’ in the body section? That’s because everything inside the body element inherits the style. This happens whenever one element is inside another, like here:

```html
<p>Have you seen Felix? <em>Please</em> contact his owner</p>
```

The ‘Please’ will have the style of the `<p>` element with the style of the `<em>` element added on. This is why the stylesheets are called __cascading__ - the styles cascade from elements into all the ones inside them. Be careful, though, because some styles are not *inherited*. We will find out about these later.

## Now __SAVE__ your file and view it in a browser { .save}

##Further study { .try}

+ How would you change the page to make it look better? Why not try using all your favourite colours? Do they have colour names or do you need to use hexcode?
+ If you finish early you can go back and add styles to the html we made in previous lessons.
