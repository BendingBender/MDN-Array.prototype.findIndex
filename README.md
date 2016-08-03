[![Build Status](https://travis-ci.org/BendingBender/MDN-Array.prototype.findIndex.svg?branch=master)](https://travis-ci.org/BendingBender/MDN-Array.prototype.findIndex)

# ES6 `Array.prototype.findIndex` shim

Simple ES6 [Array.prototype.findIndex](http://people.mozilla.org/%7Ejorendorff/es6-draft.html#sec-array.prototype.findindex) polyfill for older environments taken from [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex#Polyfill).

For browsers only, bower-friendly. Explicitly not meant to be used with node, use the following [shim](https://github.com/paulmillr/Array.prototype.findIndex) if you wish a shim for node.

## Installation
* Just include repo before your scripts.
* `bower install mdn-array.prototype.findindex`

## Usage

* `Array.prototype.findindex(predicate[, thisArg])` returns first item index that matches `predicate` function.
* `predicate(value, index, collection)`: takes three arguments
    * `value`: current collection element
    * `index`: current collection element index
    * `collection`: the collection

Code example:

```javascript
// Default:
[1, 5, 10, 15].findIndex(function(a) {return a > 9;}) // 2
```


## Acknowledgements

Tests, readme and travis support gratefully taken from [Array.prototype.findIndex](https://github.com/paulmillr/Array.prototype.findIndex)

## License
CC0 1.0
