---
title: Styling and formatting text
level: HTML&CSS 1
language: en-GB
embeds: "*.png"
materials: "code and images"
stylesheet: web
...

## __Introduction:__ {.intro }
In this session we are going to learn how to style text with different fonts, colours and sizes. We'll also learn how to add background colours and borders. We will be using the same project you worked on last time, so make sure you open the index.html from the Felix folder.

#Step 1: Fonts {.activity}

We can change the look of the text by changing the __font__. The most common fonts are called

+ Arial
+ Courier New, Courier
+ Garamond
+ Georgia
+ Lucida Sans, Lucida Grande, Lucida
+ Palatino Linotype
+ Tahoma
+ Times New Roman, Times
+ Trebuchet
+ Verdana

Not all fonts exist on all computers, so we need to provide __fall-back fonts__ as well. These are very generic like ‘sans serif’, ‘serif’.

Let’s try changing the font of the headline using the `font-family` property.

```{.language-css}
h1 {
	color: red;
	background-color: black;
	font-family: impact, sans-serif;
	font-size: 72px;
	text-decoration: underline;
	text-transform: uppercase;
}
```
And the font of the paragraphs...

```{.language-css}
p {
	font-family: Georgia, 'Times New Roman', serif;
}
```

##__Save__ and __view__. {.save}

Try some of the different fonts to see which ones you like best. Notice how we separate each font with a comma, and if the font has a name with more than one word we need to put it inside quotation marks.

Which of the fonts we mentioned do you think looks best? Which one do you think is easiest to read?

Do you have other fonts on your computer than the ones mentioned? (you probably do). Try opening a program like Word or Pages, all the fonts stored on the computer can usually be found there.

![screenshot](fonts.png)

Find one you like and try it out on the website!

You can make text __bold__, *italic* or both with the font-style property. Let’s change the email text (remember it’s inside an `<a>` tag).

```{.language-css}
a {
	font-style: bold;
}
```

##__Save__ and __view__. {.save}

Or we could make it italic.

```{.language-css}
a {
	font-style: italic;
}
```
##__Save__ and __view__. {.save}

There’s also a font-style value called ‘oblique’. What does that look like?

We can even say how bold some text should be using the property `font-weight`. It takes the values `normal`, `bold`, `bolder`, `lighter`. You can also use numbers, 100, 200, 300, 400, 500, 600, 700, 800, and 900, where 100 is the thinnest text and 900 is the thickest (boldest text). Normal text is the same as 400, bold is the same as 700. However, not all the fonts have all these, so it’s safer to just use normal and bold. Headlines are normally bold by default. If we wanted our `h2` to not be bold, we need to write:

```{.language-css}
h2 {
	font-weight: normal;
}
```

Try it!

#Step 2: Borders! {.activity}

Let’s add a border around the image

```{.language-css}
img {
	border-color: green;
	border-style: solid;
	border-width: 5px;
}
```
##__Save__ and __view__. {.save}

Try changing the color, width and border-style until you are happy. Some values for border-syle are `dashed`, `dotted`, `double`, `groove`, `ridge`, `inset`, `outset`.

You can put borders around all kinds of elements, why not try a few more.

#Step 3: IDs and classes {.activity}

We want to make the contact paragraph __highlighted__.  We can’t use the `<p>` tag because that would change all the paragraphs. To make a style apply only to one element, we use something called IDs. We need to edit the html to this:

```{.language-markup}
<p id ="highlight">Have you seen Felix? <em>Please</em> contact his owners at <a href="mailto:felixowners@email.com">felixowners@email.com</a></p>
```

Then we can style the ID like so:

```{.language-css}
#highlight {
	color: red;
}
```

##__Save__ and __view__. {.save}

An ID is unique and can only be used once per page. So what if we wanted to make two of the paragraphs have a larger font-size? We can do that by using classes. First we need to give class names to the paragraphs we want changing.

```{.language-markup}
<p class="large">He went missing from the garden yesterday.</p>
<p class="large"><strong>Thank you!</strong></p>
```
we style a class like this (with a `.` instead of a `#`):

```{.language-css}
.large {
	font-size:24px;
}
```

##Further study: {.try}

+ How would you change the page to make it look better? Why not try using your favourite fonts and colours?
+ If you finish early you can go back and style the html like we did in previous lessons.
+ By the way, did you know that the background property does not only take values that are colours, but also images?
