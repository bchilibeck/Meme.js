Meme.js
=======

Use one function to generate a meme.

You can call it all with strings:

    var memeCreator = Meme('dog.jpg', 'canvasID', 320, 'Buy pizza, 'Pay in snakes');

Or with a selected canvas element:

    var canvas = document.getElementById('canvasID');
    var memeCreator =Meme('wolf.jpg', canvas, 320, 'The time is now', 'to take what\'s yours');

Or with a jQuery/Zepto selection:

    Meme('spidey.jpg', $('#canvasID'), 320, 'Did someone say', 'Spiderman JS?');

You can also pass in an image:

    var img = new Image();
    img.src = 'insanity.jpg';
    var can = document.getElementById('canvasID');
    var memeCreator = Meme(img, can, 'you ignore my calls', 320, 'I ignore your screams of mercy');

The Meme.js arguments are as follows:

	- Background Image
	- Canvas
	- Max width/height of generated Meme
	- Top Text
	- Bottom Text

You also toggle many text effects:
	
	var memeCreator = Meme(img, can, 'you ignore my calls', 320, 'I ignore your screams of mercy');

	memeCreator.toggleAllCaps();
	memeCreator.toggleItalics();

	//Inverse 8 is default, 6 is larger, 10 is smaller
	memeCreator.setFontSize(6);
	
	//Must be a font family the browser supports
	memeCreator.setFontFamily("Courier");

	memeCreator.updateTopText("top text");
	memeCreator.updateBottomText("bottom text");
	memeCreator.updateText("top text", bottom text");

License info is in LICENSE.txt.
