# JavaScript for NodeJs Developer Should Know
## 1. Lexical Structure
### Introduction

**Lexical structure** defines the basic rules for writing JavaScript code, forming the foundation for its syntax. It's essential to understand these rules to write valid and effective JavaScript programs.

### Key Concepts

1. **Case Sensitivity:**

    JavaScript distinguishes between uppercase and lowercase letters.
    `myVariable` is different from `MyVariable` and `myvariable`.

2. **Spaces and Line Breaks:**

    *Spaces and line breaks* are used for readability but are generally ignored by the interpreter.

3. **Comments:**

    *Single-line* comments start with `//` and extend to the end of the line:
```
//this is a single line comment
```
Multi-line comments start with `/*` and end with `*/`:
```
/*This is a multiline comment*/
```
4. **Literals:**

    - *Literals* represent fixed values directly in the code.
    - **Types of literals:**
        - Numbers: `123, 4.56, -789`
        - Strings: `"Hello, world!"`, `'Single quotes also work'`
        - Booleans: `true`, `false`
        - Null: `null`
        - Undefined: `undefined`
        - Regular expressions: `/\d{3}-\d{3}-\d{4}/`

5. **Identifiers and Reserved Words:**

    - Identifiers are names for variables, functions, objects, etc.
        - Start with a letter, underscore (`_`), or dollar sign (`$`)
        - Can contain letters, digits, underscores, and dollar signs
    - Reserved words have special meanings and cannot be used as identifiers.
        - Examples: `if`, `else`,`for`, `while`, `function`, `var`, `let`, `const`, `true`, `false`, `null`

6. **Unicode:**

    JavaScript supports Unicode characters for internationalization.

7. **Optional Semicolons:**

    Semicolons are typically used to terminate statements, but they're often optional.
    Good practice to use them for clarity and error prevention.

### CodeExample

```
let age = 30;   // Number literal
let name = "John"; // String literal
let isStudent = true; // Boolean literal
let address = null;  // null literal

function greet(person) {  // Identifier for function name
  if (person.age >= 18) {  // Reserved words: if, else
    console.log("Hello, " + person.name + ". You are an adult."); // String concatenation
  } else {
    console.log("Hello, " + person.name + ". You are a minor.");
  }
}

greet({ name: "Alice", age: 25 }); // Object literal

```
### Key points
- Adhere to these lexical rules to write valid JavaScript code.
- Understanding lexical structure is essential for interpreting and writing JavaScript effectively.

## 2. Expressions
### Introduction
- Expressions are the fundamental building blocks of JavaScript code that produce values.
- They are comprised of values, variables, operators, and function calls.
- The JavaScript engine evaluates expressions and returns a resulting value.

### Types of Expressions:

1. **Literal Expressions:**
    Represent fixed values directly in the code.
- **Examples**
    - Number literals: 10, 3.14, -5
    - String literals: "Hello, world!", 'Single quotes also work'
    - Boolean literals: true, false
    - Null literal: null
    - Undefined literal: undefined

2. **Identifier Expressions:**
    Refer to variables or function names that hold values.
**Examples:** `userAge`, `fullName`

3. **Operator Expressions:**
    Combine values using operators to produce new values.
- **Examples:**
    - Arithmetic operators: `+`, `-`, `*`, `/`, `%`
    - Comparison operators: `==`, `!=`, `<`, `>`,` <=`, `>=`
    - Logical operators: `&& `(and), `|| `(or),` ! `(not)

4. **Function Call Expressions:**
    Invoke a function and return its result.
- **Examples:** `Math.sqrt(16)`, `calculateArea(4, 5)`

5. **Object Expressions:**
    Create objects using curly braces `{}`.
- **Example:** `let person = { name: "John", age: 30 }`

6. **Array Expressions:**
    Create arrays using square brackets `[]`.
- **Example:** `let numbers = [1, 2, 3, 4, 5]`

7. **Assignment Expressions:**
    Assign a value to a variable using the `=` operator.
- **Example:** `let x = 10`

### Code Examples:
```
// Literal expressions
let age = 30;
let message = "Greetings!";

// Identifier expressions
let userName = "Alice";

// Operator expressions
let result = 5 + 3; // result will be 8
let isEven = number % 2 === 0;

// Function call expressions
let area = calculateArea(10, 5);

// Object and array expressions
let person = { name: "Bob", age: 25 };
let colors = ["red", "green", "blue"];

// Assignment expressions
let x = 10 + 5; // x will be assigned the value 15
```

### Key Points:

- Expressions are evaluated to produce values, while statements perform actions.
- Expressions can be nested within other expressions, forming complex calculations and logic.
- Understanding expressions is essential for writing meaningful and effective JavaScript code.

## 3. Data Types

1. [Lexical Structure](Lexicalstructure.md)
2. [Expressions](Expressions.md)