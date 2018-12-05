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
let BigInterval = require('biginterval');
let interval = 4294967295;

let myBigInterval = new BigInterval();
myBigInterval.set(function (message) {
  console.log(message);
}, interval, 'Hello world!');
```
To clear an interval:
```javascript
myBigInterval.clear();
```

# License
MIT License

Copyright (c) 2018 Majid Yaghouti

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.