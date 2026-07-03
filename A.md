
# JavaScript Introduction

---

# What is JavaScript?

**JavaScript (JS)** is a high-level, interpreted, lightweight, object-oriented, and dynamically typed programming language used to make web pages interactive and dynamic.

HTML provides the **structure** of a webpage.

CSS provides the **style** of a webpage.

JavaScript provides the **behavior and functionality** of a webpage.

Without JavaScript, a website is mostly static. JavaScript allows users to interact with web pages.

Examples include:

* Login Forms
* Registration Forms
* Image Sliders
* Dark Mode
* Pop-up Messages
* Online Calculators
* Games
* Real-time Chat Applications
* Shopping Cart
* Dynamic Content Updates

---

# Real World Example

Think of a Car.

* Engine → JavaScript
* Body → HTML
* Paint → CSS

The car body gives the structure.

The paint makes it attractive.

The engine makes it move.

Similarly,

HTML builds the webpage.

CSS designs the webpage.

JavaScript makes it interactive.

---

# Features of JavaScript

* Easy to Learn
* Lightweight Language
* Object-Oriented
* Cross Platform
* Event Driven
* Dynamic Typing
* Client Side Scripting
* Server Side Development using Node.js
* Supports Asynchronous Programming
* Large Community Support

---

# Why Learn JavaScript?

JavaScript is one of the most popular programming languages in the world.

It is used in:

* Frontend Development
* Backend Development
* Mobile App Development
* Desktop Applications
* Game Development
* Artificial Intelligence
* APIs
* Cloud Applications

---

# Applications of JavaScript

## Frontend

Examples

* Interactive Websites
* Animations
* Forms
* Dashboard

Frameworks

* React
* Angular
* Vue

---

## Backend

Using

Node.js

Examples

* REST APIs
* Authentication
* Database Operations

---

## Mobile Apps

Using

* React Native

---

## Desktop Applications

Using

* Electron

Applications

* VS Code
* Discord
* Slack

---

# Advantages of JavaScript

* Fast Execution
* Easy Syntax
* Huge Community
* Runs in Browser
* No Compilation Required
* Free to Use
* Platform Independent

---

# JavaScript Versions

| Version | Features                             |
| ------- | ------------------------------------ |
| ES5     | Basic JavaScript                     |
| ES6     | let, const, Arrow Functions, Classes |
| ES7     | Async Features                       |
| ES8     | Async Await                          |
| ES2020+ | Modern Features                      |

Today we mostly use **ES6+ JavaScript**.

---

# How JavaScript Works

```
User Clicks Button
        │
        ▼
Browser Receives Event
        │
        ▼
JavaScript Executes
        │
        ▼
HTML Updated
        │
        ▼
User Sees Result
```

---

# Ways to Add JavaScript

## 1. Inline JavaScript

```html
<button onclick="alert('Welcome')">
Click
</button>
```

Not recommended for large applications.

---

## 2. Internal JavaScript

```html
<script>

console.log("Hello JavaScript");

</script>
```

---

## 3. External JavaScript

HTML

```html
<script src="script.js"></script>
```

script.js

```javascript
console.log("External JavaScript");
```

Best Practice.

---

# First JavaScript Program

```javascript
console.log("Hello World");
```

Output

```
Hello World
```

---

# Printing Multiple Lines

```javascript
console.log("Welcome");
console.log("JavaScript");
console.log("Course");
```

Output

```
Welcome
JavaScript
Course
```

---

# Comments

Comments are ignored by JavaScript.

Used to explain code.

---

## Single Line Comment

```javascript
// This is comment
```

---

## Multi Line Comment

```javascript
/*
This
is
comment
*/
```

---

# VARIABLES

---

# What is a Variable?

A variable is a container used to store data.

Variables help us store information that can be used later.

Real-world Example

Think of a Water Bottle.

Bottle = Variable

Water = Data

You can fill different liquids in the same bottle.

Similarly,

Variables store different values.

---

# Why Variables?

Without Variables

```javascript
console.log("Rahul");
console.log("Rahul");
console.log("Rahul");
```

With Variables

```javascript
let name = "Rahul";

console.log(name);
console.log(name);
console.log(name);
```

Much easier to manage.

---

# Syntax

```javascript
keyword variableName = value;
```

Example

```javascript
let age = 20;
```

---

# Types of Variables

JavaScript has three keywords.

```
var

let

const
```

---

# var

Old way of declaring variables.

```javascript
var name = "Rahul";
```

---

Properties

* Can Redeclare
* Can Reassign
* Function Scoped

Example

```javascript
var a = 10;

var a = 20;

a = 30;

console.log(a);
```

Output

```
30
```

---

# let

Modern way.

Most commonly used.

```javascript
let age = 22;
```

Properties

* Cannot Redeclare
* Can Reassign
* Block Scoped

Example

```javascript
let marks = 90;

marks = 95;

console.log(marks);
```

Output

```
95
```

---

Redeclaration Error

```javascript
let age = 20;

let age = 30;
```

Output

```
Error
```

---

# const

Constant Variable.

Cannot change value.

```javascript
const PI = 3.14;
```

Properties

* Cannot Redeclare
* Cannot Reassign
* Block Scoped

Example

```javascript
const country = "India";

console.log(country);
```

Output

```
India
```

---

Trying to Change

```javascript
const country = "India";

country = "USA";
```

Output

```
Error
```

---

# Comparison

| Feature   | var      | let   | const |
| --------- | -------- | ----- | ----- |
| Redeclare | Yes      | No    | No    |
| Reassign  | Yes      | Yes   | No    |
| Scope     | Function | Block | Block |
| Modern    | No       | Yes   | Yes   |

---

# Variable Naming Rules

Allowed

```javascript
let name;

let studentName;

let student_name;

let student1;

let $price;

let _total;
```

---

Not Allowed

```javascript
let 1name;

let first-name;

let class;

let let;
```

---

# Best Practices

Good

```javascript
let firstName;

let studentAge;

let totalAmount;
```

Bad

```javascript
let a;

let b;

let x1;

let abc123;
```

Always use meaningful names.

---

# Multiple Variables

```javascript
let name = "John";

let age = 25;

let city = "Hyderabad";
```

---

Or

```javascript
let a = 10,
    b = 20,
    c = 30;
```

---

# Variable Example

```javascript
let student = "Ravi";

let age = 21;

console.log(student);

console.log(age);
```

Output

```
Ravi

21
```

---

# Swapping Variables

```javascript
let a = 10;

let b = 20;

let temp = a;

a = b;

b = temp;

console.log(a);

console.log(b);
```

Output

```
20

10
```

---

# DATA TYPES

---

# What is Data Type?

A Data Type specifies what type of value a variable stores.

Example

Age

```
20
```

Name

```
Rahul
```

Married

```
true
```

Different values have different data types.

---

# JavaScript Data Types

Two Categories

```
Primitive

Non Primitive
```

---

# Primitive Data Types

1 Number

2 String

3 Boolean

4 Undefined

5 Null

6 BigInt

7 Symbol

---

# Non Primitive

Objects

Arrays

Functions

Dates

Maps

Sets

---

# Number

Stores

* Integer
* Decimal

Example

```javascript
let age = 20;

let price = 99.99;
```

Output

```
20

99.99
```

---

Arithmetic

```javascript
let a = 10;

let b = 5;

console.log(a+b);

console.log(a-b);

console.log(a*b);

console.log(a/b);
```

Output

```
15

5

50

2
```

---

# String

Stores Text.

Can use

```
" "

' '

` `
```

Example

```javascript
let name = "Rahul";

console.log(name);
```

Output

```
Rahul
```

---

Concatenation

```javascript
let first = "Java";

let second = "Script";

console.log(first + second);
```

Output

```
JavaScript
```

---

Template Literal

```javascript
let name = "Rahul";

let age = 20;

console.log(`My name is ${name} and age is ${age}`);
```

Output

```
My name is Rahul and age is 20
```

---

# Boolean

Stores

```
true

false
```

Example

```javascript
let isStudent = true;

console.log(isStudent);
```

Output

```
true
```

---

# Undefined

Variable declared but not assigned.

```javascript
let city;

console.log(city);
```

Output

```
undefined
```

---

# Null

Represents empty value.

```javascript
let phone = null;

console.log(phone);
```

Output

```
null
```

---

# BigInt

Used for very large integers.

```javascript
let big = 123456789012345678901234567890n;

console.log(big);
```

---

# Symbol

Unique identifier.

```javascript
let id = Symbol("id");
```

Mostly used in advanced JavaScript.

---

# Object

Stores data in key-value pairs.

```javascript
let student = {

name : "Rahul",

age : 20,

city : "Hyderabad"

};

console.log(student);
```

Output

```
{name:"Rahul",age:20,city:"Hyderabad"}
```

---

# Array

Stores multiple values.

```javascript
let colors = [

"Red",

"Blue",

"Green"

];

console.log(colors);
```

Output

```
["Red","Blue","Green"]
```

---

# Function

Stores reusable code.

```javascript
function greet(){

console.log("Hello");

}

greet();
```

Output

```
Hello
```

---

# typeof Operator

Used to identify data type.

Syntax

```javascript
typeof variable
```

Example

```javascript
console.log(typeof 10);

console.log(typeof "Java");

console.log(typeof true);

console.log(typeof undefined);

console.log(typeof null);
```

Output

```
number

string

boolean

undefined

object
```

**Note:** `typeof null` returns `"object"` due to a historical bug in JavaScript.

---

# Type Conversion

## Automatic Conversion (Implicit)

```javascript
console.log("10" + 5);
```

Output

```
105
```

Because number `5` is converted into a string.

---

```javascript
console.log("10" - 5);
```

Output

```
5
```

Here JavaScript converts `"10"` into a number automatically.

---

## Manual Conversion (Explicit)

Convert String to Number

```javascript
let age = "25";

let numAge = Number(age);

console.log(numAge);

console.log(typeof numAge);
```

Output

```
25

number
```

---

Convert Number to String

```javascript
let price = 500;

let text = String(price);

console.log(text);

console.log(typeof text);
```

Output

```
500

string
```

---

Convert String to Boolean

```javascript
console.log(Boolean("Hello"));

console.log(Boolean(""));
```

Output

```
true

false
```

---

# Primitive vs Non-Primitive

| Primitive                | Non-Primitive           |
| ------------------------ | ----------------------- |
| Stores single value      | Stores multiple values  |
| Immutable                | Mutable                 |
| Compared by value        | Compared by reference   |
| Examples: Number, String | Object, Array, Function |

---

# Memory Tip

```
Primitive
↓

Simple Values

Number

String

Boolean

Undefined

Null

BigInt

Symbol
```

```
Non Primitive
↓

Complex Values

Object

Array

Function
```

---

# Common Beginner Mistakes

 Using `var` everywhere.

 Prefer `let` and `const`.

---

 Variable names like

```javascript
let a;
let x;
let abc;
```

 Use meaningful names.

```javascript
let studentName;
let totalMarks;
let employeeSalary;
```

---

 Forgetting quotes for strings.

Wrong

```javascript
let name = Rahul;
```

Correct

```javascript
let name = "Rahul";
```

---

 Confusing `=` and `==`

`=` → Assignment

`==` → Comparison (covered later)

---

# Interview Questions

1. What is JavaScript?
2. Difference between HTML, CSS, and JavaScript?
3. What are variables?
4. Difference between `var`, `let`, and `const`?
5. What is block scope?
6. What are primitive data types?
7. What is `undefined`?
8. Difference between `undefined` and `null`?
9. What is `typeof`?
10. Why does `typeof null` return `"object"`?
11. What is a template literal?
12. What is type conversion?
13. Difference between implicit and explicit conversion?
14. What is BigInt?
15. What are non-primitive data types?

---

# Practice Programs

### Program 1

```javascript
let name = "Apex";

console.log(name);
```

---

### Program 2

```javascript
let age = 22;

console.log(age);
```

---

### Program 3

```javascript
let first = "Hello";

let second = "World";

console.log(first + " " + second);
```

---

### Program 4

```javascript
const PI = 3.14159;

console.log(PI);
```

---

### Program 5

```javascript
let student = {
    name: "Rahul",
    age: 20,
    course: "Java Full Stack"
};

console.log(student);
```

---

### Program 6

```javascript
let fruits = ["Apple", "Mango", "Orange"];

console.log(fruits);
```

---

### Program 7

```javascript
let salary = "50000";

console.log(Number(salary));
```

---

Awesome! I'm glad you liked the format. 😊

For the rest of the course, I'll keep the **same professional structure**:

* ✅ Simple definitions
* ✅ Real-world examples
* ✅ Easy explanations
* ✅ Syntax
* ✅ Multiple code examples
* ✅ Output for every program
* ✅ Tables
* ✅ Important Notes
* ✅ Memory Tips
* ✅ Common Beginner Mistakes
* ✅ Interview Questions
* ✅ Practice Programs
* ✅ Summary

---

# Day 1 - JavaScript Fundamentals (Part 2)

# Operators

---

# What is an Operator?

An **Operator** is a special symbol that performs an operation on one or more values (operands).

In simple words,

> Operators tell JavaScript what operation should be performed.

Example

```javascript
let a = 10;
let b = 5;

console.log(a + b);
```

Output

```
15
```

Here,

* `+` is the operator.
* `10` and `5` are operands.

---

# Real World Example

Imagine you are using a calculator.

```
10 + 5
```

The `+` button tells the calculator to add two numbers.

Similarly,

JavaScript operators perform operations like:

* Addition
* Subtraction
* Comparison
* Assignment
* Logical Operations
* Increment
* Decrement

---

# Types of Operators

JavaScript provides several types of operators.

1. Arithmetic Operators
2. Assignment Operators
3. Comparison Operators
4. Logical Operators
5. Increment & Decrement Operators
6. Ternary Operator

---

# 1. Arithmetic Operators

Arithmetic operators are used to perform mathematical calculations.

| Operator | Meaning             |
| -------- | ------------------- |
| +        | Addition            |
| -        | Subtraction         |
| *        | Multiplication      |
| /        | Division            |
| %        | Modulus (Remainder) |
| **       | Exponent (Power)    |

---

## Addition (+)

Adds two numbers.

Syntax

```javascript
value1 + value2
```

Example

```javascript
let a = 20;
let b = 10;

console.log(a + b);
```

Output

```
30
```

---

## Subtraction (-)

Subtracts one value from another.

```javascript
let a = 20;
let b = 10;

console.log(a - b);
```

Output

```
10
```

---

## Multiplication (*)

```javascript
let a = 5;
let b = 6;

console.log(a * b);
```

Output

```
30
```

---

## Division (/)

```javascript
let a = 20;
let b = 5;

console.log(a / b);
```

Output

```
4
```

---

## Modulus (%)

Returns the remainder after division.

Example

```javascript
console.log(10 % 3);
```

Output

```
1
```

Explanation

```
10 ÷ 3 = 3

3 × 3 = 9

10 - 9 = 1
```

So,

```
Remainder = 1
```

---

## Exponent (**)

Calculates the power of a number.

```javascript
console.log(2 ** 3);
```

Output

```
8
```

Meaning

```
2 × 2 × 2
```

---

# Arithmetic Example

```javascript
let a = 15;
let b = 4;

console.log(a + b);
console.log(a - b);
console.log(a * b);
console.log(a / b);
console.log(a % b);
```

Output

```
19
11
60
3.75
3
```

---

# 2. Assignment Operators

Assignment operators assign values to variables.

| Operator | Meaning             |
| -------- | ------------------- |
| =        | Assign              |
| +=       | Add and Assign      |
| -=       | Subtract and Assign |
| *=       | Multiply and Assign |
| /=       | Divide and Assign   |
| %=       | Modulus and Assign  |

---

## =

```javascript
let age = 20;
```

---

## +=

```javascript
let marks = 50;

marks += 10;

console.log(marks);
```

Output

```
60
```

Equivalent to

```javascript
marks = marks + 10;
```

---

## -=

```javascript
let marks = 80;

marks -= 20;

console.log(marks);
```

Output

```
60
```

---

## *=

```javascript
let value = 5;

value *= 4;

console.log(value);
```

Output

```
20
```

---

## /=

```javascript
let value = 40;

value /= 5;

console.log(value);
```

Output

```
8
```

---

## %=

```javascript
let value = 25;

value %= 7;

console.log(value);
```

Output

```
4
```

---

# 3. Comparison Operators

Comparison operators compare two values.

The result is always

```
true

or

false
```

| Operator | Meaning               |
| -------- | --------------------- |
| ==       | Equal                 |
| ===      | Strict Equal          |
| !=       | Not Equal             |
| !==      | Strict Not Equal      |
| >        | Greater Than          |
| <        | Less Than             |
| >=       | Greater Than or Equal |
| <=       | Less Than or Equal    |

---

## == (Loose Equality)

Checks only values.

```javascript
console.log(10 == "10");
```

Output

```
true
```

Because JavaScript converts the string into a number.

---

## === (Strict Equality)

Checks both value and data type.

```javascript
console.log(10 === "10");
```

Output

```
false
```

Number is different from String.

---

## !=

```javascript
console.log(10 != 5);
```

Output

```
true
```

---

## !==

```javascript
console.log(10 !== "10");
```

Output

```
true
```

---

## Greater Than

```javascript
console.log(20 > 10);
```

Output

```
true
```

---

## Less Than

```javascript
console.log(20 < 10);
```

Output

```
false
```

---

## Greater Than or Equal

```javascript
console.log(50 >= 50);
```

Output

```
true
```

---

## Less Than or Equal

```javascript
console.log(20 <= 30);
```

Output

```
true
```

---

# Difference Between == and ===

| ==                         | ===                   |
| -------------------------- | --------------------- |
| Checks only value          | Checks value and type |
| Performs type conversion   | No type conversion    |
| Less strict                | More strict           |
| Avoid in modern JavaScript | Recommended           |

Example

```javascript
console.log(5 == "5");
```

Output

```
true
```

```javascript
console.log(5 === "5");
```

Output

```
false
```

**Best Practice:** Always prefer `===` and `!==` to avoid unexpected type conversion.

---

# 4. Logical Operators

Logical operators combine multiple conditions.

| Operator | Meaning |
| -------- | ------- |
| &&       | AND     |
| ||       | OR      |
| !        | NOT     |

---

## AND (&&)

Returns `true` only if **all conditions are true**.

Truth Table

| A     | B     | Result |
| ----- | ----- | ------ |
| true  | true  | true   |
| true  | false | false  |
| false | true  | false  |
| false | false | false  |

Example

```javascript
let age = 22;
let hasLicense = true;

console.log(age >= 18 && hasLicense);
```

Output

```
true
```

---

## OR (||)

Returns `true` if **at least one condition is true**.

Truth Table

| A     | B     | Result |
| ----- | ----- | ------ |
| true  | true  | true   |
| true  | false | true   |
| false | true  | true   |
| false | false | false  |

Example

```javascript
let isHoliday = false;
let isSunday = true;

console.log(isHoliday || isSunday);
```

Output

```
true
```

---

## NOT (!)

Reverses a boolean value.

```javascript
console.log(!true);
console.log(!false);
```

Output

```
false
true
```

---

# Operator Precedence

JavaScript follows the **BODMAS** rule.

Priority

1. `()`
2. `**`
3. `* / %`
4. `+ -`
5. Comparison Operators
6. Logical Operators

Example

```javascript
console.log(10 + 5 * 2);
```

Output

```
20
```

Explanation

```
5 × 2 = 10

10 + 10 = 20
```

---

# Increment Operator (++)

Increases the value by **1**.

```javascript
let count = 5;

count++;

console.log(count);
```

Output

```
6
```

---

## Pre Increment

```javascript
let a = 5;

console.log(++a);
```

Output

```
6
```

---

## Post Increment

```javascript
let a = 5;

console.log(a++);
console.log(a);
```

Output

```
5
6
```

---

# Decrement Operator (--)

Decreases the value by **1**.

```javascript
let count = 10;

count--;

console.log(count);
```

Output

```
9
```

---

## Pre Decrement

```javascript
let a = 10;

console.log(--a);
```

Output

```
9
```

---

## Post Decrement

```javascript
let a = 10;

console.log(a--);
console.log(a);
```

Output

```
10
9
```

---

# Ternary Operator

The ternary operator is a **short form of the `if...else` statement**. It evaluates a condition and returns one value if the condition is `true`, otherwise it returns another value.

### Syntax

```javascript
condition ? valueIfTrue : valueIfFalse;
```

---

### Example

```javascript
let age = 20;

let result = age >= 18 ? "Eligible to Vote" : "Not Eligible";

console.log(result);
```

Output

```
Eligible to Vote
```

---

### Another Example

```javascript
let marks = 45;

let result = marks >= 35 ? "Pass" : "Fail";

console.log(result);
```

Output

```
Pass
```

---

# Common Beginner Mistakes

❌ Using `=` instead of `==` or `===`.

Wrong

```javascript
if (age = 18)
```

Correct

```javascript
if (age === 18)
```

---

❌ Using `==` when strict comparison is needed.

```javascript
5 == "5"
```

Better

```javascript
5 === "5"
```

---

❌ Forgetting operator precedence.

Wrong assumption

```javascript
10 + 5 * 2 = 30
```

Correct

```
10 + (5 × 2) = 20
```

---

❌ Confusing pre-increment and post-increment.

```javascript
let a = 5;

console.log(a++);
```

Output

```
5
```

Many beginners expect `6`, but `a++` returns the current value first and increments afterward.

---

# Memory Tips

### Arithmetic

```
+  Add

-  Subtract

*  Multiply

/  Divide

%  Remainder

** Power
```

---

### Comparison

```
==   Value

===  Value + Type

!=   Not Equal

!==  Strict Not Equal
```

---

### Logical

```
&&

Both True

||

Any One True

!

Reverse Boolean
```

---

# Interview Questions

1. What is an operator in JavaScript?
2. What are operands?
3. Explain arithmetic operators.
4. What is the difference between `%` and `/`?
5. What is the purpose of assignment operators?
6. Explain the difference between `==` and `===`.
7. Why is `===` recommended over `==`?
8. What are logical operators?
9. Explain the truth table of `&&` and `||`.
10. What is the difference between pre-increment and post-increment?
11. What is operator precedence?
12. What is the ternary operator?
13. When should you use the ternary operator?
14. What does `!true` return?
15. What is the output of `10 + 5 * 2` and why?

---

# Practice Programs

### Program 1 - Arithmetic Operations

```javascript
let a = 12;
let b = 5;

console.log("Addition:", a + b);
console.log("Subtraction:", a - b);
console.log("Multiplication:", a * b);
console.log("Division:", a / b);
console.log("Remainder:", a % b);
```

---

### Program 2 - Assignment Operators

```javascript
let marks = 50;

marks += 20;
marks -= 5;
marks *= 2;
marks /= 5;

console.log(marks);
```

---

### Program 3 - Comparison Operators

```javascript
let x = 25;
let y = "25";

console.log(x == y);
console.log(x === y);
console.log(x != y);
console.log(x !== y);
```

---

### Program 4 - Logical Operators

```javascript
let age = 22;
let hasLicense = true;

console.log(age >= 18 && hasLicense);
console.log(age >= 18 || hasLicense);
console.log(!hasLicense);
```

---

### Program 5 - Increment & Decrement

```javascript
let count = 10;

console.log(count++);
console.log(count);

console.log(++count);

console.log(count--);
console.log(count);

console.log(--count);
```

---

### Program 6 - Ternary Operator

```javascript
let temperature = 32;

let weather = temperature > 30 ? "Hot Day" : "Pleasant Day";

console.log(weather);
```

---

### Program 7 - Mixed Operators

```javascript
let num1 = 15;
let num2 = 4;

let result = (num1 + num2) * 2 > 30 && num1 % num2 !== 0;

console.log(result);
```
---
# Day 1 - JavaScript Fundamentals (Part 3)

# Conditional Statements

---

# What are Conditional Statements?

A **Conditional Statement** is used to make decisions in a program.

It allows JavaScript to execute different blocks of code depending on whether a condition is **true** or **false**.

In simple words,

> Conditional statements help the program decide **what to do next**.

---

# Real World Example

Imagine you are logging into a website.

```text
Enter Username
        │
        ▼
Enter Password
        │
        ▼
Password Correct?
      /      \
    Yes       No
    │          │
    ▼          ▼
 Login     Show Error
```

The decision is based on a **condition**.

---

# Why do we need Conditional Statements?

Without Conditions

```javascript
console.log("You can vote.");
```

The message is printed for everyone.

With Conditions

```javascript
let age = 20;

if(age >= 18){
    console.log("You can vote.");
}
```

Now the message is displayed only when the condition is true.

---

# Types of Conditional Statements

JavaScript provides the following conditional statements.

* if
* if...else
* else if
* Nested if
* switch
* Ternary Operator (Already Learned)

---

# if Statement

The **if** statement executes a block of code only when the condition is **true**.

---

## Syntax

```javascript
if(condition){
    // Code
}
```

---

## Flow

```text
Condition
   │
 ┌─┴─────┐
 │ True  │
 ▼        │
Execute   │
 Code     │
 │         │
 └─────────┘
```

---

## Example

```javascript
let age = 20;

if(age >= 18){
    console.log("Eligible to Vote");
}
```

Output

```text
Eligible to Vote
```

---

## Example 2

```javascript
let marks = 80;

if(marks >= 35){
    console.log("Pass");
}
```

Output

```text
Pass
```

---

# if...else Statement

If the condition is true,

execute one block.

Otherwise,

execute another block.

---

## Syntax

```javascript
if(condition){

}

else{

}
```

---

## Flow

```text
Condition
    │
 ┌──┴─────┐
 │ True   │ False
 ▼         ▼
Block 1  Block 2
```

---

## Example

```javascript
let age = 15;

if(age >= 18){
    console.log("Eligible");
}
else{
    console.log("Not Eligible");
}
```

Output

```text
Not Eligible
```

---

## Example

```javascript
let number = 10;

if(number % 2 == 0){
    console.log("Even Number");
}
else{
    console.log("Odd Number");
}
```

Output

```text
Even Number
```

---

# else if Statement

Used when there are **multiple conditions**.

---

## Syntax

```javascript
if(condition1){

}
else if(condition2){

}
else{

}
```

---

## Example

```javascript
let marks = 82;

if(marks >= 90){
    console.log("Grade A+");
}
else if(marks >= 75){
    console.log("Grade A");
}
else if(marks >= 60){
    console.log("Grade B");
}
else if(marks >= 35){
    console.log("Grade C");
}
else{
    console.log("Fail");
}
```

Output

```text
Grade A
```

---

# Real World Example

ATM Machine

```text
Balance > ₹5000
        │
      Yes
        │
Premium Customer

Otherwise

Regular Customer
```

---

# Nested if Statement

An **if statement inside another if statement** is called a Nested if.

---

## Syntax

```javascript
if(condition1){

    if(condition2){

    }

}
```

---

## Example

```javascript
let age = 20;
let hasLicense = true;

if(age >= 18){

    if(hasLicense){
        console.log("You Can Drive");
    }

}
```

Output

```text
You Can Drive
```

---

## Example 2

```javascript
let username = "admin";
let password = "12345";

if(username == "admin"){

    if(password == "12345"){
        console.log("Login Success");
    }
    else{
        console.log("Wrong Password");
    }

}
else{
    console.log("Invalid User");
}
```

Output

```text
Login Success
```

---

# switch Statement

The **switch statement** is used when there are multiple possible values for one variable.

It is cleaner than writing many `else if` statements.

---

## Syntax

```javascript
switch(expression){

case value:

    code;

    break;

default:

    code;

}
```

---

## Flow

```text
Expression
     │
 ┌───┼──────────────┐
 │   │              │
Case1 Case2      Default
```

---

## Example

```javascript
let day = 3;

switch(day){

case 1:
console.log("Monday");
break;

case 2:
console.log("Tuesday");
break;

case 3:
console.log("Wednesday");
break;

default:
console.log("Invalid");
}
```

Output

```text
Wednesday
```

---

## Example

```javascript
let color = "Red";

switch(color){

case "Blue":
console.log("Blue Color");
break;

case "Green":
console.log("Green Color");
break;

case "Red":
console.log("Red Color");
break;

default:
console.log("Unknown");
}
```

Output

```text
Red Color
```

---

# Importance of break

Without `break`, JavaScript continues executing the remaining cases.

Example

```javascript
let day = 2;

switch(day){

case 1:
console.log("Monday");

case 2:
console.log("Tuesday");

case 3:
console.log("Wednesday");

}
```

Output

```text
Tuesday
Wednesday
```

---

Correct Version

```javascript
let day = 2;

switch(day){

case 1:
console.log("Monday");
break;

case 2:
console.log("Tuesday");
break;

case 3:
console.log("Wednesday");
break;

}
```

Output

```text
Tuesday
```

---

# if vs switch

| if                    | switch                  |
| --------------------- | ----------------------- |
| Works with conditions | Works with values       |
| More flexible         | Cleaner for many values |
| Used for ranges       | Used for exact matches  |

---

# LOOPS

---

# What is a Loop?

A **Loop** is used to execute the same block of code multiple times.

Instead of writing the same code repeatedly,

we use loops.

---

# Real World Example

Suppose you need to print

```text
Welcome
```

100 times.

Without Loop

```javascript
console.log("Welcome");
console.log("Welcome");
console.log("Welcome");
```

100 lines...

With Loop

```javascript
for(let i=1;i<=100;i++){

console.log("Welcome");

}
```

---

# Types of Loops

* for
* while
* do...while
* Nested Loop

---

# for Loop

The **for loop** is used when we know how many times the loop should execute.

---

## Syntax

```javascript
for(initialization; condition; increment){

}
```

---

## Parts of for Loop

```text
Initialization

↓

Condition

↓

Code Executes

↓

Increment

↓

Condition Again
```

---

## Flow Diagram

```text
Start
  │
Initialization
  │
Condition
  │
True
  │
Code
  │
Increment
  │
Condition Again
  │
False
  ▼
Stop
```

---

## Example

```javascript
for(let i=1;i<=5;i++){

console.log(i);

}
```

Output

```text
1
2
3
4
5
```

---

## Print Even Numbers

```javascript
for(let i=2;i<=20;i+=2){

console.log(i);

}
```

Output

```text
2
4
6
8
10
12
14
16
18
20
```

---

## Print Odd Numbers

```javascript
for(let i=1;i<=19;i+=2){

console.log(i);

}
```

---

# while Loop

The **while loop** executes as long as the condition remains true.

---

## Syntax

```javascript
while(condition){

}
```

---

## Example

```javascript
let i=1;

while(i<=5){

console.log(i);

i++;

}
```

Output

```text
1
2
3
4
5
```

---

# do...while Loop

The **do...while** loop executes the block **at least once**, even if the condition is false.

---

## Syntax

```javascript
do{

}
while(condition);
```

---

## Example

```javascript
let i=1;

do{

console.log(i);

i++;

}
while(i<=5);
```

Output

```text
1
2
3
4
5
```

---

## Difference

```javascript
let i=10;

while(i<=5){

console.log(i);

}
```

Output

```text
Nothing Printed
```

---

```javascript
let i=10;

do{

console.log(i);

}
while(i<=5);
```

Output

```text
10
```

---

# break Statement

Used to stop a loop immediately.

---

## Example

```javascript
for(let i=1;i<=10;i++){

if(i==6){

break;

}

console.log(i);

}
```

Output

```text
1
2
3
4
5
```

---

# continue Statement

Skips the current iteration.

---

## Example

```javascript
for(let i=1;i<=5;i++){

if(i==3){

continue;

}

console.log(i);

}
```

Output

```text
1
2
4
5
```

---

# Nested Loop

A loop inside another loop.

---

## Example

```javascript
for(let i=1;i<=3;i++){

for(let j=1;j<=3;j++){

console.log(i,j);

}

}
```

Output

```text
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2
3 3
```

---

# Multiplication Table

```javascript
let number=5;

for(let i=1;i<=10;i++){

console.log(number+" x "+i+" = "+number*i);

}
```

Output

```text
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
...
5 x 10 = 50
```

---

# Sum of Numbers

```javascript
let sum=0;

for(let i=1;i<=10;i++){

sum+=i;

}

console.log(sum);
```

Output

```text
55
```

---

# Factorial Program

```javascript
let fact=1;

for(let i=1;i<=5;i++){

fact*=i;

}

console.log(fact);
```

Output

```text
120
```

---

# Common Beginner Mistakes

❌ Forgetting braces `{}`

```javascript
if(age>=18)
console.log("Eligible");
```

Although valid for a single statement, always use braces for better readability.

---

❌ Using `=` instead of `===`

Wrong

```javascript
if(age=18)
```

Correct

```javascript
if(age===18)
```

---

❌ Infinite Loop

```javascript
let i=1;

while(i<=5){

console.log(i);

}
```

`i` is never incremented, so the loop runs forever.

Correct

```javascript
let i=1;

while(i<=5){

console.log(i);

i++;

}
```

---

❌ Forgetting `break` in `switch`

Without `break`, execution falls through to the next case.

---

# Memory Tips

### Conditional Statements

```text
if
↓

One Condition

if...else
↓

Two Choices

else if
↓

Many Conditions

switch
↓

Many Values
```

---

### Loops

```text
for

Know Number of Iterations

while

Condition First

do...while

Runs At Least Once
```

---

### Loop Control Statements

```text
break

↓

Stop Loop

continue

↓

Skip Current Iteration
```

---

# Interview Questions

1. What is a conditional statement?
2. What is the difference between `if` and `if...else`?
3. When should you use `else if`?
4. What is a nested `if`?
5. What is a `switch` statement?
6. Why is `break` important in a `switch` statement?
7. Difference between `if` and `switch`?
8. What is a loop?
9. Difference between `for`, `while`, and `do...while`?
10. What is an infinite loop?
11. What is the difference between `break` and `continue`?
12. What is a nested loop?
13. How do you print a multiplication table using a loop?
14. How do you calculate the sum of numbers using a loop?
15. How do you calculate the factorial of a number?

---

# Practice Programs

### Program 1 - Check Positive or Negative

```javascript
let number = -10;

if(number >= 0){
    console.log("Positive");
}
else{
    console.log("Negative");
}
```

---

### Program 2 - Grade Calculator

```javascript
let marks = 88;

if(marks >= 90){
    console.log("A+");
}
else if(marks >= 75){
    console.log("A");
}
else if(marks >= 60){
    console.log("B");
}
else if(marks >= 35){
    console.log("C");
}
else{
    console.log("Fail");
}
```

---

### Program 3 - Day Using Switch

```javascript
let day = 5;

switch(day){
    case 1: console.log("Monday"); break;
    case 2: console.log("Tuesday"); break;
    case 3: console.log("Wednesday"); break;
    case 4: console.log("Thursday"); break;
    case 5: console.log("Friday"); break;
    case 6: console.log("Saturday"); break;
    case 7: console.log("Sunday"); break;
    default: console.log("Invalid Day");
}
```

---

### Program 4 - Print Numbers 1 to 20

```javascript
for(let i = 1; i <= 20; i++){
    console.log(i);
}
```

---

### Program 5 - Print Even Numbers

```javascript
for(let i = 2; i <= 20; i += 2){
    console.log(i);
}
```

---

### Program 6 - Multiplication Table

```javascript
let number = 7;

for(let i = 1; i <= 10; i++){
    console.log(`${number} x ${i} = ${number * i}`);
}
```

---

### Program 7 - Sum of First 100 Numbers

```javascript
let sum = 0;

for(let i = 1; i <= 100; i++){
    sum += i;
}

console.log(sum);
```

---

### Program 8 - Factorial

```javascript
let fact = 1;

for(let i = 1; i <= 6; i++){
    fact *= i;
}

console.log(fact);
```

---

### Program 9 - Break Example

```javascript
for(let i = 1; i <= 10; i++){

    if(i === 7){
        break;
    }

    console.log(i);
}
```

---

### Program 10 - Continue Example

```javascript
for(let i = 1; i <= 10; i++){

    if(i === 5){
        continue;
    }

    console.log(i);
}
```

---
