# Monkey Interpreter

This is a simple "tree-walking" interpreter for the Monkey programming language. It is based
on the book "[Writing An Interpreter In Go](https://interpreterbook.com/)" by Thorsten Ball.

## Features
The monkey programming language supports the following features: 
- C-like syntax
- Variable bindings
- Integers and booleans
- Arithmetic expressions
- Built-in functions
- First-class and higher-order functions
- Closures
- A string data structure
- An array data structure
- A hash data structure

### Example
The following code snippet demonstrates the syntax of the Monkey programming language:
```js
// Binding values to names
let age = 1;
let name = "Monkey";
let result = 10 * (20 / 2);

// Arrays and Hashes
let myArray = [1, 2, 3, 4, 5];
let thorsten = {"name": "Thorsten", "age": 28};

// Accessing elements in arrays and hashes
myArray[0] // => 1
thorsten["name"] // => "Thorsten"

// Functions
let add = fn(a, b) { a + b; };
add(1, 2); // => 3

let fibonacci = fn(x) {
    if (x == 0) {
        0
    } else {
        if (x == 1) {
            1
        } else {
            fibonacci(x - 1) + fibonacci(x - 2);
        }
    }
};

// Higher-order functions
let twice = fn(f, x) {
    return f(f(x));
};

let addTwo = fn(x) { 
    return x + 2; 
};

twice(addTwo, 2); // => 6
```


