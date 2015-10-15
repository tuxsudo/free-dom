# Free-DOM

A composition of small micro-libraries for interacting with the DOM.


## qsa

A small shortcut to using `querySelectorAll()` which also coerces NodeList to an Array.

	import qsa from 'qsa';

	qsa('p'); // returns an array of all matching `<p>` tags.



## class-acts

Lamda function factories for adding, removing, & toggling a CSS class on HTML Elements.

	import qsa from 'qsa';
	import classActs from 'class-acts';

	qsa('p')
		.map( classActs.add('my-class') )
		.map( classActs.toggle('your-class') )
		.map( classActs.remove('its-class') );


## attr-boy

Lamds function factories for adding, removing, & toggling data attributes.

	import qsa from 'qsa';
	import toggleAttr from 'attr-boy/toggle';

	qsa('p')
		.map(toggleAttr('data-is-on'));


## dom-emit

Emit custom events in the DOM. For modern browsers and IE9+. Polyfill included.

	import qsa from 'qsa';
	import emit from 'dom-emit';

	emit('my-event-name');
	emit.from(document.body, 'another-custom-event', {data: true});
	qsa('p').map( emit.map('custom-event') );



