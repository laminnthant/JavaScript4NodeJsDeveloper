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
    *Multi-line* comments start with `/*` and end with `*/`:
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
        - Number literals: `10, 3.14, -5`
        - String literals: `"Hello, world!"`, `'Single quotes also work'`
        - Boolean literals: `true`, `false`
        - Null literal: `null`
        - Undefined literal: `undefined`

2. **Identifier Expressions:**
    Refer to variables or function names that hold values.
    - **Examples:** `userAge`, `fullName`

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

### Introduction

**Data types** define the kind of information a variable can hold and the operations that can be performed on it.JavaScript has two main categories of data type , primitive data type and non-primitive data type(reference type).
 
#### 1. Primitive Data Types

    Simple , indivisible values stored directly in memory.

1. **Number:**

    Represents numeric values including `integer` and `floating point`.
    - Integer (`10, -5, 0`)
    - Floating-point (`3.14, 2.5e-3`)
    - Examples:
    ```let age = 30;
     let pi = 3.14159;
    ```
2. **String:**

    Represents a sequence of characters enclosed in single or double quotes.
    - Examples:
    ```
    let name = "Alice";
    let greeting = 'Hell0, Alice!';
    ```
3. **Boolean:**

    Represents logical values : `true` or `false`.
    - Examples:
    ```
    let isLoggedIn = true;
    let isLoading = false;
    ```
4. **Null:**

    Represents the intentional absence of a value.
    - Example:
    ```
    let middleName = null;
    ```
5. **Undefined:**

    Indicates a declared variable has not been assigned a value.
    - Example:
    ```
    let uninitializedVariable ; // Undefined by Default
    ```
6. **Symbol:**

    Introduced in ECMAScript 6 (ES6), symbols are unique and immutable primitive.
    You use the `Symbol()` function to create a Symbol.
    - Example:
    ```
    let sym = Symbol('Hello, symbol');
    console.log(sym); // Symbol(Hello, symbol);
    ```

#### 2. Non-Primitive Data Types(Reference Types,Object Types)

    Store references to memory locations where the actual values are stored.

1. **Objects:**

    Represents a collection of key-value pairs (properties).It is a fundamental data structure in JavaScript.
    - Example:
    ```
    let person {
        name: "Alice",
        age: 30,
        isStudent: false
    }
    ```
2. **Arrays:**

    Represents an ordered list of values and uses zero-based indexing.
    - Example:
    ```
    let number = [ 1, 2, 3, 4, 5];
    ```
3. **Functions:**

    Represents  a reusable block of code that perform specific tasks.
    - Example:
    ```
    function greet(name) {
        comsole.log('Hello, '+ name + '!');
    }
    greet('Alice'); // Hello, Alice
    ```
### Key Points:

- Understanding data types is essential for writing accurate and predictable JavaScript code.
- Choose appropriate data types based on the nature of the data you're working with.
- JavaScript's dynamic typing means you don't need to explicitly declare data types, but it's often good    practice for clarity and error prevention.

1. [Lexical Structure](Lexicalstructure.md)
2. [Expressions](Expressions.md)