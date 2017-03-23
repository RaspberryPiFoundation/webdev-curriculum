---
title: Sunrise
description: Create an animated sunrise. 
layout: project
notes: "Sunrise - notes.md"
...

# Introduction { .intro}

In this project, you'll learn how to use CSS to create an animated sunrise.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/abcc0284a3?outputOnly=true&start=result" width="600" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="images/sunrise-final.png">
</div>

# Step 1: Creating the sun { .activity}

Let's start by adding an image for the sun and positioning it with some CSS.

## Activity Checklist { .check}

+ Open this trinket: <a href="http://jumpto.cc/web-sunrise" target="_blank">jumpto.cc/web-sunrise</a>. 

    The project should look like this:

	![screenshot](images/sunrise-starter.png)

+ Look inside the `body` of your `index.html` file and you'll find the the `div` elements for the sky and the sea.

    ```
    <div id="sky">
    </div>
    
    <div id="sea">
    </div>
    ```

+ An image for the sun is already included in your project. 

    Add the image inside your sun `div` including an id so you can style it:

    ![screenshot](images/sunrise-sun-image.png)

+ Whoa, the image is huge. Go to `style.css` and add the CSS to set the image height:

    ![screenshot](images/sunrise-sun-height.png)

    Note that the width is updated automatically to keep the proportions the same. 

+ Finally, let's add some code to position the sun:

    ![screenshot](images/sunrise-sun-position.png)


## Save Your Project {.save}

# Step 2: Animating the sunrise { .activity}

To animate your sunrise, you need to define how the sun moves and how long it takes to rise.

To do this you define a list of __key frames__. Each key frame defines the CSS properties of an element at a particular point in an animation. 

## Activity Checklist { .check}

+ First, you need to use `@keyframes` to create a new animation called sunrise. 

    Add this CSS code to the end of your `style.css` file:

    ```
    @keyframes sunrise {
        0% {top: 90%;}
        100% {top: 0;}
    }
    ```

    This code tells the sun where to position itself at the start (`0%`) and the end (`100%`) of the animation.

    Because the sun is inside the sky `div`, the `top` and `left` positions you give are within to the sky, with `top: 100%` being the bottom of the sky, and not the bottom of the webpage.


+ Now that you have created a `sunrise` animation, you just need to tell your sun to use it! 

    Add the highlighted code to your sun's CSS:

    ![screenshot](images/sunrise-sunrise.png)

    This tells the sun to spend 10 seconds animating a sunrise.

+ To run the animation again in Trinket, just click **Autorun**. 

## Save Your Project {.save}

##Challenge: Diagonal animation {.challenge}
Can you add code to your `sunrise` animation, to make your sun start at the bottom left of the sky and move diagonally to its position at roughly the top center?

You can use the `left` property to do this, for example:

```
left: 40%;
```

![screenshot](images/sunrise-left.png)

## Save Your Project {.save}


# Step 3: Infinite animation { .activity}

Let's make the animation keep repeating forever.

## Activity Checklist { .check}

+ If you want the sun to rise and then set, just add more keyframes to your animation:

    ```
    @keyframes sunrise {
        0%   {top:90%; left:0;}
        33%  {top:0; left:40%; }
        66%  {top:0; left:40%; }
        100% {top:90%; left:80%; }
    }
    ```

    This means that the animation starts and ends with the sun at the bottom of the sky, and stays at the top from 33% until 66% of the animation.

+ Now you just need to add the word `infinite` to the `#sun` animation to make it loop forever:

    ![screenshot](images/sunrise-infinite.png)

+ Test out your animation. Does the sun keep rising and setting? 


## Save Your Project {.save}

# Step 4: Animating the sky { .activity}

Animation isn't just for movement. Let's animate the sky to turn dark at night.

## Activity Checklist { .check}

+ Add an animation called `sky` to your CSS:

    ```
    @keyframes sky {
        0% {background: black}
        100% {background: lightblue}
    }
    ```

    Notice that this time you're animating the colour of the sky, and not the position.

+ Add code to your sky, to tell it to use your new animation:

    ```
    animation: sky 10s;
    ```

    ![screenshot](images/sunrise-sky.png)

+ Click **Autorun** to test your animation. 

## Save Your Project {.save}

##Challenge: Improve the sky {.challenge}

Can you change the sky animation so that it matches the sun and stays blue during the day and returns to black as the sun sets. Make it loop forever too. 

![screenshot](images/sunrise-sky-challenge.png)

##Challenge: More animation {.challenge}

Can you animate another image? You can animate the position, colour, shape, size, opacity (seethroughness) or anything else you can think of. Also try changing the amount of time your animations run for. 

For each item you want to animate, you will need to:

+ Include it in your HTML with an id
+ Add a style for the id
+ Create an @keyframes rule
+ Use `animation:` in the style to use the animation you defined with @keyframes 

Click on the image icon to see the images that are included in the project:

![screenshot](images/sunrise-images.png)

You can also upload your own images if you like. 

Don't forget you can put items in the sea as well as the sky:

![screenshot](images/sunrise-boat.png)

In the example the rainbow uses opacity for a fade effect:

```
@keyframes fade {
  0%   {opacity: 0;}
  50%  {opacity: 100;}
  66%  {opacity: 0;}
  100%   {opacity: 0;}
}
```

The boat uses a negative starting position so that you can't see it for part of the animation:

```
 @keyframes left-right {
  0%    {left:-50%;}
  100%  {left:200%;}
}
```

## Save Your Project {.save}
