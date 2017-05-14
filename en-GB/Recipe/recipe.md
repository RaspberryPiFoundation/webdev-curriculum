---
title: Recipe
level: HTML & CSS 1
language: en-GB
embeds: "*.png"
materials: ["Club Leader Resources/recipe-finished/*.*", "Project Resources/template/*.*"]
stylesheet: web
...

# Introduction { .intro}

In this project, you’ll learn how to create a webpage for your favourite recipe.

![screenshot](recipe-final.png)

# Step 1: Decide on a recipe { .activity}

Before you get coding, you’ll need to decide on a recipe.

## Activity Checklist { .check}

+ Think about a recipe you want to share with your friends. It could be:
	+ A recipe you found online;
	+ Your favourite meal;
	+ Something you made up!

The example recipe you’ll see in this project is for a banana milkshake. You can copy this recipe if you can’t find one of your own.

# Step 2: Ingredients { .activity}

Let’s list the ingredients that are needed for your recipe.

## Activity Checklist { .check}

+ Open this template trinket: [jumpto.cc/trinket-template](http://jumpto.cc/trinket-template). If you’re reading this online, you can also use the embedded version of this trinket below.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ef4c882ae6" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ For your list of ingredients, you’re going to use an __unordered list__, using the `<ul>` tag. Go to line 8 of the template and add this HTML, replacing the text in the `<h1>` title with the name of your own recipe:

```
<h1>Banana Milkshake</h1>

<h3>Ingredients:</h3>

<ul>

</ul>
```

+ View your webpage, and you should see your two headings.

![screenshot](recipe-headings.png)

You won’t see your list yet though, because you haven’t added any list items to it!

+ The next step is to add list items into your list, by using the `<li>` tag. Add the following code inside your `<ul>` tag:

```
<li>1 banana</li>
```
![screenshot](recipe-ul.png)

As your list is unordered, there are no numbers next to the list items, just bullet points.

##Challenge: More ingredients {.challenge}
Can you add all of the ingredients for __your__ recipe?

Your webpage should look something like this:

![screenshot](recipe-more-ingredients.png)

## Save Your Project {.save}

# Step 3: Method { .activity }

Next, let’s explain how to make your recipe.

## Activity Checklist { .check}

+ You’re going to use another list to write your method, but this time you’ll be using an __ordered list__, by using the `<ol>` tag.

An ordered list is a numbered list, which you should use when the order of the steps is important.

Add this code underneath your ingredients list, making sure that it’s still inside your `<body>` tag:

```
<h3>Method:</h3>

<ol>

</ol>
```

![screenshot](recipe-method.png)

+ Now you just need to add list items into your new ordered list:

```
<li>Peel the banana and add to a blender</li>
```

![screenshot](recipe-ol.png)

Notice that the list items are automatically numbered!

##Challenge: More steps {.challenge}
Can you add all of the steps for making __your__ recipe?

Your method should look something like this:

![screenshot](recipe-more-method.png)

## Save Your Project {.save}

# Step 4: Colours! { .activity}

Let’s add some colour to your recipe webpage.

## Activity Checklist { .check}

+ You’ve already learnt how to add coloured text to a webpage. Add this code inside your `style.css` file, to make all of the text in the website body blue:

```
body {
    color: blue;
}
```

![screenshot](recipe-blue.png)

+ Your browser knows colours like `blue`, `yellow` and even `lightgreen`, but did you know that your browser actually knows the __names__ of over 140 different colours?

There’s a list of all the colour names you can use: [jumpto.cc/web-colours](http://jumpto.cc/web-colours), which includes colour names like `tomato`, `firebrick` and `peachpuff`.

Change the text colour from `blue` to `tomato`.

![screenshot](recipe-tomato.png)

+ Your browser knows the names of 140 colours, but actually knows the __colour values__ of more than 16 million colours!


As you may know, all colours can be made from the primary colours: red, green and blue. To tell the browser which colour to display, you just need to let it know how much of each primary colour to use.

The amounts of red, green and blue to use are written as a number between `0` and `255`.

![screenshot](recipe-rgb-img.png)

Add this code to the CSS for the body of the webpage, to display a light yellow background:

```
background: rgb(250,250,210);
```

![screenshot](recipe-rgb.png)

+ If you prefer, you can tell the browser which colour to display by using a hexadecimal code (or __hex code__). This works in a similar way to the `rgb()` code above, except that hex codes always start with a `#`, and use hexadecimal ‘numbers’ between `00` and `ff` for the amount of red, green and blue.

![screenshot](recipe-hex-img.png)

Replace the `rgb()` code in your CSS with this hex code:

```
background: #fafad2;
```

![screenshot](recipe-hex.png)

You should see the same light yellow as before!

## Save Your Project {.save}

# Step 5: Finishing touches { .activity}

Let’s add a little more HTML and CSS to improve your webpage.

## Activity Checklist { .check}

+ You can add a horizontal line at the end of your recipe, by using the `<hr>` tag.

![screenshot](recipe-hr.png)

Notice that this tag doesn’t have an end tag, just like the `<img>` tag.

+ The line you’ve just added doesn’t match the style of the rest of your webpage. Let’s fix that by adding some CSS code:

```
hr {
    height: 2px;
    border: none;
    background-color: tomato;
}
```

![screenshot](recipe-hr-css.png)

+ You can even change how your bullet points look with this CSS code:

```
ul {
    list-style-type: square;
}
```

![screenshot](recipe-ul-css.png)

##Challenge: More colours! {.challenge}
Change the colours in your code by using colour names, `rgb()` values and hex codes. There’s a list of loads of colours at <a href="http://jumpto.cc/web-colours" target="_blank">jumpto.cc/web-colours</a>.

Here are some example colours:

+ Red can be written as:
	+ `red` (obviously!)
	+ `rgb(255,0,0)` (loads of red, no green and no blue)
	+ `#ff0000`

+ Olive can be written as:
	+ `olive`
	+ `rgb(128, 128, 0)` (a bit of red and green, and no blue)
	+ `#808000`

Try to make sure that the colours you use match your recipe!

## Save Your Project {.save}

##Challenge: Reviews {.challenge}
Ask a few of your friends to leave a review for your recipe. You’ll need to make another list to do this.

![screenshot](recipe-reviews.png)

## Save Your Project {.save}

##Challenge: More styling {.challenge}
Can you add an image into your webpage? Or change the font? Here’s how your webpage could look:

![screenshot](recipe-final.png)

Here’s some code that will help you:

```
font-family: Arial / Comic Sans MS / Courier / Impact / Tahoma;
font-size: 12pt;
font-weight: bold;

<img src="image-link-goes-here">
```

## Save Your Project {.save}
