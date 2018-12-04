# Big Interval
Set intervals with delays greater than maximum delay of javascript's setInterval function.

To install:
> npm install biginterval

Usage:

To set an interval:
```javascript
let BigInterval = require('biginterval');
let interval = 4294967295;

let myBigInterval = new BigInterval(function (message) {
  console.log(message);
}, interval, 'Hello world!');
```
or
```javascript
let myBigInterval = new BigInterval();
let interval = 4294967295;

myBigInterval.set(function (message) {
  console.log(message);
}, interval, 'Hello world!');
```
To clear an interval:
```javascript
myBigInterval.clear();
```
