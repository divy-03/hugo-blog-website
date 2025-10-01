---
title: JavaScript
description: My JS notes for placement prep

date: 2025-09-14T20:12:52+08:00
lastmod: 2025-09-14T20:12:52+08:00
tags:
  - interview
  - notes
categories:
  - prep
---


### var / let

| Feature        | `var`                                          | `let`                                               |
| -------------- | ---------------------------------------------- | --------------------------------------------------- |
| Scope          | Function-scoped                                | Block-scoped                                        |
| Global Binding | Becomes property of global object (`window.x`) | Does **not** attach to global object                |
| Hoisting       | Hoisted, initialized with `undefined`          | Hoisted, but in TDZ (cannot use before declaration) |
| Redeclaration  | Allowed in same scope                          | Not allowed in same scope                           |
| Local Use      | Exists inside functions                        | Exists inside blocks (`if`, `for`, etc.)            |

| Feature       | `var`                 | `let`               | `const`             |
| ------------- | --------------------- | ------------------- | ------------------- |
| Scope         | Function / global     | Block               | Block               |
| Hoisting      | Yes, `undefined` init | Yes, TDZ until init | Yes, TDZ until init |
| Redeclaration | ✅ Allowed             | ❌ Not allowed       | ❌ Not allowed       |
| Reassignment  | ✅ Allowed             | ✅ Allowed           | ❌ Not allowed       |
| Global Object | Attaches to `window`  | Doesn’t attach      | Doesn’t attach      |
### Hoisting 
Hoisting is JavaScript’s behavior of **moving declarations to the top of their scope (function or global)** before code execution.

| Declaration Type | Hoisted?          | Initialized?             | Behavior                                          |
| ---------------- | ----------------- | ------------------------ | ------------------------------------------------- |
| `var`            | Yes               | With `undefined`         | Accessible before declaration (gives `undefined`) |
| `let`            | Yes               | No (TDZ)                 | ReferenceError if accessed before declaration     |
| `const`          | Yes               | No (TDZ)                 | ReferenceError if accessed before declaration     |
| Function Decl.   | Yes               | With function body       | Can call before definition                        |
| Function Expr.   | Yes (`var`/`let`) | Depends on variable type | Error if called before                            |

### Functions 

Function Expression 

```javascript
console.log(sayHi()); // TypeError: sayHi is not a function
const sayHi = function() {
  return "Hi!";
};
```

Named Function 

```javascript
function greet() {
  return "Hello!";
}
```

Arrow Function 

```javascript
const add = (a, b) => a + b;
```

Anonymous Function 

```javascript
setTimeout(function() {
  console.log("Anonymous function");
}, 1000);
```

Immediate Invoked Function 

```javascript
(function() {
  console.log("IIFE runs immediately!");
})();
```

Constructor Function

```javascript
function Person(name) {
  this.name = name;
}
const user = new Person("Divy");
console.log(user.name); // "Divy"
```

Async Function

```javascript
async function fetchData() {
  return "Data received";
}
fetchData().then(console.log); // "Data received"
```

Higher-Order Function

```javascript
function greet(name) {
  return `Hello, ${name}`;
}
function processUserInput(callback) {
  return callback("Divy");
}
console.log(processUserInput(greet)); // "Hello, Divy"
```

### Template Literals 

Embedding variables and expressions directly into a string.

### Data Types

Primitive and Non-Primitive
### == vs === 

== performs type coercion, but === doesn't
```javascript
5 =='5' // true
5 === '5' // false
```

### isNaN() 

checks if a variable is a number 
> isNaN(NaN) // gives false but typeof NaN is number

### Map 
Map maps the array to perform a specific function on each element of the array then return the array after manipulation
