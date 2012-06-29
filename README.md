jQuery.bgImages.js
==================

jQuery plugin to manage multiple background images for an element, as permitted by CSS3.
Currently supports adding a new background image, and shifting existing background images relative to their current position. 
Future features may include deleting existing background images, and arbitrary repositionning.

Example Usage
-------------

	// Will add image_name.jpg, shifting all other background images left by 5px.
	$('div').bgImages( {add: 'img_name.jpg', shift_tagged: false, left: '5px'} );

For more examples, see included test.html file.

Standard Options
----------------

* add (string):		The URL (relative or absolute) of an image to be added to the background.
* position (string):	The position attribute to apply to any added image. Defaults to 0px 0px.
* repeat (string):	The repeat attribute to apply to any added image. Defaults to no-repeat.
* tags (array): 	Any images whose full path ends in a string contained in this array will be tagged.
* shift_tagged (bool):	If true, all tagged images will be shifted as defined by 'left' and 'right' options. 
 			If false, all untagged images will be so shifted.
* left (string): 	The amount to add to the 'left' position of eligable images, with units. 
			Defaults to 0px (no shift).
* top (string): 	The amount to add to the 'top' position of eligable images, with units. 
			Defaults to 0px (no shift).
						
Developers, check the commented code for additional options, such as 'debug'.

Notes
-----

- If an image has already had its position defined, any shifting via the "left" or "top" options must be done in the same units. Otherwise, no 
shifting will occur.

Author
------

Craig McIntosh  
craigmc.info

Licence
-------

!["Creative Commons License"] (http://i.creativecommons.org/l/by/3.0/88x31.png)

This work is licensed under a [Creative Commons Attribution 3.0 Unported License] (http://creativecommons.org/licenses/by/3.0/).

