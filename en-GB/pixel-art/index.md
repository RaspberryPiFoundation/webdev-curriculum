---
title: Pixel Art
description: Create a pixel art editor. 
layout: project
notes: "Pixel Art - notes.md"
new: true
project-type: new
project-type: beta
---

# Introduction {.intro}

In this project, you'll create a pixel art editor. As well as using HTML and CSS you'll learn how to add JavaScript to your project.

![screenshot](images/pixel-art-final.png)

__How to use the editor__: Click on a colour from the palette to choose your pen colour then click on pixels to change their colour.

# Step 1: Creating a grid of pixels {.activity}

Let's create a grid of pixels that you can use for creating pixel art. CSS provides table styles for grid and table layouts. 

Tables contain rows which contain cells. You are going to create a table with a black background and then put white pixels into it. 

## Activity Checklist { .check}

+ Open this trinket: <a href="http://jumpto.cc/web-pixel" target="_blank">jumpto.cc/web-pixel</a>. If you're reading this online then  you can also use the embedded trinket below. 

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/705f264f59" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ 

 	Add the following html into the `<body>` of your `index.html` file to create a `<div>` as a container for your pixel art and give it an `art` id so you can style it:

 	![screenshot](images/pixel-art-art.png)

 	Now go to your `style.css` file and add the table styling for the art `<div>`:

	![screenshot](images/pixel-art-style.png)

	This creates a table with a border and sets the spacing inside the grid. 

	It doesn't look very interesting yet, you need to put rows of pixels inside it. 

 + Now go back to your `index.html` file and add a row of 3 pixels inside the art `<div>`:

 	![screenshot](images/pixel-art-row.png)

 	This time you're using classes to style the `<div>`s as there will be lots of them. 

 	Then add the following style for the rows and cells:

	![screenshot](images/pixel-art-row-style.png)

 	Now your pixels will line up in a grid with black lines around them. 

 + Now add another two rows of pixels to create a 3 x 3 grid. 

	![screenshot](images/pixel-art-grid-3.png)
	
    
##Challenge: Resize your grid {.challenge}

3x3 is quite a small grid for pixel art. Can you make the grid bigger? 8x8 is a good size for pixel art. 

Try using cut and paste rather than typing everything out. 

![screenshot](images/pixel-art-grid-8.png)

## Save Your Project {.save}

# Step 2: Colour the pixels {.activity}

You could use HTML and CSS to set the background colour of individual pixels, but that would be a slow way to work! Instead you're going to add some JavaScript code to colour pixels automatically. 

+ In JavaScript, code is placed in `function`s that can be called when we want to run that code. 

	You're going to create a function called `setPixelColour`

	The `setPixelColour` function needs to know which pixel to change the colour of, this is an `input`.

	Add the following code to the `script.js` file to set the background colour of a pixel:

	![screenshot](images/pixel-art-set-pixel-colour.png)

+ Now we need to call that function when a pixel is clicked on.

	HTML uses `onclick` to call a function when an element is clicked on. You'll need to pass in 'this' as the input so your function knows which pixel to change the colour of. 

	Go to `index.html` and add the following code to the first pixel:

	![screenshot](images/pixel-art-onclick.png)

+ Test your code by clicking in the first pixel. It should turn black:

	![screenshot](images/pixel-art-black.png)

	You only added `onclick` code to the first pixel so this won't work for the other pixels yet. 


##Challenge: Make all the pixels clickable {.challenge}

Can you make all the pixels clickable? Use cut and paste to make it quicker. 

Create a quick piece of pixel art. 

![screenshot](images/pixel-art-black-example.png)

# Step 3: Add a colour palette {.activity}

Did you find it annoying that you couldn't change a pixel colour back to white if you made a mistake? Let's fix that by creating a colour palette so that you can click on a colour to change the pen. 

+ First create a pen style. 

	Add the following code at the bottom of your `style.css` file:

	![screenshot](images/pixel-art-pen.png)

+ Now create black and white pen colours that use that style. 

	Add the following code to your `index.html` after the `<body>`:

	![screenshot](images/pixel-art-palette.png)

+ You want to be able to change the pen colour when a pen colour is clicked on. 

	Variables are used to store information. Let's create a penColour variable in `script.js`.

	Add the following code at the top of the file:

	![screenshot](images/pixel-art-pencolour.png)

	Then add a function to change the penColour:

	![screenshot](images/pixel-art-set-pen.png)

+ You'll also need use the pen colour when you change the colour of a pixel. 

	Change the `setPixelColour` function to use the `penColour` variable instead of `black`:

	 ![screenshot](images/pixel-art-use-pen.png)

+ Now you need to call the `setPenColour` function when a pen colour gets clicked. 

	Add the highlighted `onclick` code to your pen colours:

	![screenshot](images/pixel-art-palette-onclick.png)

+ Now test that you can switch the pen colour between black and white to fill in or delete pixels.


## Save Your Project {.save}

##Challenge: Add more colours to the palette {.challenge}

Can you add more colours to the palette? Choose the colours that you want to create pixel art with. 

The create some cool pixel art.

Hint: The bright green colour is called `chartreuse`.

![screenshot](images/pixel-art-final.png)

Ask a volunteer if you can use the Windows Snipping Tool or an alternative to create copies of your pixel art. 

## Save Your Project {.save}

