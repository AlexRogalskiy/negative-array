# negative-array [![Build Status](https://travis-ci.org/sindresorhus/negative-array.svg?branch=gh-pages)](https://travis-ci.org/sindresorhus/negative-array)

> Negative array index support `array[-1]` using ES2015 Proxy

JavaScript doesn't natively support the use of a negative index to get items backwards from the end, but with [ES2015 Proxy](http://soft.vub.ac.be/~tvcutsem/proxies/) it's possible. Take a look at the [source](index.js) to see how simple it is to implement and read this [short article](http://dailyjs.com/2013/11/15/negative-array/) about it.

> Proxies are objects for which the programmer has to define the semantics in JavaScript. The default object semantics are implemented in the JavaScript engine, often written in lower-level languages like C++. Proxies let the programmer define most of the behavior of an object in JavaScript. They are said to provide a meta-programming API.


## Usage

```
$ npm install negative-array
```

```js
const negativeArray = require('negative-array');

// Adds negative array index support to any given array
const unicorn = negativeArray(['pony', 'cake', 'rainbow']);

// Get the last item by using a negative index
console.log(unicorn[-1]);
//=> 'rainbow'

// OMG, YES!
```


## License

MIT © [Sindre Sorhus](https://sindresorhus.com)
