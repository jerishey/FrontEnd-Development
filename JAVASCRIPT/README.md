# JavaScript
JavaScript is a programming language used to create dynamic content for websites. It is a lightweight, cross-platform, and single-threaded programming language. It's an interpreted language that executes code line by line, providing more flexibility.

## Features :
```bash
1. Lightweight & Interpreted : JavaScript runs directly in the browser without compilation, making it fast and easy to use.

2. Dynamic Typing : No need to declare data types—variables can change type automatically.

3. Event-Driven : JavaScript responds to user actions like clicks, typing, and mouse movements.

4. Asynchronous Programming : It can perform tasks (like API calls) in the background without stopping the program.

5. Object-Oriented : Supports objects, classes, and inheritance to organize code efficiently.

6. Platform Independent : Runs on any device or operating system with a web browser.
```

## Client Side and Server Side nature of JavaScript
JavaScript's flexibility extends to both the client-side and server-side, allowing developers to create complete web applications. Here’s how it functions in each environment:

`1. Client-Side`
```bash
1. Involves controlling the browser and its DOM (Document Object Model).

2. Handles user events like clicks and form inputs.

3. Common libraries include AngularJS, ReactJS, and VueJS.
```
`2. Server-Side`
```bash
1. Involves interacting with databases, manipulating files, and generating responses.

2. Node.js and frameworks like Express.js are widely used for server-side JavaScript, enabling full-stack development.
```

## Limitations of JavaScript
```bash
1. Security Risks : Can be used for attacks like Cross-Site Scripting (XSS), where malicious scripts are injected into a website to steal data by exploiting elements like <img>, <object>, or <script> tags.

2. Performance : Slower than traditional languages for complex tasks, but for simple tasks in a browser, performance is usually not a major issue.

3. Complexity : To write advanced JavaScript, programmers need to understand core programming concepts, objects, and both client- and server-side scripting, which can be challenging.

4. Weak Error Handling and Type Checking : Weakly typed, meaning variables don’t require explicit types. This can lead to issues as type checking is not strictly enforced.
```

## Adding JavaScript in HTML Document
JavaScript can be included in an HTML document to add interactivity and dynamic behavior to web pages. It allows the browser to execute scripts that can modify content, handle events, and communicate with servers.

```bash
1. Inline JavaScript: Code written directly inside HTML tags using attributes like onclick.

2. Internal JavaScript: Script written inside the <script> tag within the HTML file.

3. External JavaScript: JavaScript stored in a separate .js file and linked using the <script src="file.js"></script> tag.
```

### Example :

`1. Inline JavaScript` : You can write JavaScript code directly inside the HTML element using the onclick, onmouseover, or other event handler attributes.
```bash
<html>
<head></head>
<body>
    <h2>
        Adding JavaScript in HTML Document
    </h2>
    <button onclick="alert('Button Clicked!')">
        Click Here
    </button>
</body>
</html>
```
<br>

`2. Internal JavaScript (Within <script> Tag)` : You can write JavaScript code inside the `<script>` tag within the HTML file. This is known as internal JavaScript and is commonly placed inside the `<head>` or `<body>` section of the HTML document.

<i>

```bash
1. JavaScript Code Inside <head> Tag : Placing JavaScript within the <head> section of an HTML document ensures that the script is loaded and executed as the page loads. This is useful for scripts that need to be initialized before the page content is rendered.

Example:
<html>
<head>
    <script>
        function myFun() {
            document.getElementById("demo")
                .innerHTML = "Content changed!";
        }
    </script>
</head>
<body>
    <h2>
        Add JavaScript Code
        inside Head Section
    </h2>
    <h3 id="demo" style="color:green;">
        JavaScript
    </h3>
    <button type="button" onclick="myFun()">
        Click Here
    </button>
</body>
</html>

2. JavaScript Code Inside <body> Tag : JavaScript can also be placed inside the <body> section of an HTML page. Typically, scripts placed at the end of the <body> load after the content, which can be useful if your script depends on the DOM being fully loaded.

Example:
<html>
<head></head>
<body>
    <h2>
        Add JavaScript Code
        inside Body Section
    </h2>
    <h3 id="demo" style="color:green;">
        JavaScript
    </h3>
    <button type="button" onclick="myFun()">
        Click Here
    </button>
    <script>
        function myFun() {
            document.getElementById("demo")
                .innerHTML = "Content changed!";
        }
    </script>
</body>
</html>
```
</i>

`3. External JavaScript (Using External File)` : For larger projects or when reusing scripts across multiple HTML files, you can place your JavaScript code in an external .js file. This file is then linked to your HTML document using the src attribute within a `<script>` tag.

```bash
<html>
<head>
    <script src="script.js"></script>
</head>
<body>
    <h2>
        External JavaScript
    </h2>
    <h3 id="demo" style="color:green;">
        JavaScipt
    </h3>
    <button type="button" onclick="myFun()">
        Click Here
    </button>
</body>
</html>

/* Filename: script.js*/

function myFun () {
    document.getElementById('demo')
        .innerHTML = 'Content Changed'
}
```
### Advantages of External JavaScript
```bash
1. Faster Page Load Times: Cached external JavaScript files don’t need to be reloaded every time the page is visited, which can speed up loading times.

2. Improved Readability and Maintenance: Keeping HTML and JavaScript separate makes both easier to read and maintain.

3. Separation of Concerns: By separating HTML (structure) and JavaScript (behavior), your code becomes cleaner and more modular.

4. Code Reusability: One external JavaScript file can be linked to multiple HTML files, reducing redundancy and making updates easier.
```

## 1. Data Types
JavaScript data types define what kind of values a variable can hold and how those values behave in a program. They determine how data is stored in memory and how operations like comparison, calculation, and conversion work.

- Each data type has its own methods and operations that control how it can be used.
- Understanding data types helps prevent errors and makes code more efficient and reliable.

### Data Type Categories
`1. Primitive Data Type` : Primitive data types in JavaScript represent simple, immutable values stored directly in memory, ensuring efficiency in both memory usage and performance.
```bash
1. Number : The Number data type in JavaScript includes both integers and floating-point numbers. Special values like Infinity, -Infinity, and NaN represent infinite values and computational errors, respectively.

Example:
let n1 = 2;
console.log(n1)

let n2 = 1.3;
console.log(n2)

2. String : A String in JavaScript is a series of characters that are surrounded by quotes. There are three types of quotes in JavaScript, which are.

Example:
let s1 = "Hello There";  # using double quotes
console.log(s1); 

let s2 = 'Single quotes work fine'; # using single quotes
console.log(s2); 

let s3 = `can embed ${s1}`; # using backticks
console.log(s3);

3. Boolean : The boolean type has only two values i.e. true and false.

Example:
let b1 = true;
console.log(b1);  

let b2 = false;
console.log(b2);

4. Null : The special null value does not belong to any of the default data types. It forms a separate type of its own which contains only the null value.

Example:
let age = null;
console.log(age)
- The 'null' data type defines a special value that represents nothing, or empty value.

5. Undefined : A variable that has been declared but not initialized with a value is automatically assigned the undefined value. It means the variable exists, but it has no value assigned to it.

Example:
let a;
console.log(a);

6. Symbol (Introduced in ES6) : Symbols, introduced in ES6, are unique and immutable primitive values used as identifiers for object properties. They help create unique keys in objects, preventing conflicts with other properties.

Example:
let s1 = Symbol("Java");
let s2 = Symbol("Script");
console.log(s1 == s2);

7. BigInt (Introduced in ES2020) : BigInt is a built-in object that provides a way to represent whole numbers greater than 253. The largest number that JavaScript can reliably represent with the Number primitive is 253, which is represented by the MAX_SAFE_INTEGER constant.

Example:
let b = BigInt("0b1010101001010101001111111111111111");
console.log(b);
```

`2. Non-Primitive Data Types` : The data types that are derived from primitive data types are known as non-primitive data types. It is also known as derived data types or reference data types.

```bash
1. Object : JavaScript objects are key-value pairs used to store data, created with {} or the new keyword. They are fundamental as nearly everything in JavaScript is an object.

Example:
let abc = {
    type: "Company",
    location: "Noida"
}
console.log(abc.type)

2. Arrays : An Array is a special kind of object used to store an ordered collection of values, which can be of any data type.

Example:
let a1 = [1, 2, 3, 4, 5];
console.log(a1);

let a2 = [1, "two", { name: "Object" }, [3, 4, 5]];
console.log(a2);

3. Function : A function in JavaScript is a block of reusable code designed to perform a specific task when called.

Example:
// Defining a function to greet a user
function greet(name) { return "Hello, " + name + "!"; }
// Calling the function
console.log(greet("Ajay"));

4. Date Object : The Date object in JavaScript is used to work with dates and times, allowing for date creation, manipulation, and formatting.

Example:
// Creating a new Date object for the
// current date and time
let currentDate = new Date();

// Displaying the current date and time
console.log(currentDate);

5. Regular Expression : A RegExp (Regular Expression) in JavaScript is an object used to define search patterns for matching text in strings.

Example:
// Creating a regular expression to match the word "hello"
let pattern = /hello/;

// Testing the pattern against a string
// Returns false because "hello" is not present
let result = pattern.test("Hello, world!"); 

console.log(result);
```
### Facts about Data Types
`1. Dynamically Typed :` JavaScript Variables are not bound to a specific data type. Mainly data type is stored with value (not with variable name) and is decided & checked at run time.
```bash
let x = 42;   
console.log(x)

x = "hello";  
console.log(x)

x = [1, 2, 3]
console.log(x)
```
`2. Everything is an Object (Sort of) :` In JavaScript, Functions are objects, arrays are objects, and even primitive values can behave like objects temporarily when you try to access properties on them.
```bash
let s = "hello";
console.log(s.length);  

// Example with a number
let x = 42;
console.log(x.toString()); 

// Example with a boolean
let y = true;
console.log(y.toString());

/* Internal Working of primitives
   to be treeated as objects
   
// Temporary wrapper object
let temp = new String("hello"); 

console.log(temp.length); // 5

// The wrapper is discarded after use
temp = null; */
```

`3. NaN is not equal to itself :` NaN Stands for “Not-a-Number”, It is used to represent a computational error. NaN is technically of type number.
```bash
console.log(typeof NaN);
console.log(NaN === NaN);
```

`4. A Symbol is Never Equal to Another One :` Symbol is a unique and immutable data type often used for creating private properties and methods. Symbols are never equal to any other Symbol.
```bash
let s1 = Symbol("abc");
let s2 = Symbol("abc");
console.log(s1 === s2);
```

`5. Undefined and Null :` undefined represents a variable that has been declared but not assigned, while null is an explicit assignment representing “no value”.

`6.` Integers are Floating are Numbers only. There is only one type number that covers both integers and floating point numbers.

`7.` A character is also a string. There is no separate type for characters. A single character is also a string.
```bash
let s1 = "gfg";   // String
let s2 = 'g';    // Character

console.log(typeof s1); 
console.log(typeof s2);
```

## 2. Variables
Variables in JavaScript are used to store data values. They can be declared in different ways depending on how the value should behave.
```bash
1. Variables can be declared using var, let, or const.
2. JavaScript is dynamically typed, so types are decided at runtime.
3. You don’t need to specify a data type when creating a variable.

Example:
// Old style
var a = 10    

// Prferred for non-const
let b = 20;    

// Preferred for const (cannot be changed)
const c = 30;  

console.log(a);
console.log(b);
console.log(c);
```

### Declaring Variables in JavaScript
```bash
1. Before ES6 (2015): Variables were declared only with var, which is function-scoped and global-scoped, causing issues like hoisting and global pollution.

2. ES6 Introduction:let and const were introduced to provide safer alternatives for declaring variables.

3. Scope: let and const are block-scoped (limited to { } block) or global-scoped, reducing errors compared to var.
```

`1. var keyword :` var is a keyword in JavaScript used to declare variables and it is Function-scoped and hoisted, allowing redeclaration but can lead to unexpected bugs.

```bash
var a = "Hello Jerishey";
var b = 10;
console.log(a);
console.log(b);
```
`2. let keyword :` let is a keyword in JavaScript used to declare variables and it is Block-scoped and not hoisted to the top, suitable for mutable variables.

```bash
let a = 12
let b = "js";
console.log(a);
console.log(b);
```

`3. const keyword :` const is a keyword in JavaScript used to declare variables and it is Block-scoped, immutable bindings that can't be reassigned, though objects can still be mutated.

```bash
const a = 5
let b = "js";
console.log(a);
console.log(b);
```
### Rules for Naming Variables
```bash
1. Variable names must begin with a letter, underscore (_), or dollar sign ($).

2. Subsequent characters can be letters, numbers, underscores, or dollar signs.

3. Variable names are case-sensitive (e.g., age and Age are different variables).

4. Reserved keywords (like function, class, return, etc.) cannot be used as variable names.

Example:
let userName = "Suman";  // Valid
let $price = 100;         // Valid
let _temp = 0;            // Valid
let 123name = "Ajay";    // Invalid
let function = "js"; // Invalid
```
### Scope of Variables in JavaScript
Scope determines where a variable can be accessed or used within a JavaScript program. It helps control the visibility and lifetime of variables in different parts of the code.

```bash
// Declaring a global variable
let x = 10;

function func() {
    
    // Declaring a local variable
    let y = 20;

    // Accessing Local and Global
    // variables
    console.log(x,",", y);
}

func();
```
<b>Global and Local Scope :</b>

`1. Global Scope :` A global variable refers to a variable that is declared outside any function or block, so it can be used anywhere in the program, both inside functions and in the main code.

```bash
// Global Variable accessed from within a function 
const x = 10;

function fun1() {
    console.log(x);
}

fun1();

Explanation: In the program, the variables outside the function and now we can access those variables from anywhere in the JavaScript program.
```

`2. Local Scope :` A local variable is a variable declared inside a function, making it accessible only within that function. It cannot be used outside the function.

```bash
function fun2(){
    
    // This variable is local to fun2() and 
    // cannot be accessed outuside this function
    let x = 10;
    console.log(x);
}

fun2();

Explanation: Here, the code defines a function fun2 with a local variable x, which is accessible only inside the function, and prints its value when the function is called.
```
<b>Block and Lexical Scope :</b>

`1. Block and Lexical Scope :` In JavaScript, block scope refers to variables declared with let or const inside a { } block. These variables are accessible only within that block and not outside it.
<br>

<i>
Variables declared with var do not have block scope. A var variable declared inside a function is accessible throughout that entire function, regardless of any blocks (like if statements or for loops) within the function.  If var is declared used outside of any function, it creates a global variable.
</i>

```bash
{
    
    // Var can Accessible inside & outside the block scope 
    var x = 10;
    
    // let , const Accessible only inside the block scope
    const y = 20;
    let z = 30;
    
    console.log(x);
    console.log(y);
    console.log(z);
}

console.log(x);
```

`2. Lexical Scope :` The variable is declared inside the function and can only be accessed inside that block or nested block is called lexical scope.

```bash
function func1() {
    const x = 10;

    function func2() {
        const y = 20;
        console.log(`${x} ${y}`);
    }

    func2();
}

func1();

Explanation: This code demonstrates lexical scope, where func2 accesses the variable x from func1 and prints “10 20”.
```

`3. Modular Scope :` Module scope refers to variables and functions that are accessible only within a specific JavaScript module. It helps keep code organized and prevents variables from affecting the global scope.

```bash
// math.js (module file)
export const number = 10;

export function add(a, b) {
  return a + b;
}

// main.js (another file)
import { number, add } from "./math.js";

console.log(number);      // 10
console.log(add(5, 3));   // 8

Expalnation: 
- math.js has variables and functions inside its module scope.
- They are only accessible in other files when we use export and import.
```

### Difference between var, let and const keywords in JavaScript
JavaScript provides three ways to declare variables: var, let, and const, but they differ in scope, hoisting behaviour, and re-assignment rules.
<i>

| `var`                                                | `let`                                                 | `const`                                               |
| ---------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- |
| Has **function/global scope**                        | Has **block scope**                                   | Has **block scope**                                   |
| Can be **re-declared and updated**                   | Can be **updated but not re-declared**                | Cannot be **updated or re-declared**                  |
| **Initialization not required**                      | **Initialization not required**                       | **Initialization required**                           |
| Can be accessed before declaration (**undefined**)   | Cannot be accessed before declaration (**TDZ error**) | Cannot be accessed before declaration (**TDZ error**) |
| Hoisted and **initialized with undefined**           | Hoisted but **not initialized (TDZ)**                 | Hoisted but **not initialized (TDZ)**                 |
| Attached to **global object** when declared globally | Not attached to global object                         | Not attached to global object                         |

#### Explanation :

```bash
1. var : Declares variables with function or global scope and allows re-declaration and updates within the same scope.

2. let : Declares variables with block scope, allowing updates but not re-declaration within the same block.

3. const : Declares block-scoped variables that cannot be reassigned after their initial assignment.

Example:
// var example
var x = 10;
var x = 20;   // Re-declaration allowed
x = 30;       // Update allowed
console.log(x); // Output: 30


// let example
let y = 10;
// let y = 20; // Re-declaration NOT allowed
y = 25;       // Update allowed
console.log(y); // Output: 25


// const example
const z = 10;
// z = 20;     // Re-assignment NOT allowed
console.log(z); // Output: 10


// Block scope demonstration
if (true) {
  var a = 1;
  let b = 2;
  const c = 3;
}

console.log(a); // Works (var is function/global scoped)
// console.log(b); //  Error (let is block scoped)
// console.log(c); //  Error (const is block scoped)
```
</i>


