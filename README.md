# JavaScript Fundamentals Course Guide

## Table of Contents

### Part 1: JavaScript Fundamentals - Basics

1. [Getting Started](#1-getting-started)
2. [Values and Variables](#2-values-and-variables)
3. [Data Types](#3-data-types)
4. [Let, Const, and Var](#4-let-const-and-var)
5. [Basic Operators](#5-basic-operators)
6. [Operator Precedence](#6-operator-precedence)
7. [Strings and Template Literals](#7-strings-and-template-literals)
8. [Taking Decisions: if/else Statements](#8-taking-decisions-ifelse-statements)
9. [Type Conversion and Coercion](#9-type-conversion-and-coercion)
10. [Truthy and Falsy Values](#10-truthy-and-falsy-values)
11. [Equality Operators: == vs ===](#11-equality-operators--vs-)
12. [Logical Operators](#12-logical-operators)
13. [The Switch Statement](#13-the-switch-statement)
14. [Statements and Expressions](#14-statements-and-expressions)
15. [The Conditional (Ternary) Operator](#15-the-conditional-ternary-operator)

### Part 2: JavaScript Fundamentals - Functions, Objects & Loops

16. [Activating Strict Mode](#16-activating-strict-mode)
17. [Functions](#17-functions)
18. [Function Declarations vs Expressions](#18-function-declarations-vs-expressions)
19. [Arrow Functions](#19-arrow-functions)
20. [Functions Calling Other Functions](#20-functions-calling-other-functions)
21. [Introduction to Arrays](#21-introduction-to-arrays)
22. [Basic Array Operations (Methods)](#22-basic-array-operations-methods)
23. [Introduction to Objects](#23-introduction-to-objects)
24. [Dot vs Bracket Notation](#24-dot-vs-bracket-notation)
25. [Object Methods](#25-object-methods)
26. [Iteration: The for Loop](#26-iteration-the-for-loop)
27. [Looping Arrays, Breaking and Continuing](#27-looping-arrays-breaking-and-continuing)
28. [Looping Backwards and Loops in Loops](#28-looping-backwards-and-loops-in-loops)
29. [The while Loop](#29-the-while-loop)

### Coding Challenges

30. [Coding Challenge Solutions](#30-coding-challenges)

### JavaScript with DOM

31. [Embedding JavaScript in HTML](#embedding-javascript-in-html)
32. [NoScript Tag](#noscript-tag)
33. [Interacting With The Browser](#interacting-with-the-browser)
34. [Windows & Frames](#windows--frames)
35. [Document Object Model (DOM)](#document-object-model-dom)
36. [Event Handling](#event-handling)
37. [Forms](#forms)
38. [Cookies](#cookies)
39. [Handling Regular Expressions](#handling-regular-expressions)
40. [Client Side Validations](#client-side-validations)
41. [Projects](#projects)

### Advanced JavaScript

#### Data Structure Operators

42. [Enhanced Object Literals](#enhanced-object-literals)
43. [Destructuring Arrays](#destructuring-arrays)
44. [Destructuring Objects](#destructuring-objects)
45. [The Spread Operator (...)](#the-spread-operator-)
46. [Rest Pattern and Parameters](#rest-pattern-and-parameters)
47. [Short Circuiting (&& and ||)](#short-circuiting--and-)
48. [The Nullish Coalescing Operator](#the-nullish-coalescing-operator)
49. [Logical Assignment Operators](#logical-assignment-operators)
50. [The for-of Loop](#the-for-of-loop)
51. [Optional Chaining](#optional-chaining)
52. [Looping Objects: Object Keys, Values, and Entries](#looping-objects-object-keys-values-and-entries)
53. [Sets](#sets)
54. [New Operations to Make Sets Useful!](#new-operations-to-make-sets-useful)
55. [Maps: Fundamentals](#maps-fundamentals)
56. [Maps: Iteration](#maps-iteration)
57. [Working With Strings - Part 1](#working-with-strings---part-1)
58. [Working With Strings - Part 2](#working-with-strings---part-2)
59. [Working With Strings - Part 3](#working-with-strings---part-3)
60. [Coding Challenges](#coding-challenges)

#### Functions

61. [Default Parameters](#default-parameters)
62. [How Passing Arguments Works: Values vs. Reference](#how-passing-arguments-works-values-vs-reference)
63. [Functions Accepting Callback Functions](#functions-accepting-callback-functions)
64. [Functions Returning Functions](#functions-returning-functions)
65. [The call and apply Methods](#the-call-and-apply-methods)
66. [The bind Method](#the-bind-method)
67. [Coding Challenge #1 - Poll App](#coding-challenge-1---poll-app)
68. [Immediately Invoked Function Expressions (IIFE)](#immediately-invoked-function-expressions-iife)
69. [Closures](#closures)
70. [More Closure Examples](#more-closure-examples)
71. [Coding Challenge #2 - IIFE with Event Listener](#coding-challenge-2---iife-with-event-listener)

#### OOP

72. [Constructor Functions and the new Operator](#constructor-functions-and-the-new-operator)
73. [Prototypes](#prototypes)
74. [Prototypal Inheritance on Built-In Objects](#prototypal-inheritance-on-built-in-objects)
75. [Coding Challenge #1: Car Constructor](#coding-challenge-1-car-constructor)
76. [ES6 Classes](#es6-classes)
77. [Setters and Getters](#setters-and-getters)
78. [Object.create](#objectcreate)
79. [Coding Challenge #2: Car Class with Speed Conversion](#coding-challenge-2-car-class-with-speed-conversion)
80. [Inheritance Between Classes: Constructor Functions](#inheritance-between-classes-constructor-functions)
81. [Coding Challenge #3: Electric Car Inheritance](#coding-challenge-3-electric-car-inheritance)
82. [Inheritance Between Classes: ES6 Classes](#inheritance-between-classes-es6-classes)
83. [Inheritance Between Classes: Object.create](#inheritance-between-classes-objectcreate)
84. [Encapsulation: Private Class Fields and Methods](#encapsulation-private-class-fields-and-methods)
85. [Coding Challenge #4: Electric Car with Private Fields](#coding-challenge-4-electric-car-with-private-fields)

---

## Part 1: JavaScript Fundamentals - Basics

### 1. Getting Started

JavaScript is a powerful programming language that runs in web browsers and many other environments. Let's start with the basics:

```javascript
// Linking a JavaScript File
let js = "amazing";
console.log(40 + 8 + 23 - 10); // Output: 61
```

### 2. Values and Variables

Variables are containers that store data values. In JavaScript, you can create variables using `let`, `const`, or `var`.

```javascript
console.log("Jonas");
console.log(23);

let firstName = "Matilda";
console.log(firstName);

// Variable name conventions
let jonas_matilda = "JM";
let $function = 27;
let person = "jonas";
let PI = 3.1415;

// Descriptive variable names (recommended)
let myFirstJob = "Coder";
let myCurrentJob = "Teacher";

// Less descriptive (not recommended)
let job1 = "programmer";
let job2 = "teacher";
```

**Best Practices for Variable Names:**

- Use camelCase for multiple words
- Start with a letter, underscore, or dollar sign
- Cannot start with a number
- Use descriptive names

### 3. Data Types

JavaScript has several built-in data types:

```javascript
let javascriptIsFun = true; // Boolean
console.log(typeof javascriptIsFun); // "boolean"

console.log(typeof 23); // "number"
console.log(typeof "Jonas"); // "string"

// Dynamic typing - can change variable type
javascriptIsFun = "YES!";
console.log(typeof javascriptIsFun); // "string"

// Undefined
let year;
console.log(year); // undefined
console.log(typeof year); // "undefined"

year = 1991;
console.log(typeof year); // "number"

// Special case - typeof null returns "object" (known bug)
console.log(typeof null); // "object"
```

**JavaScript Data Types:**

- **Number**: Floating point numbers
- **String**: Sequence of characters
- **Boolean**: true or false
- **Undefined**: Value taken by a variable that is not yet defined
- **Null**: Empty value
- **Symbol**: Unique identifier (ES6)
- **BigInt**: Larger integers (ES2020)

### 4. Let, Const, and Var

```javascript
// let - can be reassigned, block-scoped
let age = 30;
age = 31; // OK

// const - cannot be reassigned, block-scoped
const birthYear = 1991;
// birthYear = 1990; // ERROR!
// const job; // ERROR! Must be initialized

// var - older way, function-scoped, avoid using
var job = "programmer";
job = "teacher"; // OK

// Without declaration (creates global property - avoid!)
lastName = "Schmedtmann";
console.log(lastName);
```

**Recommendations:**

- Use `const` by default
- Use `let` when you need to reassign the variable
- Avoid `var` and undeclared variables

### 5. Basic Operators

```javascript
// Math operators
const now = 2037;
const ageJonas = now - 1991; // 46
const ageSarah = now - 2018; // 19
console.log(ageJonas, ageSarah);

console.log(ageJonas * 2, ageJonas / 10, 2 ** 3);
// 2 ** 3 means 2 to the power of 3 = 2 * 2 * 2 = 8

// String concatenation
const firstName = "Jonas";
const lastName = "Schmedtmann";
console.log(firstName + " " + lastName);

// Assignment operators
let x = 10 + 5; // 15
x += 10; // x = x + 10 = 25
x *= 4; // x = x * 4 = 100
x++; // x = x + 1 = 101
x--; // x = x - 1 = 100
console.log(x); // 100

// Comparison operators
console.log(ageJonas > ageSarah); // true
console.log(ageSarah >= 18); // true

const isFullAge = ageSarah >= 18;
console.log(now - 1991 > now - 2018); // true
```

### 6. Operator Precedence

```javascript
const now = 2037;
const ageJonas = now - 1991;
const ageSarah = now - 2018;

// Multiplication and division have higher precedence than comparison
console.log(now - 1991 > now - 2018); // true

// Assignment has right-to-left associativity
let x, y;
x = y = 25 - 10 - 5; // x = y = 10
console.log(x, y); // 10, 10

// Parentheses have highest precedence
const averageAge = (ageJonas + ageSarah) / 2;
console.log(ageJonas, ageSarah, averageAge);
```

### 7. Strings and Template Literals

```javascript
const firstName = "Jonas";
const job = "teacher";
const birthYear = 1991;
const year = 2037;

// Old way - string concatenation
const jonas =
  "I'm " + firstName + ", a " + (year - birthYear) + " year old " + job + "!";
console.log(jonas);

// New way - template literals (ES6)
const jonasNew = `I'm ${firstName}, a ${year - birthYear} year old ${job}!`;
console.log(jonasNew);

// Template literals can be used for any string
console.log(`Just a regular string...`);

// Multi-line strings
// Old way
console.log(
  "String with \n\
multiple \n\
lines"
);

// New way
console.log(`String
multiple
lines`);
```

### 8. Taking Decisions: if/else Statements

```javascript
const age = 15;

if (age >= 18) {
  console.log("Sarah can start driving license 🚗");
} else {
  const yearsLeft = 18 - age;
  console.log(`Sarah is too young. Wait another ${yearsLeft} years :)`);
}

// Using if/else to set values
const birthYear = 2012;
let century;

if (birthYear <= 2000) {
  century = 20;
} else {
  century = 21;
}
console.log(century); // 21
```

### 9. Type Conversion and Coercion

```javascript
// Type Conversion (manual)
const inputYear = "1991";
console.log(Number(inputYear), inputYear); // 1991, "1991"
console.log(Number(inputYear) + 18); // 2009

console.log(Number("Jonas")); // NaN
console.log(typeof NaN); // "number"

console.log(String(23), 23); // "23", 23

// Type Coercion (automatic)
console.log("I am " + 23 + " years old"); // "I am 23 years old"
console.log("23" - "10" - 3); // 10
console.log("23" / "2"); // 11.5

let n = "1" + 1; // '11' (string)
n = n - 1; // 10 (number)
console.log(n); // 10
```

### 10. Truthy and Falsy Values

```javascript
// 5 falsy values: 0, '', undefined, null, NaN
console.log(Boolean(0)); // false
console.log(Boolean(undefined)); // false
console.log(Boolean("Jonas")); // true
console.log(Boolean({})); // true
console.log(Boolean("")); // false

// Practical example
const money = 100;
if (money) {
  console.log("Don't spend it all ;)");
} else {
  console.log("You should get a job!");
}

// Bug example
let height = 0;
if (height) {
  console.log("YAY! Height is defined");
} else {
  console.log("Height is UNDEFINED"); // This will run even though height is defined
}
```

### 11. Equality Operators: == vs ===

```javascript
const age = "18";

// Strict equality (no type coercion)
if (age === 18) console.log("You just became an adult :D (strict)");

// Loose equality (with type coercion)
if (age == 18) console.log("You just became an adult :D (loose)");

// Getting input and converting
const favourite = Number(prompt("What's your favourite number?"));
console.log(favourite);
console.log(typeof favourite);

if (favourite === 23) {
  console.log("Cool! 23 is an amazing number!");
} else if (favourite === 7) {
  console.log("7 is also a cool number");
} else if (favourite === 9) {
  console.log("9 is also a cool number");
} else {
  console.log("Number is not 23 or 7 or 9");
}

// Strict inequality
if (favourite !== 23) console.log("Why not 23?");
```

**Best Practice:** Always use `===` and `!==` for comparisons to avoid unexpected type coercion.

### 12. Logical Operators

```javascript
const hasDriversLicense = true; // A
const hasGoodVision = true; // B

// AND operator
console.log(hasDriversLicense && hasGoodVision); // true

// OR operator
console.log(hasDriversLicense || hasGoodVision); // true

// NOT operator
console.log(!hasDriversLicense); // false

// Complex condition
const isTired = false; // C
console.log(hasDriversLicense && hasGoodVision && isTired); // false

if (hasDriversLicense && hasGoodVision && !isTired) {
  console.log("Sarah is able to drive!");
} else {
  console.log("Someone else should drive...");
}
```

### 13. The Switch Statement

```javascript
const day = "friday";

switch (day) {
  case "monday": // day === 'monday'
    console.log("Plan course structure");
    console.log("Go to coding meetup");
    break;
  case "tuesday":
    console.log("Prepare theory videos");
    break;
  case "wednesday":
  case "thursday":
    console.log("Write code examples");
    break;
  case "friday":
    console.log("Record videos");
    break;
  case "saturday":
  case "sunday":
    console.log("Enjoy the weekend :D");
    break;
  default:
    console.log("Not a valid day!");
}

// Equivalent if/else
if (day === "monday") {
  console.log("Plan course structure");
  console.log("Go to coding meetup");
} else if (day === "tuesday") {
  console.log("Prepare theory videos");
} else if (day === "wednesday" || day === "thursday") {
  console.log("Write code examples");
} else if (day === "friday") {
  console.log("Record videos");
} else if (day === "saturday" || day === "sunday") {
  console.log("Enjoy the weekend :D");
} else {
  console.log("Not a valid day!");
}
```

### 14. Statements and Expressions

```javascript
// Expressions produce values
3 + 4;
1991;
true && false && !false;

// Statements perform actions
if (23 > 10) {
  const str = "23 is bigger";
}

// Template literals expect expressions
const me = "Jonas";
console.log(`I'm ${2037 - 1991} years old ${me}`);
```

### 15. The Conditional (Ternary) Operator

```javascript
const age = 23;

// Ternary operator (condition ? if-true : if-false)
age >= 18
  ? console.log("I like to drink wine 🍷")
  : console.log("I like to drink water 💧");

// Storing result in variable
const drink = age >= 18 ? "wine 🍷" : "water 💧";
console.log(drink);

// Equivalent if/else
let drink2;
if (age >= 18) {
  drink2 = "wine 🍷";
} else {
  drink2 = "water 💧";
}
console.log(drink2);

// Using in template literal
console.log(`I like to drink ${age >= 18 ? "wine 🍷" : "water 💧"}`);
```

---

## Part 2: JavaScript Fundamentals - Functions, Objects & Loops

### 16. Activating Strict Mode

```javascript
"use strict";

let hasDriversLicense = false;
const passTest = true;

if (passTest) hasDriversLicense = true;
if (hasDriversLicense) console.log("I can drive :D");

// Strict mode helps catch common mistakes
// const interface = 'Audio'; // Error: interface is reserved
// const private = 534;       // Error: private is reserved
```

**Benefits of Strict Mode:**

- Makes debugging easier
- Prevents accidental globals
- Eliminates silent errors
- Prohibits duplicate property names

### 17. Functions

```javascript
// Function declaration
function logger() {
  console.log("My name is Jonas");
}

// Calling/running/invoking function
logger();
logger();
logger();

// Function with parameters and return value
function fruitProcessor(apples, oranges) {
  const juice = `Juice with ${apples} apples and ${oranges} oranges.`;
  return juice;
}

const appleJuice = fruitProcessor(5, 0);
console.log(appleJuice);

const appleOrangeJuice = fruitProcessor(2, 4);
console.log(appleOrangeJuice);
```

### 18. Function Declarations vs Expressions

```javascript
// Function declaration - can be called before definition
function calcAge1(birthYear) {
  return 2037 - birthYear;
}
const age1 = calcAge1(1991);

// Function expression - cannot be called before definition
const calcAge2 = function (birthYear) {
  return 2037 - birthYear;
};
const age2 = calcAge2(1991);

console.log(age1, age2); // 46, 46
```

### 19. Arrow Functions

```javascript
// Arrow function (ES6)
const calcAge3 = (birthYear) => 2037 - birthYear;
const age3 = calcAge3(1991);
console.log(age3); // 46

// Arrow function with multiple parameters and statements
const yearsUntilRetirement = (birthYear, firstName) => {
  const age = 2037 - birthYear;
  const retirement = 65 - age;
  return `${firstName} retires in ${retirement} years`;
};

console.log(yearsUntilRetirement(1991, "Jonas"));
console.log(yearsUntilRetirement(1980, "Bob"));
```

### 20. Functions Calling Other Functions

```javascript
function cutFruitPieces(fruit) {
  return fruit * 4;
}

function fruitProcessor(apples, oranges) {
  const applePieces = cutFruitPieces(apples);
  const orangePieces = cutFruitPieces(oranges);

  const juice = `Juice with ${applePieces} piece of apple and ${orangePieces} pieces of orange.`;
  return juice;
}

console.log(fruitProcessor(2, 3));

// More complex example
const calcAge = function (birthYear) {
  return 2037 - birthYear;
};

const yearsUntilRetirement = function (birthYear, firstName) {
  const age = calcAge(birthYear);
  const retirement = 65 - age;

  if (retirement > 0) {
    console.log(`${firstName} retires in ${retirement} years`);
    return retirement;
  } else {
    console.log(`${firstName} has already retired 🎉`);
    return -1;
  }
};

console.log(yearsUntilRetirement(1991, "Jonas"));
console.log(yearsUntilRetirement(1950, "Mike"));
```

### 21. Introduction to Arrays

```javascript
// Creating arrays
const friend1 = "Michael";
const friend2 = "Steven";
const friend3 = "Peter";

const friends = ["Michael", "Steven", "Peter"];
console.log(friends);

// Alternative syntax
const y = new Array(1991, 1984, 2008, 2020);

// Accessing array elements
console.log(friends[0]); // 'Michael'
console.log(friends[2]); // 'Peter'
console.log(friends.length); // 3
console.log(friends[friends.length - 1]); // 'Peter'

// Mutating arrays (even const arrays)
friends[2] = "Jay";
console.log(friends); // ['Michael', 'Steven', 'Jay']

// Mixed data types in arrays
const firstName = "Jonas";
const jonas = [firstName, "Schmedtmann", 2037 - 1991, "teacher", friends];
console.log(jonas);

// Using functions with arrays
const calcAge = function (birthYear) {
  return 2037 - birthYear;
};

const years = [1990, 1967, 2002, 2010, 2018];
const age1 = calcAge(years[0]);
const age2 = calcAge(years[1]);
const age3 = calcAge(years[years.length - 1]);

const ages = [
  calcAge(years[0]),
  calcAge(years[1]),
  calcAge(years[years.length - 1]),
];
console.log(ages);
```

### 22. Basic Array Operations (Methods)

```javascript
const friends = ["Michael", "Steven", "Peter"];

// Add elements
const newLength = friends.push("Jay"); // Add to end
console.log(friends); // ['Michael', 'Steven', 'Peter', 'Jay']
console.log(newLength); // 4

friends.unshift("John"); // Add to beginning
console.log(friends); // ['John', 'Michael', 'Steven', 'Peter', 'Jay']

// Remove elements
friends.pop(); // Remove from end
const popped = friends.pop();
console.log(popped); // 'Peter'
console.log(friends); // ['John', 'Michael', 'Steven']

friends.shift(); // Remove from beginning
console.log(friends); // ['Michael', 'Steven']

// Find elements
console.log(friends.indexOf("Steven")); // 1
console.log(friends.indexOf("Bob")); // -1 (not found)

// Check if element exists (ES6)
friends.push(23);
console.log(friends.includes("Steven")); // true
console.log(friends.includes("Bob")); // false
console.log(friends.includes(23)); // true

// Practical use
if (friends.includes("Steven")) {
  console.log("You have a friend called Steven");
}
```

### 23. Introduction to Objects

```javascript
// Array (ordered list)
const jonasArray = [
  "Jonas",
  "Schmedtmann",
  2037 - 1991,
  "teacher",
  ["Michael", "Peter", "Steven"],
];

// Object (key-value pairs)
const jonas = {
  firstName: "Jonas",
  lastName: "Schmedtmann",
  age: 2037 - 1991,
  job: "teacher",
  friends: ["Michael", "Peter", "Steven"],
};
```

### 24. Dot vs Bracket Notation

```javascript
const jonas = {
  firstName: "Jonas",
  lastName: "Schmedtmann",
  age: 2037 - 1991,
  job: "teacher",
  friends: ["Michael", "Peter", "Steven"],
};

// Dot notation
console.log(jonas.lastName);

// Bracket notation
console.log(jonas["lastName"]);

// Dynamic property access
const nameKey = "Name";
console.log(jonas["first" + nameKey]); // firstName
console.log(jonas["last" + nameKey]); // lastName

// Getting user input
const interestedIn = prompt(
  "What do you want to know about Jonas? Choose between firstName, lastName, age, job, and friends"
);

if (jonas[interestedIn]) {
  console.log(jonas[interestedIn]);
} else {
  console.log(
    "Wrong request! Choose between firstName, lastName, age, job, and friends"
  );
}

// Adding properties
jonas.location = "Portugal";
jonas["twitter"] = "@jonasschmedtman";
console.log(jonas);

// Challenge: "Jonas has 3 friends, and his best friend is called Michael"
console.log(
  `${jonas.firstName} has ${jonas.friends.length} friends, and his best friend is called ${jonas.friends[0]}`
);
```

### 25. Object Methods

```javascript
const jonas = {
  firstName: "Jonas",
  lastName: "Schmedtmann",
  birthYear: 1991,
  job: "teacher",
  friends: ["Michael", "Peter", "Steven"],
  hasDriversLicense: true,

  // Method with 'this' keyword
  calcAge: function () {
    this.age = 2037 - this.birthYear;
    return this.age;
  },

  getSummary: function () {
    return `${this.firstName} is a ${this.calcAge()}-year old ${
      this.job
    }, and he has ${this.hasDriversLicense ? "a" : "no"} driver's license.`;
  },
};

console.log(jonas.calcAge()); // 46
console.log(jonas.age); // 46 (stored property)

// Challenge: "Jonas is a 46-year old teacher, and he has a driver's license"
console.log(jonas.getSummary());
```

### 26. Iteration: The for Loop

```javascript
// Manual repetition (inefficient)
// console.log('Lifting weights repetition 1 🏋️‍♀️');
// console.log('Lifting weights repetition 2 🏋️‍♀️');
// ... (repeated 10 times)

// for loop keeps running while condition is TRUE
for (let rep = 1; rep <= 10; rep++) {
  console.log(`Lifting weights repetition ${rep} 🏋️‍♀️`);
}
```

### 27. Looping Arrays, Breaking and Continuing

```javascript
const jonas = [
  "Jonas",
  "Schmedtmann",
  2037 - 1991,
  "teacher",
  ["Michael", "Peter", "Steven"],
  true,
];
const types = [];

for (let i = 0; i < jonas.length; i++) {
  // Reading from jonas array
  console.log(jonas[i], typeof jonas[i]);

  // Filling types array
  types.push(typeof jonas[i]);
}
console.log(types);

// Example with years
const years = [1991, 2007, 1969, 2020];
const ages = [];

for (let i = 0; i < years.length; i++) {
  ages.push(2037 - years[i]);
}
console.log(ages);

// continue and break
console.log("--- ONLY STRINGS ---");
for (let i = 0; i < jonas.length; i++) {
  if (typeof jonas[i] !== "string") continue;
  console.log(jonas[i], typeof jonas[i]);
}

console.log("--- BREAK WITH NUMBER ---");
for (let i = 0; i < jonas.length; i++) {
  if (typeof jonas[i] === "number") break;
  console.log(jonas[i], typeof jonas[i]);
}
```

### 28. Looping Backwards and Loops in Loops

```javascript
const jonas = [
  "Jonas",
  "Schmedtmann",
  2037 - 1991,
  "teacher",
  ["Michael", "Peter", "Steven"],
  true,
];

// Looping backwards
for (let i = jonas.length - 1; i >= 0; i--) {
  console.log(i, jonas[i]);
}

// Loop inside a loop
for (let exercise = 1; exercise < 4; exercise++) {
  console.log(`-------- Starting exercise ${exercise}`);

  for (let rep = 1; rep < 6; rep++) {
    console.log(`Exercise ${exercise}: Lifting weight repetition ${rep} 🏋️‍♀️`);
  }
}
```

### 29. The while Loop

```javascript
// for loop
for (let rep = 1; rep <= 10; rep++) {
  console.log(`Lifting weights repetition ${rep} 🏋️‍♀️`);
}

// while loop
let rep = 1;
while (rep <= 10) {
  console.log(`WHILE: Lifting weights repetition ${rep} 🏋️‍♀️`);
  rep++;
}

// while loop with random condition
let dice = Math.trunc(Math.random() * 6) + 1;

while (dice !== 6) {
  console.log(`You rolled a ${dice}`);
  dice = Math.trunc(Math.random() * 6) + 1;
  if (dice === 6) console.log("Loop is about to end...");
}
```

---

## 30. Coding Challenges

### Challenge #1: BMI Calculator

**Problem:** Mark and John are trying to compare their BMI (Body Mass Index), which is calculated using the formula: BMI = mass / height² = mass / (height \* height). (mass in kg and height in meter).

**Tasks:**

1. Store Mark's and John's mass and height in variables
2. Calculate both their BMIs using the formula
3. Create a boolean variable 'markHigherBMI' containing information about whether Mark has a higher BMI than John.

```javascript
// Test Data 1: Mark weighs 78 kg and is 1.69 m tall. John weighs 92 kg and is 1.95 m tall.
const massMark = 78;
const heightMark = 1.69;
const massJohn = 92;
const heightJohn = 1.95;

const BMIMark = massMark / heightMark ** 2;
const BMIJohn = massJohn / (heightJohn * heightJohn);
const markHigherBMI = BMIMark > BMIJohn;

console.log(BMIMark, BMIJohn, markHigherBMI);
```

### Challenge #2: BMI Calculator with Output

**Problem:** Use the BMI example from Challenge #1, and improve it with nice output messages.

```javascript
const massMark = 78;
const heightMark = 1.69;
const massJohn = 92;
const heightJohn = 1.95;

const BMIMark = massMark / heightMark ** 2;
const BMIJohn = massJohn / (heightJohn * heightJohn);

if (BMIMark > BMIJohn) {
  console.log(`Mark's BMI (${BMIMark}) is higher than John's (${BMIJohn})!`);
} else {
  console.log(`John's BMI (${BMIJohn}) is higher than Mark's (${BMIMark})!`);
}
```

### Challenge #3: Gymnastics Competition

**Problem:** Two gymnastics teams, Dolphins and Koalas, compete against each other 3 times. The winner with the highest average score wins a trophy!

```javascript
// Test Data: Dolphins score 97, 112 and 80. Koalas score 109, 95 and 50
const scoreDolphins = (97 + 112 + 80) / 3;
const scoreKoalas = (109 + 95 + 50) / 3;

if (scoreDolphins > scoreKoalas && scoreDolphins >= 100) {
  console.log("Dolphins win the trophy 🏆");
} else if (scoreKoalas > scoreDolphins && scoreKoalas >= 100) {
  console.log("Koalas win the trophy 🏆");
} else if (
  scoreDolphins === scoreKoalas &&
  scoreDolphins >= 100 &&
  scoreKoalas >= 100
) {
  console.log("Both win the trophy!");
} else {
  console.log("No one wins the trophy 😭");
}
```

### Challenge #4: Tip Calculator

**Problem:** Steven wants to build a simple tip calculator. Tip 15% if the bill value is between 50 and 300, otherwise tip 20%.

```javascript
const bill = 275;
const tip = bill <= 300 && bill >= 50 ? bill * 0.15 : bill * 0.2;
console.log(`The bill was ${bill}, the tip was ${bill + tip}`);
```

### Challenge #5: Gymnastics Teams with Functions

**Problem:** Back to the two gymnastics teams, the Dolphins and the Koalas! There is a new gymnastics discipline, which works differently. A team ONLY wins if it has at least DOUBLE the average score of the other team.

```javascript
const calcAverage = (a, b, c) => (a + b + c) / 3;

const checkWinner = function (avgDolphins, avgKoalas) {
  if (avgDolphins >= 2 * avgKoalas) {
    console.log(`Dolphins win 🏆 (${avgDolphins} vs. ${avgKoalas})`);
  } else if (avgKoalas >= 2 * avgDolphins) {
    console.log(`Koalas win 🏆 (${avgKoalas} vs. ${avgDolphins})`);
  } else {
    console.log("No team wins...");
  }
};

// Test 1: Dolphins score 44, 23 and 71. Koalas score 65, 54 and 49
let scoreDolphins = calcAverage(44, 23, 71);
let scoreKoalas = calcAverage(65, 54, 49);
checkWinner(scoreDolphins, scoreKoalas);

// Test 2: Dolphins score 85, 54 and 41. Koalas score 23, 34 and 27
scoreDolphins = calcAverage(85, 54, 41);
scoreKoalas = calcAverage(23, 34, 27);
checkWinner(scoreDolphins, scoreKoalas);
```

### Challenge #6: Enhanced Tip Calculator with Arrays

**Problem:** Steven wants to improve his tip calculator using arrays and loops.

```javascript
const calcTip = function (bill) {
  return bill >= 50 && bill <= 300 ? bill * 0.15 : bill * 0.2;
};

const bills = [125, 555, 44];
const tips = [calcTip(bills[0]), calcTip(bills[1]), calcTip(bills[2])];
const totals = [bills[0] + tips[0], bills[1] + tips[1], bills[2] + tips[2]];

console.log(bills, tips, totals);
```

### Challenge #7: BMI Calculator with Objects

**Problem:** Let's go back to Mark and John comparing their BMIs! This time, use objects to implement the calculations!

```javascript
const mark = {
  fullName: "Mark Miller",
  mass: 78,
  height: 1.69,
  calcBMI: function () {
    this.bmi = this.mass / this.height ** 2;
    return this.bmi;
  },
};

const john = {
  fullName: "John Smith",
  mass: 92,
  height: 1.95,
  calcBMI: function () {
    this.bmi = this.mass / this.height ** 2;
    return this.bmi;
  },
};

mark.calcBMI();
john.calcBMI();

if (mark.bmi > john.bmi) {
  console.log(
    `${mark.fullName}'s BMI (${mark.bmi}) is higher than ${john.fullName}'s BMI (${john.bmi})`
  );
} else if (john.bmi > mark.bmi) {
  console.log(
    `${john.fullName}'s BMI (${john.bmi}) is higher than ${mark.fullName}'s BMI (${mark.bmi})`
  );
}
```

### Challenge #8: Advanced Tip Calculator with Loops

**Problem:** Let's improve Steven's tip calculator even more, this time using loops!

```javascript
const calcTip = function (bill) {
  return bill >= 50 && bill <= 300 ? bill * 0.15 : bill * 0.2;
};

const bills = [22, 295, 176, 440, 37, 105, 10, 1100, 86, 52];
const tips = [];
const totals = [];

for (let i = 0; i < bills.length; i++) {
  const tip = calcTip(bills[i]);
  tips.push(tip);
  totals.push(tip + bills[i]);
}
console.log(bills, tips, totals);

// BONUS: Calculate average function
const calcAverage = function (arr) {
  let sum = 0;
  for (let i = 0; i < arr.length; i++) {
    sum += arr[i];
  }
  return sum / arr.length;
};

console.log(calcAverage(totals)); // Average of all totals
console.log(calcAverage(tips)); // Average of all tips
```

---

## Embedding JavaScript in HTML

### 1. Inline JavaScript

- You can write JavaScript directly within HTML elements using event attributes:

```html
<button onclick="alert('Hello!')">Click me</button>
<body onload="console.log('Page loaded')"></body>
```

### 2. Internal JavaScript with `<script>` tags

- Place JavaScript code directly in the HTML document between `<script>`and `</script>` tags:

```html
<script>
  function myFunction() {
    console.log("Hello from internal script");
  }
  myFunction();
</script>
```

### 3. External JavaScript files

- Link to separate .js files using the src attribute:

```html
<script src="script.js"></script>
```

---

## NoScript Tag

Provides fallback content when JavaScript is disabled.

```html
<!DOCTYPE html>
<html>
  <body>
    <script>
      document.write("JavaScript is enabled!");
    </script>

    <noscript>
      <p>
        JavaScript is disabled in your browser. Please enable it for full
        functionality.
      </p>
    </noscript>
  </body>
</html>
```

---

## Interacting With The Browser

### Window Object

```javascript
// Window properties
console.log(window.innerWidth); // Browser window width
console.log(window.innerHeight); // Browser window height
console.log(window.location.href); // Current URL

// Window methods
window.alert("This is an alert!");
let userResponse = window.confirm("Do you want to continue?");
let userInput = window.prompt("Enter your name:");

// Navigation
// window.open("https://example.com", "_blank");
// window.close(); // Close current window
// window.location.href = "https://example.com"; // Navigate to URL
```

### Example

```html
<html>
  <head>
    <title>Window Object</title>
  </head>
  <body>
    <h1>Window Object Example</h1>
    <button id="openWindow">Open New Window</button>
    <button id="changeLocation">Change Location</button>
    <div style="height: 200vh"></div>
    <script>
      console.log(
        "Window inner size: " + window.innerWidth + "x" + window.innerHeight
      );

      // Handling button clicks
      document.getElementById("openWindow").addEventListener("click", () => {
        window.open("https://www.apple.com");
      });

      document
        .getElementById("changeLocation")
        .addEventListener("click", () => {
          window.location.href = "https://www.apple.com";
        });

      // Handling window events
      window.addEventListener("resize", () => {
        console.log(
          "Window resized to: " + window.innerWidth + "x" + window.innerHeight
        );
      });

      window.addEventListener("scroll", () => {
        console.log("Window scrolled. Scroll position: " + window.scrollY);
      });

      // Storing a string
      localStorage.setItem("username", "John Doe");

      //   window.localStorage.removeItem("username");
      // Storing an object
      const user = {
        name: "John Doe",
        age: 30,
        email: "johndoe@example.com",
      };
      localStorage.setItem("user", JSON.stringify(user));

      // Retrieving a string
      const username = localStorage.getItem("username");
      console.log(username); // Output: John Doe

      // Retrieving an object
      const userRetrived = JSON.parse(localStorage.getItem("user"));
      console.log(user); // Output: { name: 'John Doe', age: 30, email: 'johndoe@example.com' }
    </script>
  </body>
</html>
```

### Popup Example

- A dialog box in JavaScript is a pop-up window that allows you to interact with the user. It's commonly used for:
  - Showing messages
  - Asking for confirmation
  - Taking input
- These are built-in methods of the window object and work in all browsers.

#### **Types:**

- The alert() method displays a simple message to the user in an alert box.
- The confirm() method displays a confirmation dialog box with two buttons: OK and Cancel.
- The prompt() method displays a dialog box with a text input field where the user can enter data.
  <br>
  <br>

```html
<html>
  <head>
    <title>Pop Up</title>
  </head>
  <body>
    <h1>Project 1</h1>
    <button onclick="deleteProject()">Delete Project</button>
    <script>
      function deleteProject() {
        const isConfirmed = confirm("Are you sure to delete?");
        if (isConfirmed) {
          const projectName = prompt("Type Project Name to Verify Deletion");
          if (projectName == "Project 1") {
            document.body.removeChild(document.getElementsByTagName("h1")[0]);
          } else {
            alert("Project Name did not match");
          }
        } else {
          alert("Deleteion Cancelled");
        }
      }
    </script>
  </body>
</html>
```

---

### Screen Object

```javascript
console.log(screen.width); // Screen width
console.log(screen.height); // Screen height
console.log(screen.availWidth); // Available screen width
console.log(screen.availHeight); // Available screen height
console.log(screen.colorDepth); // Color depth
```

### Navigator Object

```javascript
console.log(navigator.userAgent); // Browser information
console.log(navigator.platform); // Operating system
console.log(navigator.language); // Browser language
console.log(navigator.onLine); // Online status
console.log(navigator.cookieEnabled); // Cookie support
```

---

## Windows & Frames

### Working with Windows

```javascript
// Open new window
let newWindow = window.open("", "myWindow", "width=400,height=300");
newWindow.document.write("<h1>New Window Content</h1>");

// Focus and blur
// newWindow.focus();
// newWindow.blur();

// Close window
// newWindow.close();
```

### Working with Frames

```html
<!-- HTML with frames -->
<iframe id="myFrame" src="about:blank" width="300" height="200"></iframe>

<script>
  // Access frame content
  let frame = document.getElementById("myFrame");
  frame.onload = function () {
    console.log("Frame loaded");
  };

  // Write to frame
  frame.src = "data:text/html,<h1>Frame Content</h1>";
</script>
```

---

## Document Object Model (DOM)

#### What is the DOM?

- The Document Object Model (DOM) is a programming interface for web documents. It represents the structure of an HTML or XML document as a tree of nodes.

- Each element in the HTML (like `<html>`, `<body>`, `<ul>`, `<li>`, etc.) becomes a node in this tree. These nodes are related to each other as parents, children, siblings, etc.

#### Structure of the DOM

![Structure of the DOM](/images/dom1.gif "Structure of the DOM")

**Root Node:**

- `<html>` is the root of the DOM tree.
- It contains all other elements.

**Nodes:**

- All tags like `<head>`, `<body>`, `<nav>`, etc., are nodes.
- Nodes can be elements, text, attributes, or comments.

**Parent-Child Relationship:**

- For example, `<ul>` is the parent of its `<li>` children.
  `<body>` is the parent of `<nav>` and `<section>`.

**Leaves:**

- A leaf is a node without children (e.g., `<img>` or individual `<li>`'s).

**Branches:**

- Intermediate nodes with children (e.g., `<nav>`, `<ul>`).

#### Structure of the DOM

```html
<html>
  <head>
    <title>My Page</title>
  </head>
  <body>
    <h1>Welcome</h1>
    <p>This is some text.</p>
  </body>
</html>
```

#### Why is the DOM Important?

**Dynamic Content:**

- JavaScript can access and modify the DOM to update web pages without reloading, enabling dynamic content.

**Interactivity:**

- DOM lets scripts respond to user interactions (clicks, keypresses, etc.).

**Structure and Organization:**

- It provides a hierarchical representation of content, making it easier for developers and browsers to work with.

**Foundation for Frameworks:**

- Modern JavaScript frameworks like React, Angular, and Vue.js are built upon the DOM, providing higher-level abstractions and tools to efficiently manage and manipulate the DOM for complex applications.

#### Example: JavaScript DOM Manipulation

```js
const newLi = document.createElement("li");
const textNode = document.createTextNode("New Item");
newLi.appendChild(textNode);
document.querySelector("ul").appendChild(newLi);
// ---------------
// ------OR-------
// ---------------
const newLi = document.createElement("li");
newLi.textContent = "New Item"; // newLi.innerText also works (behind the scenes, browser creates text node)
document.querySelector("ul").appendChild(newLi);

// See topics below for more examples
```

### Selecting Elements

```javascript
// Select by ID
let elementById = document.getElementById("myId");

// Select by class name
// returns HTMLCollection
// does not have forEach builtin
let elementsByClass = document.getElementsByClassName("myClass");

// Select by tag name
// returns HTMLCollection
let elementsByTag = document.getElementsByTagName("p");

// Query selector (CSS selector)
let firstMatch = document.querySelector(".myClass");
// returns NodeList
// has forEach
let allMatches = document.querySelectorAll(".myClass");
```

```html
<html>
  <head>
    <title>Selecting Elements</title>
  </head>
  <body>
    <h1 id="myId">Hello</h1>
    <h1 class="myClass">Hi</h1>
    <h1 class="myClass">Hi</h1>
    <p>Hello</p>
    <p>Hello</p>
    <script>
      let elementById = document.getElementById("myId");
      let elementsByClass = document.getElementsByClassName("myClass");
      let elementsByTag = document.getElementsByTagName("p");
      let firstMatch = document.querySelector(".myClass");
      let allMatches = document.querySelectorAll(".myClass");

      window.onload = () => {
        elementById.style.color = "green";

        // [...elementsByClass].forEach()
        for (let element of elementsByClass) {
          element.style.background = "yellow";
        }

        for (let element of elementsByTag) {
          element.style.background = "pink";
        }

        firstMatch.style.color = "red";

        allMatches.forEach((element) => {
          element.style.fontStyle = "italic";
        });
      };
    </script>
  </body>
</html>
```

### Manipulating Elements

```javascript
// Change content
document.getElementById("demo").innerHTML = "<b>New HTML content</b>";
document.getElementById("demo").textContent = "New text content";

// Change attributes
let image = document.getElementById("myImage");
image.src = "new-image.jpg";
image.alt = "New image description";

// Change styles
let element = document.getElementById("myElement");
element.style.color = "red";
element.style.fontSize = "20px";
element.style.display = "none";

// Add/remove classes
element.classList.add("newClass");
element.classList.remove("oldClass");
element.classList.toggle("toggleClass");
```

### Creating and Removing Elements

```javascript
// Create new element
let newParagraph = document.createElement("p");
newParagraph.textContent = "This is a new paragraph";
newParagraph.className = "highlight";

// Append to document
document.body.appendChild(newParagraph);

// Insert before specific element
let existingElement = document.getElementById("existing");
document.body.insertBefore(newParagraph, existingElement);

// Remove element
let elementToRemove = document.getElementById("remove-me");
elementToRemove.parentNode.removeChild(elementToRemove);

// Modern remove method
// elementToRemove.remove();
```

---

---

---

## Event Handling

A **JavaScript Event** is an action or occurrence that happens in the browser, like:

- A user clicks a button
- A web page loads
- A form is submitted
- A key is pressed

- You can write **JavaScript code to "listen" and "respond"** to these events.

## Common Event Types

```javascript
// Click Event
element.addEventListener("click", function () {
  /* code */
});

// Keyboard Events
element.addEventListener("keyup", function (event) {
  /* code */
});
element.addEventListener("keydown", function (event) {
  /* code */
});

// Mouse Events
element.addEventListener("mouseenter", function () {
  /* code */
});
element.addEventListener("mouseleave", function () {
  /* code */
});

// Form Events
form.addEventListener("submit", function (event) {
  /* code */
});
input.addEventListener("change", function () {
  /* code */
});
```

### Inline Event Handlers

```html
<button onclick="alert('Button clicked!')">Click Me</button>
<input type="text" onchange="console.log('Input changed')" />
```

### Event Listeners

```javascript
// Add event listener
document.getElementById("myButton").addEventListener("click", function () {
  alert("Button was clicked!");
});

// Event listener with named function
function handleClick(event) {
  console.log("Button clicked!");
  console.log("Event type:", event.type);
  console.log("Target element:", event.target);
}

document.getElementById("myButton").addEventListener("click", handleClick);

// Multiple event types
let input = document.getElementById("myInput");
input.addEventListener("focus", function () {
  console.log("Input focused");
});
input.addEventListener("blur", function () {
  console.log("Input lost focus");
});
input.addEventListener("keyup", function (e) {
  console.log("Key pressed:", e.key);
});
```

### Event Object

```javascript
document.addEventListener("click", function (event) {
  console.log("Click coordinates:", event.clientX, event.clientY);
  console.log("Target element:", event.target.tagName);

  // Prevent default behavior
  if (event.target.tagName === "A") {
    event.preventDefault();
    console.log("Link click prevented");
  }
});
```

---

## Forms

### Form Validation and Handling

```html
<form id="myForm">
  <input type="text" id="username" placeholder="Username" required />
  <input type="email" id="email" placeholder="Email" required />
  <input type="password" id="password" placeholder="Password" required />
  <button type="submit">Submit</button>
</form>

<script>
  document
    .getElementById("myForm")
    .addEventListener("submit", function (event) {
      event.preventDefault(); // Prevent form submission

      // Get form values
      let username = document.getElementById("username").value;
      let email = document.getElementById("email").value;
      let password = document.getElementById("password").value;

      // Validation
      if (username.length < 3) {
        alert("Username must be at least 3 characters");
        return;
      }

      if (!email.includes("@")) {
        alert("Please enter a valid email");
        return;
      }

      if (password.length < 6) {
        alert("Password must be at least 6 characters");
        return;
      }

      console.log("Form data:", { username, email, password });
      alert("Form submitted successfully!");
    });
</script>
```

### Form Element Access

```javascript
// Access form elements
let form = document.forms["myForm"]; // or document.getElementById("myForm")
let username = form.elements["username"];
let email = form.elements["email"];

// Get all form data
function getFormData(form) {
  let formData = {};
  for (let i = 0; i < form.elements.length; i++) {
    let element = form.elements[i];
    if (element.name) {
      formData[element.name] = element.value;
    }
  }
  return formData;
}
```

---

## Cookies

### Creating and Reading Cookies

```javascript
// Set cookie
function setCookie(name, value, days) {
  let expires = "";
  if (days) {
    let date = new Date();
    date.setTime(date.getTime() + days * 24 * 60 * 60 * 1000);
    expires = "; expires=" + date.toUTCString();
  }
  document.cookie = name + "=" + value + expires + "; path=/";
}

// Get cookie
function getCookie(name) {
  let nameEQ = name + "=";
  let cookies = document.cookie.split(";");
  for (let i = 0; i < cookies.length; i++) {
    let cookie = cookies[i];
    while (cookie.charAt(0) === " ") {
      cookie = cookie.substring(1, cookie.length);
    }
    if (cookie.indexOf(nameEQ) === 0) {
      return cookie.substring(nameEQ.length, cookie.length);
    }
  }
  return null;
}

// Delete cookie
function deleteCookie(name) {
  document.cookie = name + "=; expires=Thu, 01 Jan 1970 00:00:00 UTC; path=/;";
}

// Example usage
setCookie("username", "john_doe", 7); // Set for 7 days
console.log(getCookie("username")); // john_doe
deleteCookie("username");
```

### Practical Cookie Example

```javascript
// Welcome message using cookies
function showWelcomeMessage() {
  let lastVisit = getCookie("lastVisit");
  let now = new Date();

  if (lastVisit) {
    alert("Welcome back! Your last visit was: " + lastVisit);
  } else {
    alert("Welcome to our website!");
  }

  setCookie("lastVisit", now.toString(), 30);
}

// Call on page load
window.onload = showWelcomeMessage;
```

---

## Handling Regular Expressions

### Creating Regular Expressions

```javascript
// Literal notation
let regex1 = /pattern/flags;

// Constructor notation
let regex2 = new RegExp("pattern", "flags");

// Common flags:
// g - global (find all matches)
// i - case insensitive
// m - multiline
```

### Pattern Matching

```javascript
let text = "The quick brown fox jumps over the lazy dog";

// Test if pattern exists
let hasQuick = /quick/i.test(text);
console.log(hasQuick); // true

// Find matches
let matches = text.match(/the/gi);
console.log(matches); // ["The", "the"]

// Replace with regex
let newText = text.replace(/the/gi, "a");
console.log(newText); // "a quick brown fox jumps over a lazy dog"

// Split with regex
let words = text.split(/\s+/);
console.log(words); // Array of words
```

### Common Patterns

```javascript
// Email validation
function validateEmail(email) {
  let emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
  return emailRegex.test(email);
}

// Phone number validation (US format)
function validatePhone(phone) {
  let phoneRegex = /^\(\d{3}\)\s\d{3}-\d{4}$/;
  return phoneRegex.test(phone);
}

// Password strength (at least 8 chars, 1 uppercase, 1 lowercase, 1 number)
function validatePassword(password) {
  let passwordRegex = /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[a-zA-Z\d]{8,}$/;
  return passwordRegex.test(password);
}

// Extract numbers from string
function extractNumbers(text) {
  return text.match(/\d+/g) || [];
}

// Examples
console.log(validateEmail("user@example.com")); // true
console.log(validatePhone("(123) 456-7890")); // true
console.log(validatePassword("MyPass123")); // true
console.log(extractNumbers("I have 5 apples and 3 oranges")); // ["5", "3"]
```

---

## Client Side Validations

### Complete Form Validation Example

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Form Validation</title>
    <style>
      .error {
        color: red;
        font-size: 12px;
      }
      .valid {
        border: 2px solid green;
      }
      .invalid {
        border: 2px solid red;
      }
    </style>
  </head>
  <body>
    <form id="registrationForm">
      <div>
        <label>Full Name:</label>
        <input type="text" id="fullName" required />
        <span class="error" id="nameError"></span>
      </div>

      <div>
        <label>Email:</label>
        <input type="email" id="email" required />
        <span class="error" id="emailError"></span>
      </div>

      <div>
        <label>Phone:</label>
        <input type="tel" id="phone" required />
        <span class="error" id="phoneError"></span>
      </div>

      <div>
        <label>Age:</label>
        <input type="number" id="age" min="18" max="100" required />
        <span class="error" id="ageError"></span>
      </div>

      <div>
        <label>Password:</label>
        <input type="password" id="password" required />
        <span class="error" id="passwordError"></span>
      </div>

      <div>
        <label>Confirm Password:</label>
        <input type="password" id="confirmPassword" required />
        <span class="error" id="confirmPasswordError"></span>
      </div>

      <button type="submit">Register</button>
    </form>

    <script>
      // Validation functions
      function validateName(name) {
        return name.length >= 2 && /^[a-zA-Z\s]+$/.test(name);
      }

      function validateEmail(email) {
        return /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
      }

      function validatePhone(phone) {
        return /^\d{10}$/.test(phone.replace(/\D/g, ""));
      }

      function validateAge(age) {
        return age >= 18 && age <= 100;
      }

      function validatePassword(password) {
        return (
          password.length >= 8 &&
          /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)/.test(password)
        );
      }

      // Real-time validation
      document.getElementById("fullName").addEventListener("blur", function () {
        let name = this.value;
        let errorElement = document.getElementById("nameError");

        if (!validateName(name)) {
          this.className = "invalid";
          errorElement.textContent =
            "Name must be at least 2 characters and contain only letters";
        } else {
          this.className = "valid";
          errorElement.textContent = "";
        }
      });

      document.getElementById("email").addEventListener("blur", function () {
        let email = this.value;
        let errorElement = document.getElementById("emailError");

        if (!validateEmail(email)) {
          this.className = "invalid";
          errorElement.textContent = "Please enter a valid email address";
        } else {
          this.className = "valid";
          errorElement.textContent = "";
        }
      });

      document.getElementById("phone").addEventListener("blur", function () {
        let phone = this.value;
        let errorElement = document.getElementById("phoneError");

        if (!validatePhone(phone)) {
          this.className = "invalid";
          errorElement.textContent =
            "Please enter a valid 10-digit phone number";
        } else {
          this.className = "valid";
          errorElement.textContent = "";
        }
      });

      document.getElementById("age").addEventListener("blur", function () {
        let age = parseInt(this.value);
        let errorElement = document.getElementById("ageError");

        if (!validateAge(age)) {
          this.className = "invalid";
          errorElement.textContent = "Age must be between 18 and 100";
        } else {
          this.className = "valid";
          errorElement.textContent = "";
        }
      });

      document.getElementById("password").addEventListener("blur", function () {
        let password = this.value;
        let errorElement = document.getElementById("passwordError");

        if (!validatePassword(password)) {
          this.className = "invalid";
          errorElement.textContent =
            "Password must be 8+ characters with uppercase, lowercase, and number";
        } else {
          this.className = "valid";
          errorElement.textContent = "";
        }
      });

      document
        .getElementById("confirmPassword")
        .addEventListener("blur", function () {
          let password = document.getElementById("password").value;
          let confirmPassword = this.value;
          let errorElement = document.getElementById("confirmPasswordError");

          if (password !== confirmPassword) {
            this.className = "invalid";
            errorElement.textContent = "Passwords do not match";
          } else {
            this.className = "valid";
            errorElement.textContent = "";
          }
        });

      // Form submission validation
      document
        .getElementById("registrationForm")
        .addEventListener("submit", function (event) {
          event.preventDefault();

          let isValid = true;
          let formData = {};

          // Collect and validate all data
          let fullName = document.getElementById("fullName").value;
          let email = document.getElementById("email").value;
          let phone = document.getElementById("phone").value;
          let age = parseInt(document.getElementById("age").value);
          let password = document.getElementById("password").value;
          let confirmPassword =
            document.getElementById("confirmPassword").value;

          // Validate all fields
          if (!validateName(fullName)) {
            isValid = false;
            alert("Please enter a valid name");
            return;
          }

          if (!validateEmail(email)) {
            isValid = false;
            alert("Please enter a valid email");
            return;
          }

          if (!validatePhone(phone)) {
            isValid = false;
            alert("Please enter a valid phone number");
            return;
          }

          if (!validateAge(age)) {
            isValid = false;
            alert("Please enter a valid age (18-100)");
            return;
          }

          if (!validatePassword(password)) {
            isValid = false;
            alert("Please enter a valid password");
            return;
          }

          if (password !== confirmPassword) {
            isValid = false;
            alert("Passwords do not match");
            return;
          }

          if (isValid) {
            formData = { fullName, email, phone, age, password };
            console.log("Form submitted successfully:", formData);
            alert("Registration successful!");

            // Here you would typically send data to server
            // fetch('/register', {
            //     method: 'POST',
            //     headers: {'Content-Type': 'application/json'},
            //     body: JSON.stringify(formData)
            // });
          }
        });
    </script>
  </body>
</html>
```

---

## Projects

### Modal

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="style.css" />
    <title>Modal window</title>
  </head>
  <body>
    <button class="show-modal">Show modal 1</button>
    <button class="show-modal">Show modal 2</button>
    <button class="show-modal">Show modal 3</button>

    <div class="modal hidden">
      <button class="close-modal">&times;</button>
      <h1>I'm a modal window 😍</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
        velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt
        mollit anim id est laborum.
      </p>
    </div>
    <div class="overlay hidden"></div>

    <script src="script.js"></script>
  </body>
</html>
```

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  font-size: 62.5%;
  box-sizing: border-box;
}

body {
  font-family: sans-serif;
  color: #333;
  line-height: 1.5;
  height: 100vh;
  position: relative;
  display: flex;
  align-items: flex-start;
  justify-content: center;
  background: linear-gradient(to top left, #28b487, #7dd56f);
}

.show-modal {
  font-size: 2rem;
  font-weight: 600;
  padding: 1.75rem 3.5rem;
  margin: 5rem 2rem;
  border: none;
  background-color: #fff;
  color: #444;
  border-radius: 10rem;
  cursor: pointer;
}

.close-modal {
  position: absolute;
  top: 1.2rem;
  right: 2rem;
  font-size: 5rem;
  color: #333;
  cursor: pointer;
  border: none;
  background: none;
}

h1 {
  font-size: 2.5rem;
  margin-bottom: 2rem;
}

p {
  font-size: 1.8rem;
}

/* -------------------------- */
/* CLASSES TO MAKE MODAL WORK */
.hidden {
  display: none;
}

.modal {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 70%;

  background-color: white;
  padding: 6rem;
  border-radius: 5px;
  box-shadow: 0 3rem 5rem rgba(0, 0, 0, 0.3);
  z-index: 10;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(3px);
  z-index: 5;
}
```

```js
"use strict";

const modal = document.querySelector(".modal");
const overlay = document.querySelector(".overlay");
const btnCloseModal = document.querySelector(".close-modal");
const btnsOpenModal = document.querySelectorAll(".show-modal");

const openModal = function () {
  modal.classList.remove("hidden");
  overlay.classList.remove("hidden");
};

const closeModal = function () {
  modal.classList.add("hidden");
  overlay.classList.add("hidden");
};

for (let i = 0; i < btnsOpenModal.length; i++)
  btnsOpenModal[i].addEventListener("click", openModal);

btnCloseModal.addEventListener("click", closeModal);
overlay.addEventListener("click", closeModal);

document.addEventListener("keydown", function (e) {
  // console.log(e.key);

  if (e.key === "Escape" && !modal.classList.contains("hidden")) {
    closeModal();
  }
});
```

### Write HTML and JavaScript code to create a following calculator for performing basic arithmetic operations.

![Calculator](/images/calculator.png "Calculator")

```html
<html>
  <head>
    <title>Basic Calculator</title>
    <style>
      * {
        box-sizing: border-box;
      }
      body {
        align-content: center;
      }
      .calculator {
        border: 5px solid #aea3b0;
        padding: 10px;
        width: 350px;
        margin: 0 auto;
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 5px;
        background: #8e7f8e;
      }
      input {
        height: 40px;
        font-size: 20px;
        grid-column: 1 / 4;
        background: #aea3b0;
        outline: none;
        border: none;
        color: #333;
      }
      button {
        height: 40px;
        cursor: pointer;
        background: #aea3b0;
        border: none;
        border-radius: 2px;
        color: #333;
      }
    </style>
  </head>
  <body>
    <div class="calculator">
      <input type="text" id="display" readonly />
      <button onclick="clearDisplay()">C</button>
      <button onclick="appendNumber('1')">1</button>
      <button onclick="appendNumber('2')">2</button>
      <button onclick="appendNumber('3')">3</button>
      <button onclick="appendOperator('+')">+</button>

      <button onclick="appendNumber('4')">4</button>
      <button onclick="appendNumber('5')">5</button>
      <button onclick="appendNumber('6')">6</button>
      <button onclick="appendOperator('-')">-</button>

      <button onclick="appendNumber('7')">7</button>
      <button onclick="appendNumber('8')">8</button>
      <button onclick="appendNumber('9')">9</button>
      <button onclick="appendNumber('10')">10</button>

      <button onclick="appendNumber('0')">0</button>
      <button onclick="appendOperator('*')">*</button>
      <button onclick="appendOperator('/')">/</button>
      <button onclick="calculate()">=</button>
    </div>

    <script>
      function appendNumber(num) {
        document.getElementById("display").value += num;
      }

      function appendOperator(op) {
        const display = document.getElementById("display");
        const lastChar = display.value.slice(-1);
        if ("+-*/".includes(lastChar)) return; // prevent double operators
        display.value += op;
      }

      function clearDisplay() {
        document.getElementById("display").value = "";
      }

      function calculate() {
        const display = document.getElementById("display");
        try {
          display.value = eval(display.value);
        } catch {
          display.value = "Error";
        }
      }
    </script>
  </body>
</html>
```

---

### Guess My Number

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="style.css" />
    <title>Guess My Number!</title>
  </head>
  <body>
    <header>
      <h1>Guess My Number!</h1>
      <p class="between">(Between 1 and 20)</p>
      <button class="btn again">Again!</button>
      <div class="number">?</div>
    </header>
    <main>
      <section class="left">
        <input type="number" class="guess" />
        <button class="btn check">Check!</button>
      </section>
      <section class="right">
        <p class="message">Start guessing...</p>
        <p class="label-score">💯 Score: <span class="score">20</span></p>
        <p class="label-highscore">
          🥇 Highscore: <span class="highscore">0</span>
        </p>
      </section>
    </main>
    <script src="script.js"></script>
  </body>
</html>
```

```css
@import url("https://fonts.googleapis.com/css?family=Press+Start+2P&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  font-size: 62.5%;
  box-sizing: border-box;
}

body {
  font-family: "Press Start 2P", sans-serif;
  color: #eee;
  background-color: #222;
  /* background-color: #60b347; */
}

/* LAYOUT */
header {
  position: relative;
  height: 35vh;
  border-bottom: 7px solid #eee;
}

main {
  height: 65vh;
  color: #eee;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.left {
  width: 52rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.right {
  width: 52rem;
  font-size: 2rem;
}

/* ELEMENTS STYLE */
h1 {
  font-size: 4rem;
  text-align: center;
  position: absolute;
  width: 100%;
  top: 52%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.number {
  background: #eee;
  color: #333;
  font-size: 6rem;
  width: 15rem;
  padding: 3rem 0rem;
  text-align: center;
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translate(-50%, 50%);
}

.between {
  font-size: 1.4rem;
  position: absolute;
  top: 2rem;
  right: 2rem;
}

.again {
  position: absolute;
  top: 2rem;
  left: 2rem;
}

.guess {
  background: none;
  border: 4px solid #eee;
  font-family: inherit;
  color: inherit;
  font-size: 5rem;
  padding: 2.5rem;
  width: 25rem;
  text-align: center;
  display: block;
  margin-bottom: 3rem;
}

.btn {
  border: none;
  background-color: #eee;
  color: #222;
  font-size: 2rem;
  font-family: inherit;
  padding: 2rem 3rem;
  cursor: pointer;
}

.btn:hover {
  background-color: #ccc;
}

.message {
  margin-bottom: 8rem;
  height: 3rem;
}

.label-score {
  margin-bottom: 2rem;
}
```

```js
"use strict";

/*
console.log(document.querySelector('.message').textContent);
document.querySelector('.message').textContent = '🎉 Correct Number!';

document.querySelector('.number').textContent = 13;
document.querySelector('.score').textContent = 10;

document.querySelector('.guess').value = 23;
console.log(document.querySelector('.guess').value);
*/

let secretNumber = Math.trunc(Math.random() * 20) + 1;
let score = 20;
let highscore = 0;

const displayMessage = function (message) {
  document.querySelector(".message").textContent = message;
};

document.querySelector(".check").addEventListener("click", function () {
  const guess = Number(document.querySelector(".guess").value);
  console.log(guess, typeof guess);

  // When there is no input
  if (!guess) {
    // document.querySelector('.message').textContent = '⛔️ No number!';
    displayMessage("⛔️ No number!");

    // When player wins
  } else if (guess === secretNumber) {
    // document.querySelector('.message').textContent = '🎉 Correct Number!';
    displayMessage("🎉 Correct Number!");
    document.querySelector(".number").textContent = secretNumber;

    document.querySelector("body").style.backgroundColor = "#60b347";
    document.querySelector(".number").style.width = "30rem";

    if (score > highscore) {
      highscore = score;
      document.querySelector(".highscore").textContent = highscore;
    }

    // When guess is wrong
  } else if (guess !== secretNumber) {
    if (score > 1) {
      // document.querySelector('.message').textContent =
      // guess > secretNumber ? '📈 Too high!' : '📉 Too low!';
      displayMessage(guess > secretNumber ? "📈 Too high!" : "📉 Too low!");
      score--;
      document.querySelector(".score").textContent = score;
    } else {
      // document.querySelector('.message').textContent = '💥 You lost the game!';
      displayMessage("💥 You lost the game!");
      document.querySelector(".score").textContent = 0;
    }
  }

  //   // When guess is too high
  // } else if (guess > secretNumber) {
  //   if (score > 1) {
  //     document.querySelector('.message').textContent = '📈 Too high!';
  //     score--;
  //     document.querySelector('.score').textContent = score;
  //   } else {
  //     document.querySelector('.message').textContent = '💥 You lost the game!';
  //     document.querySelector('.score').textContent = 0;
  //   }

  //   // When guess is too low
  // } else if (guess < secretNumber) {
  //   if (score > 1) {
  //     document.querySelector('.message').textContent = '📉 Too low!';
  //     score--;
  //     document.querySelector('.score').textContent = score;
  //   } else {
  //     document.querySelector('.message').textContent = '💥 You lost the game!';
  //     document.querySelector('.score').textContent = 0;
  //   }
  // }
});

document.querySelector(".again").addEventListener("click", function () {
  score = 20;
  secretNumber = Math.trunc(Math.random() * 20) + 1;

  // document.querySelector('.message').textContent = 'Start guessing...';
  displayMessage("Start guessing...");
  document.querySelector(".score").textContent = score;
  document.querySelector(".number").textContent = "?";
  document.querySelector(".guess").value = "";

  document.querySelector("body").style.backgroundColor = "#222";
  document.querySelector(".number").style.width = "15rem";
});

///////////////////////////////////////
// Coding Challenge #1

/* 
Implement a game rest functionality, so that the player can make a new guess! Here is how:

1. Select the element with the 'again' class and attach a click event handler
2. In the handler function, restore initial values of the score and secretNumber variables
3. Restore the initial conditions of the message, number, score and guess input field
4. Also restore the original background color (#222) and number width (15rem)

GOOD LUCK 😀
*/
```

### Pig Game

![Flowchart](/images/pig-game-flowchart.png "Flowchart")

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="style.css" />
    <title>Pig Game</title>
  </head>
  <body>
    <main>
      <section class="player player--0 player--active">
        <h2 class="name" id="name--0">Player 1</h2>
        <p class="score" id="score--0">43</p>
        <div class="current">
          <p class="current-label">Current</p>
          <p class="current-score" id="current--0">0</p>
        </div>
      </section>
      <section class="player player--1">
        <h2 class="name" id="name--1">Player 2</h2>
        <p class="score" id="score--1">24</p>
        <div class="current">
          <p class="current-label">Current</p>
          <p class="current-score" id="current--1">0</p>
        </div>
      </section>

      <img src="dice-5.png" alt="Playing dice" class="dice" />
      <button class="btn btn--new">🔄 New game</button>
      <button class="btn btn--roll">🎲 Roll dice</button>
      <button class="btn btn--hold">📥 Hold</button>
    </main>
    <script src="script.js"></script>
  </body>
</html>
```

```css
@import url("https://fonts.googleapis.com/css2?family=Nunito&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  font-size: 62.5%;
  box-sizing: border-box;
}

body {
  font-family: "Nunito", sans-serif;
  font-weight: 400;
  height: 100vh;
  color: #333;
  background-image: linear-gradient(to top left, #753682 0%, #bf2e34 100%);
  display: flex;
  align-items: center;
  justify-content: center;
}

/* LAYOUT */
main {
  position: relative;
  width: 100rem;
  height: 60rem;
  background-color: rgba(255, 255, 255, 0.35);
  backdrop-filter: blur(200px);
  filter: blur();
  box-shadow: 0 3rem 5rem rgba(0, 0, 0, 0.25);
  border-radius: 9px;
  overflow: hidden;
  display: flex;
}

.player {
  flex: 50%;
  padding: 9rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: all 0.75s;
}

/* ELEMENTS */
.name {
  position: relative;
  font-size: 4rem;
  text-transform: uppercase;
  letter-spacing: 1px;
  word-spacing: 2px;
  font-weight: 300;
  margin-bottom: 1rem;
}

.score {
  font-size: 8rem;
  font-weight: 300;
  color: #c7365f;
  margin-bottom: auto;
}

.player--active {
  background-color: rgba(255, 255, 255, 0.4);
}
.player--active .name {
  font-weight: 700;
}
.player--active .score {
  font-weight: 400;
}

.player--active .current {
  opacity: 1;
}

.current {
  background-color: #c7365f;
  opacity: 0.8;
  border-radius: 9px;
  color: #fff;
  width: 65%;
  padding: 2rem;
  text-align: center;
  transition: all 0.75s;
}

.current-label {
  text-transform: uppercase;
  margin-bottom: 1rem;
  font-size: 1.7rem;
  color: #ddd;
}

.current-score {
  font-size: 3.5rem;
}

/* ABSOLUTE POSITIONED ELEMENTS */
.btn {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  color: #444;
  background: none;
  border: none;
  font-family: inherit;
  font-size: 1.8rem;
  text-transform: uppercase;
  cursor: pointer;
  font-weight: 400;
  transition: all 0.2s;

  background-color: white;
  background-color: rgba(255, 255, 255, 0.6);
  backdrop-filter: blur(10px);

  padding: 0.7rem 2.5rem;
  border-radius: 50rem;
  box-shadow: 0 1.75rem 3.5rem rgba(0, 0, 0, 0.1);
}

.btn::first-letter {
  font-size: 2.4rem;
  display: inline-block;
  margin-right: 0.7rem;
}

.btn--new {
  top: 4rem;
}
.btn--roll {
  top: 39.3rem;
}
.btn--hold {
  top: 46.1rem;
}

.btn:active {
  transform: translate(-50%, 3px);
  box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.15);
}

.btn:focus {
  outline: none;
}

.dice {
  position: absolute;
  left: 50%;
  top: 16.5rem;
  transform: translateX(-50%);
  height: 10rem;
  box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.2);
}

.player--winner {
  background-color: #2f2f2f;
}

.player--winner .name {
  font-weight: 700;
  color: #c7365f;
}

.hidden {
  display: none;
}
```

```js
"use strict";

// Selecting elements
const player0El = document.querySelector(".player--0");
const player1El = document.querySelector(".player--1");
const score0El = document.querySelector("#score--0");
const score1El = document.getElementById("score--1");
const current0El = document.getElementById("current--0");
const current1El = document.getElementById("current--1");

const diceEl = document.querySelector(".dice");
const btnNew = document.querySelector(".btn--new");
const btnRoll = document.querySelector(".btn--roll");
const btnHold = document.querySelector(".btn--hold");

let scores, currentScore, activePlayer, playing;

// Starting conditions
const init = function () {
  scores = [0, 0];
  currentScore = 0;
  activePlayer = 0;
  playing = true;

  score0El.textContent = 0;
  score1El.textContent = 0;
  current0El.textContent = 0;
  current1El.textContent = 0;

  diceEl.classList.add("hidden");
  player0El.classList.remove("player--winner");
  player1El.classList.remove("player--winner");
  player0El.classList.add("player--active");
  player1El.classList.remove("player--active");
};
init();

const switchPlayer = function () {
  document.getElementById(`current--${activePlayer}`).textContent = 0;
  currentScore = 0;
  activePlayer = activePlayer === 0 ? 1 : 0;
  player0El.classList.toggle("player--active");
  player1El.classList.toggle("player--active");
};

// Rolling dice functionality
btnRoll.addEventListener("click", function () {
  if (playing) {
    // 1. Generating a random dice roll
    const dice = Math.trunc(Math.random() * 6) + 1;

    // 2. Display dice
    diceEl.classList.remove("hidden");
    diceEl.src = `dice-${dice}.png`;

    // 3. Check for rolled 1
    if (dice !== 1) {
      // Add dice to current score
      currentScore += dice;
      document.getElementById(`current--${activePlayer}`).textContent =
        currentScore;
    } else {
      // Switch to next player
      switchPlayer();
    }
  }
});

btnHold.addEventListener("click", function () {
  if (playing) {
    // 1. Add current score to active player's score
    scores[activePlayer] += currentScore;
    // scores[1] = scores[1] + currentScore

    document.getElementById(`score--${activePlayer}`).textContent =
      scores[activePlayer];

    // 2. Check if player's score is >= 100
    if (scores[activePlayer] >= 100) {
      // Finish the game
      playing = false;
      diceEl.classList.add("hidden");

      document
        .querySelector(`.player--${activePlayer}`)
        .classList.add("player--winner");
      document
        .querySelector(`.player--${activePlayer}`)
        .classList.remove("player--active");
    } else {
      // Switch to the next player
      switchPlayer();
    }
  }
});

btnNew.addEventListener("click", init);
```

---

## Enhanced Object Literals

ES6 introduced enhanced object literals that make object creation more concise:

```javascript
const weekdays = ["mon", "tue", "wed", "thu", "fri", "sat", "sun"];
const openingHours = {
  [weekdays[3]]: {
    open: 12,
    close: 22,
  },
  [weekdays[4]]: {
    open: 11,
    close: 23,
  },
  [weekdays[5]]: {
    open: 0, // Open 24 hours
    close: 24,
  },
};

const restaurant = {
  name: "Classico Italiano",
  location: "Via Angelo Tavanti 23, Firenze, Italy",
  categories: ["Italian", "Pizzeria", "Vegetarian", "Organic"],

  // ES6 enhanced object literals
  openingHours,

  order(starterIndex, mainIndex) {
    return [this.starterMenu[starterIndex], this.mainMenu[mainIndex]];
  },
};
```

## Destructuring Arrays

Destructuring allows you to unpack values from arrays into distinct variables:

```javascript
const arr = [2, 3, 4];
const [x, y, z] = arr;
console.log(x, y, z); // 2 3 4

// Skip elements
let [main, , secondary] = restaurant.categories;

// Switching variables
[main, secondary] = [secondary, main];

// Nested destructuring
const nested = [2, 4, [5, 6]];
const [i, , [j, k]] = nested;
console.log(i, j, k); // 2 5 6

// Default values
const [p = 1, q = 1, r = 1] = [8, 9];
console.log(p, q, r); // 8 9 1
```

## Destructuring Objects

Extract object properties into variables:

```javascript
const { name, openingHours, categories } = restaurant;

// Rename variables
const {
  name: restaurantName,
  openingHours: hours,
  categories: tags,
} = restaurant;

// Default values
const { menu = [], starterMenu: starters = [] } = restaurant;

// Mutating variables
let a = 111;
let b = 999;
const obj = { a: 23, b: 7, c: 14 };
({ a, b } = obj);

// Nested objects
const {
  fri: { open: o, close: c },
} = openingHours;
```

## The Spread Operator (...)

The spread operator expands elements:

```javascript
const arr = [7, 8, 9];
const newArr = [1, 2, ...arr]; // [1, 2, 7, 8, 9]

// Copy array
const mainMenuCopy = [...restaurant.mainMenu];

// Join arrays
const menu = [...restaurant.starterMenu, ...restaurant.mainMenu];

// Works with strings
const str = "Jonas";
const letters = [...str, " ", "S."]; // ['J', 'o', 'n', 'a', 's', ' ', 'S.']

// Objects (ES2018)
const newRestaurant = { foundedIn: 1998, ...restaurant, founder: "Guiseppe" };
```

## Rest Pattern and Parameters

Collect multiple elements into an array:

```javascript
// 1) Destructuring
const [a, b, ...others] = [1, 2, 3, 4, 5];
console.log(a, b, others); // 1 2 [3, 4, 5]

// Objects
const { sat, ...weekdays } = restaurant.openingHours;

// 2) Functions - collect arguments
const add = function (...numbers) {
  let sum = 0;
  for (let i = 0; i < numbers.length; i++) sum += numbers[i];
  console.log(sum);
};

add(2, 3);
add(5, 3, 7, 2);
```

## Short Circuiting (&& and ||)

Logical operators can return values and short-circuit:

```javascript
// OR operator - returns first truthy value
console.log(3 || "Jonas"); // 3
console.log("" || "Jonas"); // 'Jonas'
console.log(undefined || 0 || "" || "Hello" || 23 || null); // 'Hello'

// Set default values
const guests2 = restaurant.numGuests || 10;

// AND operator - returns first falsy value
console.log(0 && "Jonas"); // 0
console.log(7 && "Jonas"); // 'Jonas'

// Execute code if method exists
restaurant.orderPizza && restaurant.orderPizza("mushrooms", "spinach");
```

## The Nullish Coalescing Operator

Works with nullish values (null and undefined):

```javascript
restaurant.numGuests = 0;
const guests = restaurant.numGuests || 10; // 10 (wrong!)

// Nullish: null and undefined (NOT 0 or '')
const guestCorrect = restaurant.numGuests ?? 10; // 0 (correct!)
```

## Logical Assignment Operators

Assign values based on logical operators:

```javascript
// OR assignment operator
rest1.numGuests ||= 10;
rest2.numGuests ||= 10;

// Nullish assignment operator
rest1.numGuests ??= 10;
rest2.numGuests ??= 10;

// AND assignment operator
rest1.owner &&= "<ANONYMOUS>";
rest2.owner &&= "<ANONYMOUS>";
```

## The for-of Loop

Loop over iterable objects:

```javascript
const menu = [...restaurant.starterMenu, ...restaurant.mainMenu];

for (const item of menu) console.log(item);

// Get index and element
for (const [i, el] of menu.entries()) {
  console.log(`${i + 1}: ${el}`);
}
```

## Optional Chaining

Safely access nested object properties:

```javascript
// Without optional chaining
if (restaurant.openingHours && restaurant.openingHours.mon)
  console.log(restaurant.openingHours.mon.open);

// WITH optional chaining
console.log(restaurant.openingHours.mon?.open);
console.log(restaurant.openingHours?.mon?.open);

// Methods
console.log(restaurant.order?.(0, 1) ?? "Method does not exist");

// Arrays
const users = [{ name: "Jonas", email: "hello@jonas.io" }];
console.log(users[0]?.name ?? "User array empty");
```

## Looping Objects: Object Keys, Values, and Entries

Loop over object properties:

```javascript
// Property NAMES
const properties = Object.keys(openingHours);
console.log(properties);

// Property VALUES
const values = Object.values(openingHours);
console.log(values);

// Entire object
const entries = Object.entries(openingHours);

// [key, value] destructuring
for (const [day, { open, close }] of entries) {
  console.log(`On ${day} we open at ${open} and close at ${close}`);
}
```

## Sets

Store unique values:

```javascript
const ordersSet = new Set([
  "Pasta",
  "Pizza",
  "Pizza",
  "Risotto",
  "Pasta",
  "Pizza",
]);
console.log(ordersSet); // Set(3) {'Pasta', 'Pizza', 'Risotto'}

console.log(new Set("Jonas")); // Set(5) {'J', 'o', 'n', 'a', 's'}

// Methods
console.log(ordersSet.size);
console.log(ordersSet.has("Pizza"));
ordersSet.add("Garlic Bread");
ordersSet.delete("Risotto");

// Convert to array
const staff = ["Waiter", "Chef", "Waiter", "Manager", "Chef", "Waiter"];
const staffUnique = [...new Set(staff)];
```

## New Operations to Make Sets Useful!

Modern set operations:

```javascript
const italianFoods = new Set([
  "pasta",
  "gnocchi",
  "tomatoes",
  "olive oil",
  "garlic",
  "basil",
]);
const mexicanFoods = new Set([
  "tortillas",
  "beans",
  "rice",
  "tomatoes",
  "avocado",
  "garlic",
]);

// Intersection
const commonFoods = italianFoods.intersection(mexicanFoods);

// Union
const italianMexicanFusion = italianFoods.union(mexicanFoods);

// Difference
const uniqueItalianFoods = italianFoods.difference(mexicanFoods);

// Symmetric difference
const uniqueItalianAndMexicanFoods =
  italianFoods.symmetricDifference(mexicanFoods);

// Disjoint check
console.log(italianFoods.isDisjointFrom(mexicanFoods));
```

## Maps: Fundamentals

Key-value pairs with any data type as keys:

```javascript
const rest = new Map();
rest.set("name", "Classico Italiano");
rest.set(1, "Firenze, Italy");
console.log(rest.set(2, "Lisbon, Portugal"));

// Method chaining
rest
  .set("categories", ["Italian", "Pizzeria", "Vegetarian", "Organic"])
  .set("open", 11)
  .set("close", 23)
  .set(true, "We are open :D")
  .set(false, "We are closed :(");

// Get values
console.log(rest.get("name"));
console.log(rest.get(true));

// Dynamic keys
const time = 8;
console.log(rest.get(time > rest.get("open") && time < rest.get("close")));

// Other methods
console.log(rest.has("categories"));
rest.delete(2);
console.log(rest.size);
```

## Maps: Iteration

Loop over maps and convert between data structures:

```javascript
const question = new Map([
  ["question", "What is the best programming language in the world?"],
  [1, "C"],
  [2, "Java"],
  [3, "JavaScript"],
  ["correct", 3],
  [true, "Correct 🎉"],
  [false, "Try again!"],
]);

// Convert object to map
const hoursMap = new Map(Object.entries(openingHours));

// Quiz app example
for (const [key, value] of question) {
  if (typeof key === "number") console.log(`Answer ${key}: ${value}`);
}

// Convert map to array
console.log([...question]);
console.log([...question.keys()]);
console.log([...question.values()]);
```

## Working With Strings - Part 1

Basic string methods:

```javascript
const airline = "TAP Air Portugal";
const plane = "A320";

// Accessing characters
console.log(plane[0]); // 'A'
console.log("B737"[0]); // 'B'

// Length
console.log(airline.length); // 16

// Index methods
console.log(airline.indexOf("r")); // 6
console.log(airline.lastIndexOf("r")); // 10
console.log(airline.indexOf("portugal")); // -1 (case sensitive)

// Slice method
console.log(airline.slice(4)); // 'Air Portugal'
console.log(airline.slice(4, 7)); // 'Air'
console.log(airline.slice(0, airline.indexOf(" "))); // 'TAP'
console.log(airline.slice(airline.lastIndexOf(" ") + 1)); // 'Portugal'
console.log(airline.slice(-2)); // 'al'
console.log(airline.slice(1, -1)); // 'AP Air Portuga'

// Practical example
const checkMiddleSeat = function (seat) {
  const s = seat.slice(-1);
  if (s === "B" || s === "E") console.log("You got the middle seat 😬");
  else console.log("You got lucky 😎");
};
```

## Working With Strings - Part 2

String transformation and manipulation:

```javascript
const airline = "TAP Air Portugal";

// Case transformation
console.log(airline.toLowerCase());
console.log(airline.toUpperCase());

// Fix capitalization
const passenger = "jOnAS";
const passengerLower = passenger.toLowerCase();
const passengerCorrect =
  passengerLower[0].toUpperCase() + passengerLower.slice(1);

// Comparing emails
const email = "hello@jonas.io";
const loginEmail = "  Hello@Jonas.Io \n";
const normalizedEmail = loginEmail.toLowerCase().trim();

// Replacing
const priceGB = "288,97£";
const priceUS = priceGB.replace("£", "$").replace(",", ".");

const announcement =
  "All passengers come to boarding door 23. Boarding door 23!";
console.log(announcement.replace("door", "gate"));
console.log(announcement.replaceAll("door", "gate"));

// Regular expression alternative
console.log(announcement.replace(/door/g, "gate"));

// Boolean methods
const plane = "Airbus A320neo";
console.log(plane.includes("A320")); // true
console.log(plane.startsWith("Airb")); // true
console.log(plane.endsWith("neo")); // true

// Practice exercise
const checkBaggage = function (items) {
  const baggage = items.toLowerCase();
  if (baggage.includes("knife") || baggage.includes("gun")) {
    console.log("You are NOT allowed on board");
  } else {
    console.log("Welcome aboard!");
  }
};
```

## Working With Strings - Part 3

Advanced string methods:

```javascript
// Split and join
console.log("a+very+nice+string".split("+")); // ['a', 'very', 'nice', 'string']
console.log("Jonas Schmedtmann".split(" ")); // ['Jonas', 'Schmedtmann']

const [firstName, lastName] = "Jonas Schmedtmann".split(" ");
const newName = ["Mr.", firstName, lastName.toUpperCase()].join(" ");

// Capitalize names
const capitalizeName = function (name) {
  const names = name.split(" ");
  const namesUpper = [];

  for (const n of names) {
    namesUpper.push(n[0].toUpperCase() + n.slice(1));
  }
  console.log(namesUpper.join(" "));
};

// Padding
const message = "Go to gate 23!";
console.log(message.padStart(20, "+").padEnd(30, "+"));

// Credit card masking
const maskCreditCard = function (number) {
  const str = number + "";
  const last = str.slice(-4);
  return last.padStart(str.length, "*");
};

// Repeat
const message2 = "Bad weather... All Departures Delayed... ";
console.log(message2.repeat(5));

const planesInLine = function (n) {
  console.log(`There are ${n} planes in line ${"🛩".repeat(n)}`);
};
```

## Coding Challenges

### Challenge #1 - Football Betting App

**Task**: Working with destructuring, rest/spread operators, and logical operators.

**Test Data**:

```javascript
const game = {
  team1: "Bayern Munich",
  team2: "Borrussia Dortmund",
  players: [
    [
      "Neuer",
      "Pavard",
      "Martinez",
      "Alaba",
      "Davies",
      "Kimmich",
      "Goretzka",
      "Coman",
      "Muller",
      "Gnarby",
      "Lewandowski",
    ],
    [
      "Burki",
      "Schulz",
      "Hummels",
      "Akanji",
      "Hakimi",
      "Weigl",
      "Witsel",
      "Hazard",
      "Brandt",
      "Sancho",
      "Gotze",
    ],
  ],
  score: "4:0",
  scored: ["Lewandowski", "Gnarby", "Lewandowski", "Hummels"],
  date: "Nov 9th, 2037",
  odds: {
    team1: 1.33,
    x: 3.25,
    team2: 6.5,
  },
};
```

**Solution**:

```javascript
// 1. Create player arrays for each team
const [players1, players2] = game.players;
console.log(players1, players2);

// 2. Create goalkeeper and field players for Bayern Munich
const [gk, ...fieldPlayers] = players1;
console.log(gk, fieldPlayers);

// 3. Create array with all players
const allPlayers = [...players1, ...players2];
console.log(allPlayers);

// 4. Create final team1 with substitute players
const players1Final = [...players1, "Thiago", "Coutinho", "Periscic"];

// 5. Create variables for each odd
const {
  odds: { team1, x: draw, team2 },
} = game;
console.log(team1, draw, team2);

// 6. Function to print goals
const printGoals = function (...players) {
  console.log(players);
  console.log(`${players.length} goals were scored`);
};

printGoals(...game.scored);

// 7. Team more likely to win (without if/else)
team1 < team2 && console.log("Team 1 is more likely to win");
team1 > team2 && console.log("Team 2 is more likely to win");
```

### Challenge #2 - Football Statistics

**Tasks**:

1. Loop over game.scored array and print each player name with goal number
2. Calculate and log the average odd
3. Print the 3 odds in a nice formatted way
4. BONUS: Create 'scorers' object with player names and goal counts

**Solution**:

```javascript
// 1. Loop over scored array
for (const [i, player] of game.scored.entries())
  console.log(`Goal ${i + 1}: ${player}`);

// 2. Calculate average odd
const odds = Object.values(game.odds);
let average = 0;
for (const odd of odds) average += odd;
average /= odds.length;
console.log(average);

// 3. Print odds in formatted way
for (const [team, odd] of Object.entries(game.odds)) {
  const teamStr = team === "x" ? "draw" : `victory ${game[team]}`;
  console.log(`Odd of ${teamStr} ${odd}`);
}
// Output:
// Odd of victory Bayern Munich: 1.33
// Odd of draw: 3.25
// Odd of victory Borrussia Dortmund: 6.5

// BONUS: Create scorers object
const scorers = {};
for (const player of game.scored) {
  scorers[player] ? scorers[player]++ : (scorers[player] = 1);
}
console.log(scorers);
// Output: { Gnarby: 1, Hummels: 1, Lewandowski: 2 }
```

### Challenge #3 - Game Events

**Task**: Working with Maps to handle game events.

**Test Data**:

```javascript
const gameEvents = new Map([
  [17, "⚽️ GOAL"],
  [36, "🔁 Substitution"],
  [47, "⚽️ GOAL"],
  [61, "🔁 Substitution"],
  [64, "🔶 Yellow card"],
  [69, "🔴 Red card"],
  [70, "🔁 Substitution"],
  [72, "🔁 Substitution"],
  [76, "⚽️ GOAL"],
  [80, "⚽️ GOAL"],
  [92, "🔶 Yellow card"],
]);
```

**Solution**:

```javascript
// 1. Create events array (no duplicates)
const events = [...new Set(gameEvents.values())];
console.log(events);

// 2. Remove unfair yellow card from minute 64
gameEvents.delete(64);

// 3. Print average event frequency
console.log(
  `An event happened, on average, every ${90 / gameEvents.size} minutes`
);

// Alternative calculation using actual game time
const time = [...gameEvents.keys()].pop();
console.log(
  `An event happened, on average, every ${time / gameEvents.size} minutes`
);

// 4. Loop over events and mark first/second half
for (const [min, event] of gameEvents) {
  const half = min <= 45 ? "FIRST" : "SECOND";
  console.log(`[${half} HALF] ${min}: ${event}`);
}
```

### Challenge #4 - CamelCase Converter

**Task**: Convert underscore_case to camelCase from textarea input.

**Test Data**:

```
underscore_case
 first_name
Some_Variable
  calculate_AGE
delayed_departure
```

**Expected Output**:

```
underscoreCase      ✅
firstName           ✅✅
someVariable        ✅✅✅
calculateAge        ✅✅✅✅
delayedDeparture    ✅✅✅✅✅
```

**Solution**:

```javascript
document.body.append(document.createElement("textarea"));
document.body.append(document.createElement("button"));

document.querySelector("button").addEventListener("click", function () {
  const text = document.querySelector("textarea").value;
  const rows = text.split("\n");

  for (const [i, row] of rows.entries()) {
    const [first, second] = row.toLowerCase().trim().split("_");

    const output = `${first}${second.replace(
      second[0],
      second[0].toUpperCase()
    )}`;
    console.log(`${output.padEnd(20)}${"✅".repeat(i + 1)}`);
  }
});
```

### String Methods Practice - Flight Data

**Task**: Format flight information from a messy string into a clean, readable format.

**Test Data**:

```javascript
const flights =
  "_Delayed_Departure;fao93766109;txl2133758440;11:25+_Arrival;bru0943384722;fao93766109;11:45+_Delayed_Arrival;hel7439299980;fao93766109;12:05+_Departure;fao93766109;lis2323639855;12:30";
```

**Expected Output**:

```
🔴 Delayed Departure from FAO to TXL (11h25)
             Arrival from BRU to FAO (11h45)
  🔴 Delayed Arrival from HEL to FAO (12h05)
           Departure from FAO to LIS (12h30)
```

**Solution**:

```javascript
const getCode = (str) => str.slice(0, 3).toUpperCase();

for (const flight of flights.split("+")) {
  const [type, from, to, time] = flight.split(";");
  const output = `${type.startsWith("_Delayed") ? "🔴" : ""}${type.replaceAll(
    "_",
    " "
  )} from ${getCode(from)} to ${getCode(to)} (${time.replace(
    ":",
    "h"
  )})`.padStart(45);
  console.log(output);
}
```

---

## Default Parameters

Default parameters allow function parameters to have default values if no argument is passed or if `undefined` is passed.

```javascript
const createBooking = function (
  flightNum,
  numPassengers = 1,
  price = 199 * numPassengers
) {
  const booking = {
    flightNum,
    numPassengers,
    price,
  };
  console.log(booking);
  bookings.push(booking);
};

// Usage examples:
createBooking("LH123"); // Uses defaults: 1 passenger, 199 price
createBooking("LH123", 2, 800); // All parameters specified
createBooking("LH123", 2); // Uses default price calculation
createBooking("LH123", undefined, 1000); // Skip parameter with undefined
```

**Key Points:**

- Default values can reference other parameters
- Use `undefined` to skip a parameter and use its default
- Default parameters are evaluated at call time

---

## How Passing Arguments Works: Values vs. Reference

JavaScript passes primitive values by value and objects by reference.

```javascript
const flight = "LH234";
const jonas = {
  name: "Jonas Schmedtmann",
  passport: 24739479284,
};

const checkIn = function (flightNum, passenger) {
  flightNum = "LH999"; // Doesn't affect original
  passenger.name = "Mr. " + passenger.name; // Modifies original object
};

checkIn(flight, jonas);
console.log(flight); // Still 'LH234'
console.log(jonas); // Name is now 'Mr. Jonas Schmedtmann'
```

**Key Points:**

- Primitives (string, number, boolean) are passed by value
- Objects are passed by reference
- Modifying object properties inside functions affects the original object
- Reassigning parameters doesn't affect original values

---

## Functions Accepting Callback Functions

Higher-order functions can accept other functions as arguments (callback functions).

```javascript
const oneWord = function (str) {
  return str.replace(/ /g, "").toLowerCase();
};

const upperFirstWord = function (str) {
  const [first, ...others] = str.split(" ");
  return [first.toUpperCase(), ...others].join(" ");
};

// Higher-order function
const transformer = function (str, fn) {
  console.log(`Original string: ${str}`);
  console.log(`Transformed string: ${fn(str)}`);
  console.log(`Transformed by: ${fn.name}`);
};

// Usage:
transformer("JavaScript is the best!", upperFirstWord);
transformer("JavaScript is the best!", oneWord);
```

**Common Examples:**

```javascript
// Event listeners
document.body.addEventListener("click", high5);

// Array methods
["Jonas", "Martha", "Adam"].forEach(high5);
```

**Benefits:**

- Makes code more reusable and modular
- Enables abstraction
- JavaScript uses callbacks extensively

---

## Functions Returning Functions

Functions can return other functions, creating closures.

```javascript
const greet = function (greeting) {
  return function (name) {
    console.log(`${greeting} ${name}`);
  };
};

// Usage:
const greeterHey = greet("Hey");
greeterHey("Jonas"); // "Hey Jonas"
greeterHey("Steven"); // "Hey Steven"

// Direct call:
greet("Hello")("Jonas"); // "Hello Jonas"

// Arrow function version:
const greetArr = (greeting) => (name) => console.log(`${greeting} ${name}`);
greetArr("Hi")("Jonas"); // "Hi Jonas"
```

**Key Points:**

- Inner function has access to outer function's variables (closure)
- Useful for creating specialized functions
- Arrow functions can be chained for concise syntax

---

## The call and apply Methods

`call` and `apply` methods allow you to explicitly set the `this` keyword.

```javascript
const lufthansa = {
  airline: "Lufthansa",
  iataCode: "LH",
  bookings: [],
  book(flightNum, name) {
    console.log(
      `${name} booked a seat on ${this.airline} flight ${this.iataCode}${flightNum}`
    );
    this.bookings.push({ flight: `${this.iataCode}${flightNum}`, name });
  },
};

const eurowings = {
  airline: "Eurowings",
  iataCode: "EW",
  bookings: [],
};

const book = lufthansa.book;

// Call method - arguments passed individually
book.call(eurowings, 23, "Sarah Williams");

// Apply method - arguments passed as array
const flightData = [583, "George Cooper"];
book.apply(swiss, flightData);

// Modern alternative to apply:
book.call(swiss, ...flightData);
```

**Differences:**

- `call`: Arguments passed individually
- `apply`: Arguments passed as array
- Both set `this` explicitly

---

## The bind Method

`bind` creates a new function with a preset `this` value and optionally preset arguments.

```javascript
// Basic binding
const bookEW = book.bind(eurowings);
const bookLH = book.bind(lufthansa);

bookEW(23, "Steven Williams");

// Partial application - preset arguments
const bookEW23 = book.bind(eurowings, 23);
bookEW23("Jonas Schmedtmann");
bookEW23("Martha Cooper");

// With Event Listeners
lufthansa.buyPlane = function () {
  this.planes++;
  console.log(this.planes);
};

document
  .querySelector(".buy")
  .addEventListener("click", lufthansa.buyPlane.bind(lufthansa));

// Partial application example
const addTax = (rate, value) => value + value * rate;
const addVAT = addTax.bind(null, 0.23); // Preset rate to 23%

console.log(addVAT(100)); // 123
console.log(addVAT(23)); // 28.29
```

**Key Points:**

- Creates a new function (doesn't call original)
- First argument is `this` value
- Additional arguments are preset (partial application)
- Useful for event handlers and creating specialized functions

---

## Coding Challenge #1 - Poll App

A complete poll application demonstrating method binding and the `call` method.

```javascript
const poll = {
  question: "What is your favourite programming language?",
  options: ["0: JavaScript", "1: Python", "2: Rust", "3: C++"],
  answers: new Array(4).fill(0),

  registerNewAnswer() {
    // Get answer
    const answer = Number(
      prompt(
        `${this.question}\n${this.options.join("\n")}\n(Write option number)`
      )
    );

    // Register answer with validation
    typeof answer === "number" &&
      answer < this.answers.length &&
      this.answers[answer]++;

    this.displayResults();
    this.displayResults("string");
  },

  displayResults(type = "array") {
    if (type === "array") {
      console.log(this.answers);
    } else if (type === "string") {
      console.log(`Poll results are ${this.answers.join(", ")}`);
    }
  },
};

// Bind method for event listener
document
  .querySelector(".poll")
  .addEventListener("click", poll.registerNewAnswer.bind(poll));

// Using call method with test data
poll.displayResults.call({ answers: [5, 2, 3] }, "string");
poll.displayResults.call({ answers: [1, 5, 3, 9, 6, 1] }, "string");
```

**Features Demonstrated:**

- Object methods
- Input validation
- Method binding for events
- Using `call` to change `this` context
- Default parameters

---

## Immediately Invoked Function Expressions (IIFE)

IIFE patterns for executing functions immediately and creating scope.

```javascript
// Regular function (can be called again)
const runOnce = function () {
  console.log("This will never run again");
};
runOnce();

// IIFE with function expression
(function () {
  console.log("This will never run again");
  const isPrivate = 23; // Private variable
})();

// IIFE with arrow function
(() => console.log("This will ALSO never run again"))();

// Block scope alternative
{
  const isPrivate = 23;
  var notPrivate = 46;
}
console.log(notPrivate); // Works - var is function scoped
// console.log(isPrivate); // Error - const is block scoped
```

**Use Cases:**

- Execute code immediately
- Create private scope
- Avoid polluting global namespace
- Module pattern (before ES6 modules)

---

## Closures

Closures allow inner functions to access outer function variables even after the outer function returns.

```javascript
const secureBooking = function () {
  let passengerCount = 0;

  return function () {
    passengerCount++;
    console.log(`${passengerCount} passengers`);
  };
};

const booker = secureBooking();

booker(); // "1 passengers"
booker(); // "2 passengers"
booker(); // "3 passengers"

console.dir(booker); // Shows closure in browser dev tools
```

**Key Points:**

- Inner function remembers outer function's variables
- Variables are preserved even after outer function execution
- Creates private variables
- Closure has priority over scope chain

---

## More Closure Examples

Advanced closure patterns and behavior.

### Example 1: Variable Re-assignment

```javascript
let f;

const g = function () {
  const a = 23;
  f = function () {
    console.log(a * 2);
  };
};

const h = function () {
  const b = 777;
  f = function () {
    console.log(b * 2);
  };
};

g();
f(); // 46 (23 * 2)

// Re-assigning f function
h();
f(); // 1554 (777 * 2)
```

### Example 2: Closures with Timers

```javascript
const boardPassengers = function (n, wait) {
  const perGroup = n / 3;

  setTimeout(function () {
    console.log(`We are now boarding all ${n} passengers`);
    console.log(`There are 3 groups, each with ${perGroup} passengers`);
  }, wait * 1000);

  console.log(`Will start boarding in ${wait} seconds`);
};

const perGroup = 1000; // This global variable is ignored
boardPassengers(180, 3);
```

**Key Points:**

- Closures can be reassigned to different scopes
- Closure variables have priority over global variables
- Timers create closures with their callback functions

---

## Coding Challenge #2 - IIFE with Event Listener

Demonstrates closures with IIFE and event listeners.

```javascript
(function () {
  const header = document.querySelector("h1");
  header.style.color = "red";

  document.querySelector("body").addEventListener("click", function () {
    header.style.color = "blue";
  });
})();
```

**Why This Works:**

1. The IIFE executes immediately, creating a closure
2. The `header` variable is captured in the event listener's closure
3. Even after the IIFE finishes, the event listener retains access to `header`
4. When the body is clicked, the callback can still access and modify `header`
5. This demonstrates how closures preserve access to variables from outer scopes

**Key Concept:**
The event listener callback function "closes over" the `header` variable, keeping it alive and accessible even after the IIFE has finished executing.

---

## Constructor Functions and the new Operator

Constructor functions are used to create objects with shared properties and methods. They serve as blueprints for creating multiple instances.

### Basic Constructor Function

```javascript
const Person = function (firstName, birthYear) {
  // Instance properties
  this.firstName = firstName;
  this.birthYear = birthYear;
};

const jonas = new Person("Jonas", 1991);
const matilda = new Person("Matilda", 2017);
const jack = new Person("Jack", 1975);
```

### How the `new` Operator Works

1. New empty object `{}` is created
2. Function is called, `this` points to the new object
3. New object is linked to prototype
4. Function automatically returns the object

### Static Methods

```javascript
Person.hey = function () {
  console.log("Hey there 👋");
  console.log(this);
};
Person.hey();
```

### Instance Checking

```javascript
console.log(jonas instanceof Person); // true
```

---

## Prototypes

Prototypes allow objects to inherit methods and properties from other objects, enabling efficient memory usage and method sharing.

### Adding Methods to Prototype

```javascript
Person.prototype.calcAge = function () {
  console.log(2037 - this.birthYear);
};

jonas.calcAge();
matilda.calcAge();
```

### Prototype Chain Verification

```javascript
console.log(jonas.__proto__ === Person.prototype); // true
console.log(Person.prototype.isPrototypeOf(jonas)); // true
console.log(Person.prototype.isPrototypeOf(Person)); // false
```

### Adding Properties to Prototype

```javascript
Person.prototype.species = "Homo Sapiens";
console.log(jonas.species, matilda.species);
```

### Checking Own Properties

```javascript
console.log(jonas.hasOwnProperty("firstName")); // true
console.log(jonas.hasOwnProperty("species")); // false
```

---

## Prototypal Inheritance on Built-In Objects

JavaScript built-in objects also use prototypal inheritance.

### Exploring the Prototype Chain

```javascript
// Object.prototype (top of prototype chain)
console.log(jonas.__proto__.__proto__);
console.log(jonas.__proto__.__proto__.__proto__); // null
```

### Arrays and Prototypes

```javascript
const arr = [3, 6, 6, 5, 6, 9, 9];
console.log(arr.__proto__ === Array.prototype); // true
```

### Extending Built-in Prototypes

```javascript
Array.prototype.unique = function () {
  return [...new Set(this)];
};

console.log(arr.unique()); // [3, 6, 5, 9]
```

---

## Coding Challenge #1: Car Constructor

**Task**: Implement a Car using constructor function with accelerate and brake methods.

### Requirements

- Car has `make` and `speed` properties
- `accelerate` method increases speed by 10
- `brake` method decreases speed by 5
- Create BMW (120 km/h) and Mercedes (95 km/h)

### Solution

```javascript
const Car = function (make, speed) {
  this.make = make;
  this.speed = speed;
};

Car.prototype.accelerate = function () {
  this.speed += 10;
  console.log(`${this.make} is going at ${this.speed} km/h`);
};

Car.prototype.brake = function () {
  this.speed -= 5;
  console.log(`${this.make} is going at ${this.speed} km/h`);
};

const bmw = new Car("BMW", 120);
const mercedes = new Car("Mercedes", 95);

bmw.accelerate();
bmw.brake();
```

---

## ES6 Classes

ES6 classes provide a cleaner syntax for creating objects and implementing inheritance.

### Class Declaration

```javascript
class PersonCl {
  constructor(fullName, birthYear) {
    this.fullName = fullName;
    this.birthYear = birthYear;
  }

  // Instance methods
  calcAge() {
    console.log(2037 - this.birthYear);
  }

  greet() {
    console.log(`Hey ${this.fullName}`);
  }

  // Getter
  get age() {
    return 2037 - this.birthYear;
  }

  // Setter for validation
  set fullName(name) {
    if (name.includes(" ")) this._fullName = name;
    else alert(`${name} is not a full name!`);
  }

  get fullName() {
    return this._fullName;
  }

  // Static method
  static hey() {
    console.log("Hey there 👋");
    console.log(this);
  }
}

const jessica = new PersonCl("Jessica Davis", 1996);
jessica.calcAge();
console.log(jessica.age);
```

### Important Notes about Classes

1. Classes are NOT hoisted
2. Classes are first-class citizens
3. Classes are executed in strict mode

---

## Setters and Getters

Getters and setters allow you to define object accessors (computed properties).

### Object Literal Syntax

```javascript
const account = {
  owner: "Jonas",
  movements: [200, 530, 120, 300],

  get latest() {
    return this.movements.slice(-1).pop();
  },

  set latest(mov) {
    this.movements.push(mov);
  },
};

console.log(account.latest); // 300
account.latest = 50;
console.log(account.movements); // [200, 530, 120, 300, 50]
```

---

## Object.create

`Object.create` creates a new object with the specified prototype object and properties.

### Basic Usage

```javascript
const PersonProto = {
  calcAge() {
    console.log(2037 - this.birthYear);
  },

  init(firstName, birthYear) {
    this.firstName = firstName;
    this.birthYear = birthYear;
  },
};

const steven = Object.create(PersonProto);
steven.name = "Steven";
steven.birthYear = 2002;
steven.calcAge();

const sarah = Object.create(PersonProto);
sarah.init("Sarah", 1979);
sarah.calcAge();
```

---

## Coding Challenge #2: Car Class with Speed Conversion

**Task**: Recreate Challenge #1 using ES6 class with speed conversion methods.

### Requirements

- Use ES6 class syntax
- Add `speedUS` getter (km/h to mi/h)
- Add `speedUS` setter (mi/h to km/h)
- Test with Ford at 120 km/h

### Solution

```javascript
class CarCl {
  constructor(make, speed) {
    this.make = make;
    this.speed = speed;
  }

  accelerate() {
    this.speed += 10;
    console.log(`${this.make} is going at ${this.speed} km/h`);
  }

  brake() {
    this.speed -= 5;
    console.log(`${this.make} is going at ${this.speed} km/h`);
  }

  get speedUS() {
    return this.speed / 1.6;
  }

  set speedUS(speed) {
    this.speed = speed * 1.6;
  }
}

const ford = new CarCl("Ford", 120);
console.log(ford.speedUS); // 75
ford.speedUS = 50;
console.log(ford.speed); // 80
```

---

## Inheritance Between Classes: Constructor Functions

Implementing inheritance using constructor functions requires manual prototype linking.

### Parent Constructor

```javascript
const Person = function (firstName, birthYear) {
  this.firstName = firstName;
  this.birthYear = birthYear;
};

Person.prototype.calcAge = function () {
  console.log(2037 - this.birthYear);
};
```

### Child Constructor with Inheritance

```javascript
const Student = function (firstName, birthYear, course) {
  Person.call(this, firstName, birthYear);
  this.course = course;
};

// Linking prototypes
Student.prototype = Object.create(Person.prototype);

Student.prototype.introduce = function () {
  console.log(`My name is ${this.firstName} and I study ${this.course}`);
};

const mike = new Student("Mike", 2020, "Computer Science");
mike.introduce();
mike.calcAge();

// Fix constructor reference
Student.prototype.constructor = Student;
```

### Instanceof Checks

```javascript
console.log(mike instanceof Student); // true
console.log(mike instanceof Person); // true
console.log(mike instanceof Object); // true
```

---

## Coding Challenge #3: Electric Car Inheritance

**Task**: Create an Electric Car (EV) as a child class of Car using constructor functions.

### Requirements

- EV has make, speed, and charge properties
- `chargeBattery` method sets battery charge
- `accelerate` method increases speed by 20, decreases charge by 1%
- Test with Tesla at 120 km/h, 23% charge

### Solution

```javascript
const Car = function (make, speed) {
  this.make = make;
  this.speed = speed;
};

Car.prototype.accelerate = function () {
  this.speed += 10;
  console.log(`${this.make} is going at ${this.speed} km/h`);
};

Car.prototype.brake = function () {
  this.speed -= 5;
  console.log(`${this.make} is going at ${this.speed} km/h`);
};

const EV = function (make, speed, charge) {
  Car.call(this, make, speed);
  this.charge = charge;
};

// Link the prototypes
EV.prototype = Object.create(Car.prototype);

EV.prototype.chargeBattery = function (chargeTo) {
  this.charge = chargeTo;
};

EV.prototype.accelerate = function () {
  this.speed += 20;
  this.charge--;
  console.log(
    `${this.make} is going at ${this.speed} km/h, with a charge of ${this.charge}%`
  );
};

const tesla = new EV("Tesla", 120, 23);
tesla.chargeBattery(90);
tesla.accelerate();
```

---

## Inheritance Between Classes: ES6 Classes

ES6 classes make inheritance much simpler with the `extends` keyword and `super()`.

### Parent Class

```javascript
class PersonCl {
  constructor(fullName, birthYear) {
    this.fullName = fullName;
    this.birthYear = birthYear;
  }

  calcAge() {
    console.log(2037 - this.birthYear);
  }

  greet() {
    console.log(`Hey ${this.fullName}`);
  }

  get age() {
    return 2037 - this.birthYear;
  }

  set fullName(name) {
    if (name.includes(" ")) this._fullName = name;
    else alert(`${name} is not a full name!`);
  }

  get fullName() {
    return this._fullName;
  }

  static hey() {
    console.log("Hey there 👋");
  }
}
```

### Child Class with Inheritance

```javascript
class StudentCl extends PersonCl {
  constructor(fullName, birthYear, course) {
    // Always needs to happen first!
    super(fullName, birthYear);
    this.course = course;
  }

  introduce() {
    console.log(`My name is ${this.fullName} and I study ${this.course}`);
  }

  calcAge() {
    console.log(
      `I'm ${
        2037 - this.birthYear
      } years old, but as a student I feel more like ${
        2037 - this.birthYear + 10
      }`
    );
  }
}

const martha = new StudentCl("Martha Jones", 2012, "Computer Science");
martha.introduce();
martha.calcAge();
```

---

## Inheritance Between Classes: Object.create

Using `Object.create` for inheritance provides the most direct control over the prototype chain.

### Setup

```javascript
const PersonProto = {
  calcAge() {
    console.log(2037 - this.birthYear);
  },

  init(firstName, birthYear) {
    this.firstName = firstName;
    this.birthYear = birthYear;
  },
};

const StudentProto = Object.create(PersonProto);
StudentProto.init = function (firstName, birthYear, course) {
  PersonProto.init.call(this, firstName, birthYear);
  this.course = course;
};

StudentProto.introduce = function () {
  console.log(`My name is ${this.firstName} and I study ${this.course}`);
};

const jay = Object.create(StudentProto);
jay.init("Jay", 2010, "Computer Science");
jay.introduce();
jay.calcAge();
```

---

## Encapsulation: Private Class Fields and Methods

Modern JavaScript supports true private fields and methods using the `#` syntax.

### Class Fields Types

1. Public fields
2. Private fields
3. Public methods
4. Private methods
5. Static versions of all above

### Example Implementation

```javascript
class Account {
  // Public fields
  locale = navigator.language;
  bank = "Bankist";

  // Private fields
  #movements = [];
  #pin;

  constructor(owner, currency, pin) {
    this.owner = owner;
    this.currency = currency;
    this.#pin = pin;
    console.log(`Thanks for opening an account, ${owner}`);
  }

  // Public interface (API)
  getMovements() {
    return this.#movements;
  }

  deposit(val) {
    this.#movements.push(val);
    return this; // For chaining
  }

  withdraw(val) {
    this.deposit(-val);
    return this;
  }

  // Private method
  #approveLoan(val) {
    return true;
  }

  requestLoan(val) {
    if (this.#approveLoan(val)) {
      this.deposit(val);
      console.log(`Loan approved`);
    }
    return this;
  }
}

const acc1 = new Account("Jonas", "EUR", 1111);

// Method chaining
const movements = acc1
  .deposit(300)
  .withdraw(100)
  .withdraw(50)
  .requestLoan(25000)
  .withdraw(4000)
  .getMovements();
```

---

## Coding Challenge #4: Electric Car with Private Fields

**Task**: Recreate Challenge #3 using ES6 classes with private fields and method chaining.

### Requirements

- Use ES6 classes with `extends`
- Make charge property private
- Implement method chaining for accelerate, chargeBattery, and brake
- Test with Rivian at 120 km/h, 23% charge

### Solution

```javascript
class CarCl {
  constructor(make, speed) {
    this.make = make;
    this.speed = speed;
  }

  accelerate() {
    this.speed += 10;
    console.log(`${this.make} is going at ${this.speed} km/h`);
  }

  brake() {
    this.speed -= 5;
    console.log(`${this.make} is going at ${this.speed} km/h`);
    return this; // For chaining
  }

  get speedUS() {
    return this.speed / 1.6;
  }

  set speedUS(speed) {
    this.speed = speed * 1.6;
  }
}

class EVCl extends CarCl {
  // Private field
  #charge;

  constructor(make, speed, charge) {
    super(make, speed);
    this.#charge = charge;
  }

  chargeBattery(chargeTo) {
    this.#charge = chargeTo;
    return this; // For chaining
  }

  accelerate() {
    this.speed += 20;
    this.#charge--;
    console.log(
      `${this.make} is going at ${this.speed} km/h, with a charge of ${
        this.#charge
      }%`
    );
    return this; // For chaining
  }
}

const rivian = new EVCl("Rivian", 120, 23);

// Method chaining demonstration
rivian
  .accelerate()
  .accelerate()
  .accelerate()
  .brake()
  .chargeBattery(50)
  .accelerate();

console.log(rivian.speedUS);
```

---
