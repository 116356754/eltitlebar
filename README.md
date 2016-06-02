# titlebar

Emulate window title bar. 

npm install eltitlebar

# Usage

Used with browserify or in a similar enviroment.

```javascript
var titlebar = require('eltitlebar');

//if you only have close button set only property is true
//default is false
var t = titlebar({only:true});
t.appendTo(document.body);

t.on('close', function(e) {
	console.log('close');
});

// t.element exposes the root dom element
t.element.appendChild(document.createElement('div'));

// Clean up after usage
t.destroy();
```

