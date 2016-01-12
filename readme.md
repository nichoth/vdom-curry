# vdom curry

Curry a vdom component.


## install

    $ npm install vdom-curry


## example

```js
var curry = require('vdom-curry');
var curried = curry(MyComponent, { value: 'example' });
var moreCurry = curry(curried, { valueTwo: 'example two' });
var state = moreCurry();
moreCurry.render(state);  // same as MyComponent.render(state)
```
