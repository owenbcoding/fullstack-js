# 03 – JavaScript Functions & Scope

These notes gather all of your function‑related content (and closely related scope concepts) from `Full Stack | Js interactive websites` into a single, organized file.

---

## What Are Functions?

A **function** is a reusable block of code that groups together a sequence of statements to perform a specific task.

```jsx
function greetWorld() {
  console.log("Hello, World!");
}
```

- `function` – keyword that starts a function declaration.
- `greetWorld` – function **name** (identifier).
- `()` – parameter list (empty here).
- `{ ... }` – function body (code that runs when the function is called).

You **call** (invoke) a function by writing its name followed by parentheses:

```jsx
greetWorld(); // "Hello, World!"
```

> **Hoisting** – function declarations are hoisted, which means you can technically call them before they appear in the file. It’s usually better style to declare functions before using them.

---

## Calling Functions

When you call a function:

1. Execution jumps into the function body.
2. Statements run line by line.
3. Control returns to where the function was called.

You can call the same function as many times as needed:

```jsx
function sayHi() {
  console.log("Hi!");
}

sayHi(); // "Hi!"
sayHi(); // "Hi!"
```

---

## Parameters & Arguments

Functions can take **inputs** called **parameters** and use them to perform work.

```jsx
function greet(name) {
  console.log(`Hello, ${name}!`);
}

greet("Owen");   // "Hello, Owen!"
greet("Sam");    // "Hello, Sam!"
```

- **Parameters** – names listed in the function definition (`name`).
- **Arguments** – actual values passed when calling the function (`"Owen"`, `"Sam"`).

The order of arguments must match the order of parameters.

```jsx
function rectangleArea(width, height) {
  return width * height;
}

const area1 = rectangleArea(10, 6); // width=10, height=6
const area2 = rectangleArea(4, 3);  // width=4, height=3
```

---

## Default Parameters (ES6)

Default parameters allow you to specify a **fallback value** when no argument is passed (or it’s `undefined`).

```jsx
function greeting(name = "stranger") {
  console.log(`Hello, ${name}!`);
}

greeting("Nick"); // "Hello, Nick!"
greeting();       // "Hello, stranger!"
```

If the caller provides an argument, it **overrides** the default.

---

## Return Values

Functions can **return** values using the `return` keyword. This:

- Ends execution of the function body immediately.
- Sends a value back to the caller.

```jsx
function rectangleArea(width, height) {
  if (width < 0 || height < 0) {
    return "You need positive integers to calculate area!";
  }
  return width * height;
}

const result = rectangleArea(5, 3); // 15
```

Any code after a `return` in the same block **will not execute**.

Returned values are often stored in variables:

```jsx
function add(a, b) {
  return a + b;
}

const sum = add(2, 3); // 5
```

---

## Helper Functions

You can call a function **inside another function**. When a function is used to support another, we often call it a **helper function**.

```jsx
function multiplyByNineFifths(number) {
  return number * (9 / 5);
}

function getFahrenheit(celsius) {
  return multiplyByNineFifths(celsius) + 32;
}

getFahrenheit(15); // 59
```

Breaking a large problem into smaller functions:

- Makes your code easier to understand.
- Makes it easier to test and debug.
- Encourages reuse.

---

## Function Expressions

Functions can also be created as **expressions** and stored in variables.

```jsx
const greet = function (name) {
  return `Hello, ${name}!`;
};

console.log(greet("Owen")); // "Hello, Owen!"
```

- This is called a **function expression**.
- If the function has **no name**, it’s an **anonymous** function expression.

```jsx
const greetAnon = function (name) {
  return `Hello, ${name}!`;
};

const greetNamed = function sayHello(name) {
  return `Hello, ${name}!`;
};
```

> **Important:** Function expressions are **not hoisted** the way declarations are, so you cannot call them before the line where they’re defined.

---

## Arrow Functions

ES6 introduced **arrow functions**, a shorter syntax for function expressions.

```jsx
// Regular function expression
const rectangleArea = function (width, height) {
  return width * height;
};

// Arrow function
const rectangleAreaArrow = (width, height) => {
  return width * height;
};
```

For very short functions, you can use a **concise body**:

```jsx
// Long form
const greaterThanFive = (num) => {
  return num > 5 ? true : false;
};

// Concise form
const greaterThanFiveConcise = num => num > 5 ? true : false;
```

Concise arrow functions:

- Omit parentheses when there is **one parameter**.
- Omit curly braces and `return` when the body is a **single expression**.

Arrow functions are very common in modern JS, especially with array methods and React.

---

## Scope

**Scope** defines where variables can be **accessed** or **referenced** in your program.

You can think of:

- **Global scope** – variables visible “everywhere”.
- **Block / local scope** – variables visible only inside a specific block or function.

### Blocks

A **block** is any code wrapped in `{}`.

```jsx
const logSkyColor = () => {
  let color = "blue";
  console.log(color); // "blue"
};
```

Another example:

```jsx
const city = "New York City";

const logCitySkyline = () => {
  let skyscraper = "Empire State Building";
  return "The stars over the " + skyscraper + " in " + city;
};

console.log(logCitySkyline());
// "The stars over the Empire State Building in New York City"
```

---

## Global Scope

Variables declared **outside** of any function or block are in **global scope** and are accessible anywhere.

```jsx
const satellite = "The Moon";
const galaxy = "The Milky Way";
const stars = "North Star";

const callMyNightSky = () => {
  return "Night Sky: " + satellite + ", " + stars + ", and " + galaxy;
};

console.log(callMyNightSky());
// "Night Sky: The Moon, North Star, and The Milky Way"
```

Global variables live for the lifetime of the program and can be read from any function, which can be convenient but also risky.

---

## Block (Local) Scope

Variables declared with `let` or `const` **inside** a block are only available **inside that block**. They are often called **local variables**.

```jsx
const logVisibleLightWaves = () => {
  const lightWaves = "Moonlight";
  console.log(lightWaves); // OK
};

logVisibleLightWaves();
// console.log(lightWaves); // ❌ ReferenceError: lightWaves is not defined
```

Block scope helps prevent variables from leaking into other parts of your program.

---

## Scope Pollution

**Scope pollution** happens when:

- You create too many global variables.
- You reuse variable names across different scopes carelessly.

Problems it can cause:

- It becomes hard to track where and how variables are changed.
- Variables in different parts of the code accidentally overwrite each other.

Better practice:

- Keep variables as **local** as possible.
- Avoid unnecessary globals.
- Use meaningful, specific names.

---

## Good Scoping Practice – Example

```jsx
const logVisibleLightWaves = () => {
  let lightWaves = "Moonlight";
  let region = "The Arctic";

  if (region === "The Arctic") {
    let lightWaves = "Northern Lights";
    console.log(lightWaves); // "Northern Lights"
  }

  console.log(lightWaves); // "Moonlight"
};

logVisibleLightWaves();
```

Here:

- The inner `lightWaves` in the `if` block **shadows** the outer one.
- We keep variables tightly scoped, which makes it clear which value is which.

---

## Quick Review – Functions & Scope

- A **function declaration** uses `function name(...) { ... }` and is hoisted.
- **Function expressions** assign a function to a variable; they are **not** hoisted.
- **Arrow functions** provide shorter syntax and are heavily used in modern JS.
- **Parameters** define what data a function expects; **arguments** are the actual values passed in.
- Use `return` to send values back from functions and stop execution of the function body.
- **Helper functions** break complex problems into simpler, reusable pieces.
- **Scope** determines where variables are visible:
  - **Global scope** – visible everywhere.
  - **Block / local scope** – visible only inside a block or function.
- Avoid **scope pollution** by limiting global variables and using tight, clear scoping.

