# titlebar

Emulate window title bar. 

npm install eltitlebar

# Usage

Used with browserify or in a similar enviroment.

```javascript
var titlebar = require('eltitlebar');

var t = titlebar();
t.appendTo(document.body);

t.on('close', function(e) {
	console.log('close');
});

// t.element exposes the root dom element
t.element.appendChild(document.createElement('div'));

// Clean up after usage
t.destroy();
```

