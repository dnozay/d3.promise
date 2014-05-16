d3.promise
==========

Make d3 data functions use promises instead of callbacks

This library uses ES6 Promise. (http://www.html5rocks.com/en/tutorials/es6/promises/)
To bring browsers that lack a complete promises implementation up to spec compliance, or add promises to other browsers and Node.js, check out the polyfill (2k gzipped).

### Example Usage

```
var promise = d3.promise.csv('test.csv');
promise.then(function(data){}, function(error){});

var promise = d3.promise.tsv('test.tsv');
promise.then(function(data){}, function(error){});

var promise = d3.promise.json('test.json')
promise.then(function(data){}, function(error){});

var promise = d3.promise.xml('test.xml')
promise.then(function(data){}, function(error){});
```
