---
title: Sunrise — Notes for Club Leaders
---

#Introduction:
In this project, children will to learn how to animate a simple scene using CSS. They will use the CSS @keyframes rule to animate various properties of images and divs.

#Online Resources

We recommend using [trinket](https://trinket.io/) to write HTML & CSS online. This project contains the following trinkets:

+ ['Sunrise' starting point](https://trinket.io/html/web-sunrise)

There is also a trinket containing a sample solution to the challenges:

+ ['Sunrise' Finished](https://trinket.io/html/abcc0284a3)

#Offline Resources
This project can be [completed offline](../offline.html) if preferred. You can access the project resources by clicking the 'Download Project Materials' link for this project. This link contains a 'Project Resources' folder, which includes resources that children will need to complete this project offline. Make sure that each child has access to a copy of these resources. This folder includes the following files:

+ template/index.html
+ template/prefix.js
+ template/style.css
+ sunrise/index.html
+ sunrise/style.css
+ sunrise/prefixfree.js
+ sunrise/boat.png
+ sunrise/cloud.png
+ sunrise/helicopter.png
+ sunrise/rainbow.png
+ sunrise/sun.png

You can also find a completed version of this project's challenges in the 'Volunteer Resources' section, which contains:

+ index.html
+ style.css
+ prefixfree.js
+ boat.png
+ sun.png
+ rainbow.png

#Learning Objectives
+ Styling and animation with CSS:
	+ Introducing `@keyframes` rule for defining steps in an animation.
	+ Reinforcing the use of properties to define the size, shape, position and colour of elements on a webpage.

#Challenges
+ "Diagonal animation" - editing animation `@keyframe` properties to use left:;
+ "Improve the sky" - add more keyframes and setting background:.
+ "More animation" - animate more images or elements using a variety of CSS properties. 

#Frequently Asked Questions

+ This project makes use of the javascript `prefixfree.js` library, to allow animation compatibility between browsers. If this library isn't used, then children using older browsers will instead need to declare an animation for their browser, for example:

```
animation: sky 10s infinite; 		  	//for all newer browsers
-webkit-animation: sky 10s infinite;  	// For Webkit browsers(Chrome, Safari...)
-moz-animation: sky 10s infinite;     	// For Mozilla browsers
-o-animation: sky 10s infinite;       	// For Opera browsers
-ms-animation: sky 10s infinite;		// For Microsoft browsers 
```
