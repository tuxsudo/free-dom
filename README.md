# Free-DOM

A composition of small micro-libraries for interacting with the DOM. Modules are designed and encouraged to be used a-la-carte, but a window global can be used if it's preferred.


	qsa('p')
		.map( addClass('my-class') );


## qsa

A small shortcut to using `querySelectorAll()` which also coerces list to an Array.

	import qsa from 'qsa';

	qsa('p'); // returns an array of all matching `<p>` tags.



## css-class-acts

	import qsa from 'qsa';
	import addClass from 'css-class-acts/add';

	qsa('p').addClass('my-class');


## dom-emit





