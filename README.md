# Vertical Rhythm Images
A lightweight, simple and easy to use jQuery script that resizes images according to the vertical rhythm.

[View Demo]()

## How it Works
1. The function first checks the width of the users' screen / browser window,
2. checks the height of the images,
3. compares the screen width to the break points (you have to set them in the function options) and gets the right line-height,
4. height of the image gets divided by the line-height and round downward to its nearest integer,
5. new height gets calculated and applied to the image.

##Usage
An example with two breakpoints (very common for a responsive website where you have different line-heights for mobile and desktop version).
```
$('img').imgFixHeight({[
	{
	  	// Breakpoint 1: Mobile
		breakpointStart: 0,	// Breakpoint start
		breakpointEnd: 600,	// Breakpoint end
		lh: 23 // line height	// Line height used 
	},
	{
	  	// Breakpoint 2: Tablet & Desktop
		breakpointStart: 601,
		breakpointEnd: Infinity,
		lh: 27
	}
]});
```
For further details on vertical rhythm and how to use this script read the Handcrafting Web Typography article.
