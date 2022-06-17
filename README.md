# ERRORS PACK

An error pack built with pure **JavaScript** With help of chalk.

## FEATURES
- Built-In Errors
- Create Custom Errors


## INSTALLING

for starting you have to install the package by running 
```shell 
npm i errorspack
```

import the package by typing

 ```js 
 const Error = require("errorspack")
 ```
 on your file.

 ## FUNCTIONS / BUILT-IN ERRORS

 There are built in errors in this pack

 **SOME BUILT-IN ERRORS AND FUCTIONS ARE**
 - NonStringError() - Which is for non string value for example here is a demo code:
 ```js
 const Errors = require("errorspack");

const Name = {
    name: Sam
}

if(typeof(Name) !== "string") {
    throw new Errors.nonStringError("Type of name must be number");
}
```

and the output will be:
```terminal
TypeError: Type of name must be string
```
- NonIntegerError() - which is for non integer value for example here ia another demo code:
```js
 const Errors = require("errorspack");

const Age = {
    age: "26"
}

if(typeof(Age) !== "number") {
  throw new Errors.nonIntegerError("Type of age should be an Integer");
}
```
and the output will be:
```terminal
TypeError: Type of name must be integer/number value
```
- NonBooleanError() - which is for non boolean value (true/false)

## HOW TO CREATE CUSTOM ERROR?
custom error can be created by `CustomError()` constructor

There are two parameters in `CustomError()` constructor. one is **name** another one is **message**.

for example here is another demo:
```js
const Errors = require("errorspack");

const CE = {
    name: ""
}

if(typeof(name) === "undifined") {
    const CustomError = new Errors.customError.CustomError("TypeError", "Type of name shouldn't be undifined");
}
```
and the output will be:
```terminal
TypeError: Type of name shouldn't be undifined
```
## VERSION 2.1
**HOW TO CREATE CUSTOM ERROR?**
```js
const Errors = require("errorspack");

const CE = {
    name: ""
}

if(typeof(name) === "undifined") {
    throw new Errors.customError("Type of name shouldn't be undifined");
}
```

_**NOTE: IN VERSION 2.1 YOU DON'T NEED TO CREATE CUSTOM ERROR**_

### WARNING
Please note that version 0.2.0 has some changes if you have any errors with old method then please use
```js
<packagename>.builtInErrors.<ErrorName>
```

**YOU'VE JUST LEARNED BASIC ABOUT ERRORSPACK!**


**STAY UPDATED**
