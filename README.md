[![browser support](https://ci.testling.com/BendingBender/MDN-Array.prototype.findIndex.png)](https://ci.testling.com/BendingBender/MDN-Array.prototype.findIndex)

[![Build Status](https://travis-ci.org/BendingBender/MDN-Array.prototype.findIndex.svg?branch=master)](https://travis-ci.org/BendingBender/MDN-Array.prototype.findIndex)

# ES6 `Array.prototype.findIndex` shim

Simple ES6 [Array.prototype.findIndex](https://tc39.github.io/ecma262/#sec-array.prototype.findindex) polyfill for older environments taken from [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex#Polyfill).

For browsers only, bower-friendly. Explicitly not meant to be used with node, use [Array.prototype.findIndex](https://github.com/paulmillr/Array.prototype.findIndex) if you wish a shim for node.

## Installation
* Just include repo before your scripts.
* `bower install mdn-array.prototype.findindex`

## Usage

* `Array.prototype.findindex(predicate[, thisArg])` returns first item index that matches `predicate` function.

#### Parameters

* `predicate(value, index, collection)`: takes three arguments
    * `value`: current collection element
    * `index`: current collection element index
    * `collection`: the collection
* `thisArg`: Optional. Object to use as `this` when executing `predicate`.

#### Code example

```javascript
[1, 5, 10, 15].findIndex(function(a) {return a > 9;}) // 2
```


## Acknowledgements

Tests, readme and travis support gratefully taken from [Array.prototype.findIndex](https://github.com/paulmillr/Array.prototype.findIndex)

## License
CC0 1.0
