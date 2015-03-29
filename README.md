# Vertical Rhythm Images
A simple and easy to use jQuery script that resizes images according to the vertical rhythm.



## How it Works
1. The function first checks the width of the users' screen / browser window,
2. checks the height of the images,
3. compares the screen width to the break points (you have to set them in the function options) and gets the right line-height,
4. height of the image gets divided by the line-height and round downward to its nearest integer,
5. new height gets calculated and applied to the image.

##Usage
`$('img').imgFixHeight({
  
});`
