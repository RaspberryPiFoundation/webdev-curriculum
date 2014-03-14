---
title: Audio and video on web pages 
level: Lesson 8
language: en-GB
embeds: "*.png"
materials: "code and images"
stylesheet: web
...

# Introduction { .intro}

There are a few ways to add videos or audio to your pages. Let's  have a closer look at them together.

# Add a video from YouTube { .activity}

Adding videos from YouTube is really simple.

+ Go to the video page on YouTube.
+ Under the video player you can find the `Share` button. Click that.
+ To get the code you can use on your web page, click `Embed`.

It will look something like this:

```
<iframe width="560" height="315" src="http://www.youtube.com/embed/FxhGIajRsq4"
   frameborder="0" allowfullscreen></iframe>
```

This specific code fragment would add a CodeClub video to your page. Just copy and past it where you would like the video to appear.

Notice the `width` and `height` attributes. They allow you to control how big will the video be on the page, so feel free to change them.


# Add a video from Vimeo. { .activity}

+ Go to the video page on Vimeo.
+ Click the `Share` button on the video player.
+ On the right hand side there is an Embed box. Click it to select the code and copy it. It will look a bit like this:

```
<iframe src="http://player.vimeo.com/video/44738167" width="600" height="338" 
   frameborder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>
```

+ Paste the code where you would like the video to appear on the page. Notice the `width` and `height` attributes. They allow you to control how big will the video be on the page, so feel free to change them.

# Adding a video file from your computer { .activity}

If you have a video you have created you can put it on your page without having to upload it to YouTube or Vimeo.

+ To place a video on your page you will need to add a `video` tag. Just like the `<img>` tag is has the `src` attribute pointing to the file:

```
	<video src="spaceship_landing.mp4">
	</video>
```

Sadly the annoying thing about adding video that was is that not every browser can play all of the video formats. You will have to save it in at least `.mp4` and `.ogv` formats, which will work in most browsers.

To let the browser know we have more than one format of video ready, write it like this:

```
	<video>
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ To add a picture that will be seen before the video plays, you can use a `poster` attribute:

```
	<video poster="spaceship_landing.jpg">
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ If you want to automatically play the video, you can add the `autoplay` keyword, like this:

```
	<video poster="spaceship_landing.jpg" autoplay>
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ To display video controls, such as the play button, the volume and so on you can add the `controls` keyword:

```
	<video poster="spaceship_landing.jpg" controls>
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

+ You can also control the size of the video using the `width` and `height` attributes. Write this:

```
	<video poster="spaceship_landing.jpg" width="600" height="400">
		<source src="spaceship_landing.ogv" type="video/ogg">
		<source src="spaceship_landing.mp4" type="video/mp4">
	</video>
```

# Adding an audio file from your computer { .activity}

The way to add audio files to your page from your computer is similar to adding video file.

+ To place the audio on page write this:

```
	<audio src="spaceship.mp3">
	</audio>
```

Notice the `src` attribute which points to the file.

Just like with video, not every browser can play every type of audio file, so to make sure as many people as possible can hear the audio you have to add the file in more than one format, at least in `.mp3` and `.oga`.

```
	<audio>
 		<source src="spaceship.mp3" type='audio/mp3'>
 		<source src="spaceship.ogg" type='audio/ogg; codecs=vorbis'>
	</audio>
```

+ To add the controls you need to add the `controls` keyword:

```
	<audio controls>
 		<source src="spaceship.mp3" type='audio/mp3'>
 		<source src="spaceship.ogg" type='audio/ogg; codecs=vorbis'>
	</audio>
```

+ If you want the audio to play as soon as the page loads, you can add the `autoplay` keyword, like this:

```
	<audio controls autoplay>
 		<source src="spaceship.mp3" type='audio/mp3'>
 		<source src="spaceship.ogg" type='audio/ogg; codecs=vorbis'>
	</audio>
```
