# Javascript

## Functions:
JavaScript functions can be defined in several ways. Here are the main syntaxes:

#### 1. Function Declaration
A function declaration defines a function with the specified parameters.

```javascript
function functionName(parameters) {
    // function body
    // code to be executed
}
```

Example:

```javascript
function greet(name) {
    console.log("Hello, " + name);
}

greet("Alice");
```

#### 2. Function Expression
A function expression defines a function inside an expression, and it can be anonymous or named.

```javascript
const functionName = function(parameters) {
    // function body
    // code to be executed
};
```

Example:

```javascript
const greet = function(name) {
    console.log("Hello, " + name);
};

greet("Bob");
```

#### 3. Arrow Function
Arrow functions provide a shorter syntax and lexically bind the `this` value. They are always anonymous.

```javascript
const functionName = (parameters) => {
    // function body
    // code to be executed
};
```

Example:

```javascript
const greet = (name) => {
    console.log("Hello, " + name);
};

greet("Charlie");
```

If the function body contains a single expression, you can omit the braces and `return` keyword:

```javascript
const add = (a, b) => a + b;

console.log(add(2, 3));
```

#### 4. Immediately Invoked Function Expression (IIFE)
An IIFE is a function that runs as soon as it is defined.

```javascript
(function() {
    // function body
    // code to be executed
})();
```

Example:

```javascript
(function() {
    console.log("This function runs immediately!");
})();
```

#### 5. Methods in Object Literals
Functions can be defined as methods in object literals.

```javascript
const obj = {
    methodName(parameters) {
        // function body
        // code to be executed
    }
};
```

Example:

```javascript
const person = {
    name: "Dave",
    greet() {
        console.log("Hello, " + this.name);
    }
};

person.greet();
```

#### 6. Class Methods
Functions can be defined as methods inside a class.

```javascript
class ClassName {
    methodName(parameters) {
        // function body
        // code to be executed
    }
}
```

Example:

```javascript
class Person {
    constructor(name) {
        this.name = name;
    }

    greet() {
        console.log("Hello, " + this.name);
    }
}

const alice = new Person("Alice");
alice.greet();
```

These are the main ways to define and use functions in JavaScript. Each has its use cases and advantages depending on the context of your code.
