# Vertical Rhythm Images
A lightweight, simple and easy to use jQuery script that resizes images according to the vertical rhythm.

[Check the Demo Here]()

## How it Works
1. The function first checks the width of the users' screen / browser window,
2. checks the height of the images,
3. compares the screen width to the break points (you have to set them in the function options) and gets the right line-height,
4. height of the image gets divided by the line-height and round downward to its nearest integer,
5. new height gets calculated and applied to the image.

##Usage

You will have to set the options (breakpoints and line-heights) according to your line-height. For further details on vertical rhythm and how to use this script read the Handcrafting Web Typography article.

Call in the Vertical Rhythm Images script.
```HTML
<script type="text/javascript" src="verticalRhythmImages.js"></script>
```
Initiate the function on your images.
```JavaScript
$('img').imgFixHeight({[
	{
	  	// Breakpoint 1: Mobile
		breakpointStart: 0, // Breakpoint start
		breakpointEnd: 600, // Breakpoint end
		lh: 23 // Line-height to be used 
	},
	{
	  	// Breakpoint 2: Tablet & Desktop
		breakpointStart: 601,
		breakpointEnd: Infinity,
		lh: 27
	}
]});
```
This is an example with two breakpoints. One for the mobile line-height (23px) and text sizes and another for tablet and desktop (27).
