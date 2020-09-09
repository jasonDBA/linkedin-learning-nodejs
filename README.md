# linkedin-learning-nodejs

## What did you learn?

### Give an example of Global Objects in Node.js
* Answer: console, exports, global, module, process, and etc
* More details: https://nodejs.org/api/globals.html

### How to see the current dir path and file name?
* Directory Path: console.log(__dirname);
* File Name: console.log(__filename);

### What is require function? Give me an example
* Require(): A built-in function that returns/loads/caches JavaScript modules.
```
const path = require('path');
console.log(`This file name is ${path.basename(__filename)}`);
```

### what is process.argv property?
* Answer: It returns an array containing the command line arguments passed when the Node.js process was launched.
* Example:
```
const [ , ,firstname, lastname] = process.argv;

console.log(`Your full name is ${firstname} ${lastname}`);
```
```
// In terminal:
node file.js Jason Choi

// Result in console:
Your full name is Jason Choi
```

### What is Module in Node.js?
* Answer: A set of functions you want to include in your application.
