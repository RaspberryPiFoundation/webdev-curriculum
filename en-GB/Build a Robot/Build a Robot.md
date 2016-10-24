---
title: Build a Robot
level: HTML & CSS 2
language: en-GB
embeds: "*.png"
materials: ["Club Leader Resources/robot-finished/*.*","Project Resources/robot/*.*", "Project Resources/template/*.*"]
stylesheet: web
...

# Introduction { .intro}

In this project, you’ll learn how to position images to create your own robot!

![screenshot](robot-final.png)

# Step 1: Giving your robot eyes { .activity}

Let’s give your robot some eyes!

## Activity Checklist { .check}

+ Open this trinket: <a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a>. If you're reading this online, you can also use the embedded version of this trinket below.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/b29b50e571" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ Each image in this project has it’s own name (or __id__). For example, the HTML for the face and eye images (‘face’, ‘eyes1’ and ‘eyes2’ starting on line 8 of your code) looks like this:

```
<img id="face" ...>
<img id="eyes1" ...>
<img id="eyes2" ...>
```

+ You can use an image’s id to give it it’s own style, by using the `#` symbol. This allows you to style each image separately.

Click on the `style.css` file. Notice how the size of the robot’s face and the other images are different?

![screenshot](robot-id.png)

+ Add this CSS code to style the robot’s eyes:

```
#eyes1 {
    width: 200px;
}
```

Notice that you’re styling just the `eyes1` image, by using `#eyes1` in your CSS. If you prefer, you can use `#eyes2` or `#eyes3` instead!

![screenshot](robot-eyes-width.png)

+ Notice how each image is displayed one after the other? This is called __relative__ positioning. If you want to tell the browser exactly where to place your robot’s eyes, you’ll need to use __absolute__ positioning instead.

Add these 3 lines of code to the CSS for your `eyes1` image:

```
position: absolute;
top: 200px;
left: 100px;
```

You should see that your robot’s eyes move to the correct place on your robot.

![screenshot](robot-eyes-position.png)

This CSS code tells the browser how far from the top / left of the webpage to display the image.

![screenshot](robot-eyes-position2.png)

You can use `bottom` instead of `top` to tell the browser how far from the bottom of the screen to show the image, as well as using `right` instead of `left`.

# Step 2: Giving your robot a mouth { .activity}

Let’s give your robot a mouth!

## Activity Checklist { .check}

+ Add the following CSS code to style your `mouth1` image:

```
#mouth1 {
    width: 50px;
    position: absolute;
    top: 200px;
    left: 200px;
}
```

+ Your robot’s mouth looks quite small, and isn’t in the right place.

![screenshot](robot-mouth.png)

Can you fix this, by making changes to your CSS?

## Save Your Project {.save}

##Challenge: Design your own robot {.challenge}
Use what you’ve learnt to finish designing your own robot. Here are some examples of how your robot might look:

![screenshot](robot-examples.png)

## Save Your Project {.save}

##Challenge: Add your own images {.challenge}
Can you find extra images to add to your robot, and position them on your webpage? You could even replace the robot face with your own!

```
<img id="face" src="myFace.png">
```

## Save Your Project {.save} 