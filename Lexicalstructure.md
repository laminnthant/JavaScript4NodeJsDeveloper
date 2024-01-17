# Understanding JavaScript's Lexical Structure
## Introduction

Lexical structure defines the basic rules for writing JavaScript code, forming the foundation for its syntax. It's essential to understand these rules to write valid and effective JavaScript programs.

## Key Concepts

1. Case Sensitivity:

    JavaScript distinguishes between uppercase and lowercase letters.
    myVariable is different from MyVariable and myvariable.

2. Spaces and Line Breaks:

    Spaces and line breaks are used for readability but are generally ignored by the interpreter.

3. Comments:

    Single-line comments start with // and extend to the end of the line:
```
//this is a single line comment
```
Multi-line comments start with /* and end with */:
```
/*This is a multiline comment*/
```
4. Literals:

    Literals represent fixed values directly in the code.
    Types of literals:
        Numbers: 123, 4.56, -789
        Strings: "Hello, world!", 'Single quotes also work'
        Booleans: true, false
        Null: null
        Undefined: undefined
        Regular expressions: /\d{3}-\d{3}-\d{4}/

5. Identifiers and Reserved Words:

    Identifiers are names for variables, functions, objects, etc.
    Start with a letter, underscore (_), or dollar sign ($)
    Can contain letters, digits, underscores, and dollar signs
    Reserved words have special meanings and cannot be used as identifiers.
    Examples: if, else, for, while, function, var, let, const, true, false, null

6. Unicode:

    JavaScript supports Unicode characters for internationalization.

7. Optional Semicolons:

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
## Key Points:

    Adhere to these lexical rules to write valid JavaScript code.
    Understanding lexical structure is essential for interpreting and writing JavaScript effectively.
