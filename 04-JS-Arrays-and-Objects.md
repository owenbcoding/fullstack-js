# 04 – Arrays, Loops, and Objects

These notes reorganize your array and loop content from `Full Stack | Js interactive websites` into one coherent module. The Objects section is a placeholder for when you cover that topic.

---

## Arrays – Basics

An **array** is an ordered list of values, written with square brackets `[]`.

```jsx
const mixedArray = ["Owen", 42, true];
```

- The array is everything inside the `[]`.
- Each item is an **element**.
- Elements can be **any** type (numbers, strings, booleans, objects, other arrays, etc.).

### Vocabulary

- **Index** – the position of an element in the array, starting at `0`.
  - Think “first seat is seat 0”.
- **Element** – a single value/item stored in an array.

### Key points

- Arrays are **ordered** – the order you insert items is preserved.
- Arrays are **zero‑indexed** – the first element is at index `0`.

---

## Accessing Elements

Use **bracket notation** with an index:

```jsx
const cities = ["New York", "London", "Tokyo"];

console.log(cities[0]); // "New York"
console.log(cities[1]); // "London"
console.log(cities[2]); // "Tokyo"
```

Strings are also indexable:

```jsx
const hello = "Hello World";
console.log(hello[6]); // "W"
```

---

## Arrays with `let` and `const`

```jsx
let condiments = ["Ketchup", "Mustard", "Soy Sauce", "Sriracha"];
const utensils = ["Fork", "Knife", "Chopsticks", "Spork"];
```

- Declaring an array with **`const`** means you **cannot reassign** the variable:
  - `utensils = []` ❌
- But you **can** still **mutate** its contents:

```jsx
utensils[0] = "Spoon"; // ✅ allowed
```

- Declaring with **`let`** allows both **mutation** and **reassignment** of the variable.

---

## The `.length` Property

`.length` returns the **number of elements** in an array:

```jsx
const newYearsResolutions = ["Keep a journal", "Take a falconry class"];

console.log(newYearsResolutions.length); // 2
```

`.length` is also used heavily with loops to know when to stop.

---

## Adding and Removing Elements

### `.push()` – add to the end

```jsx
const itemTracker = ["item 0", "item 1", "item 2"];

itemTracker.push("item 3", "item 4");

console.log(itemTracker);
// ["item 0", "item 1", "item 2", "item 3", "item 4"]
```

- `.push()` is a **mutating** (destructive) method – it changes the original array.

### `.pop()` – remove from the end

```jsx
const newItemTracker = ["item 0", "item 1", "item 2"];

const removed = newItemTracker.pop();

console.log(newItemTracker); // ["item 0", "item 1"]
console.log(removed);        // "item 2"
```

- `.pop()` removes the **last** element and returns it.
- Also mutates the original array.

---

## Arrays & Functions

Arrays are **passed by reference**, so changes inside functions can affect the original array.

```jsx
const flowers = ["peony", "daffodil", "marigold"];

function addFlower(arr) {
  arr.push("lily");
}

addFlower(flowers);
console.log(flowers);
// ["peony", "daffodil", "marigold", "lily"]
```

Another example:

```jsx
const concept = ["arrays", "can", "be", "mutated"];

function changeArr(arr) {
  arr[3] = "MUTATED";
}

changeArr(concept);
console.log(concept); // ["arrays", "can", "be", "MUTATED"]

function removeElement(arr) {
  arr.pop();
}

removeElement(concept);
console.log(concept); // ["arrays", "can", "be"]
```

Be careful when mutating arrays inside functions – it can be powerful but also surprising if you expect data to stay unchanged.

---

## Nested Arrays

Arrays can contain other arrays – these are **nested arrays**.

```jsx
const nestedArr = [[1], [2, 3]];

console.log(nestedArr[1]);    // [2, 3]
console.log(nestedArr[1][0]); // 2
```

Chain bracket notation to access deeper levels:

- `nestedArr[1]` → the second inner array (`[2, 3]`)
- `nestedArr[1][0]` → first element of that inner array (`2`)

---

## Loops – Basics

Loops help you avoid writing the same code over and over.

### `for` loop structure

```jsx
for (initialization; condition; finalExpression) {
  // code to run each time
}
```

Example:

```jsx
for (let counter = 0; counter < 4; counter++) {
  console.log(counter);
}
// 0, 1, 2, 3
```

Explanation:

- `let counter = 0` – start at 0.
- `counter < 4` – keep looping while this is true.
- `counter++` – increase by 1 each iteration.

Another example (5 to 10):

```jsx
for (let counter = 5; counter < 11; counter++) {
  console.log(counter);
}
// 5, 6, 7, 8, 9, 10

```
Another for example :

```jsx
  const hobbies = ['singing', 'eating', 'quidditch', 'writing'];
  
  for (let i = 0; i < hobbies.length; i++) {
    console.log(`I enjoy ${hobbies[i]}.`);
  }
```
Notice how the for...of loop has a simpler syntax which is good for readability in larger more complext applications
Example of a for...of Loop
```jsx

  const hobbies = ['singing', 'eating', 'quidditch', 'writing'];
  
  for (const hobby of hobbies) {
    console.log(`I enjoy ${hobby}.`);
  }
```
Both Examples print this: 
I enjoy singing.
I enjoy eating.
I enjoy quidditch.
I enjoy writing.
---

## Looping in Reverse

Sometimes you want to loop from the **end** of an array back to the **start**.

```jsx
const fruits = ["apple", "banana", "cherry", "date"];

for (let i = fruits.length - 1; i >= 0; i--) {
  console.log(fruits[i]);
}
// date, cherry, banana, apple
```

This is especially useful when **removing items** from an array while you iterate, to avoid index issues.


---

## Looping Through Arrays

Classic `for` loop over an array:

```jsx
const vacationSpots = ["Bali", "Paris", "Tulum"];

for (let i = 0; i < vacationSpots.length; i++) {
  console.log("I would love to visit " + vacationSpots[i]);
}
```

Modern patterns (for reference):

```jsx
const numbers = [1, 2, 3, 4];

for (const num of numbers) {
  console.log(num * 2);
}

const doubled = numbers.map(num => num * 2);
console.log(doubled); // [2, 4, 6, 8]
```

---

## Nested Loops

A **nested loop** is a loop inside another loop.

Useful when comparing each element of one array with each element of another:

```jsx
const bobsFollowers = ["Maya", "Jake", "Zara", "Omar"];
const tinasFollowers = ["Zara", "Nina", "Omar"];
const mutualFollowers = [];

for (let i = 0; i < bobsFollowers.length; i++) {
  for (let j = 0; j < tinasFollowers.length; j++) {
    if (bobsFollowers[i] === tinasFollowers[j]) {
      mutualFollowers.push(bobsFollowers[i]);
    }
  }
}

console.log(mutualFollowers); // ["Zara", "Omar"]
```

> Be careful with nested loops: they can become slow for large arrays because they compare many combinations.

---

## `while` Loops

Use a `while` loop when you **don’t know** in advance how many times you’ll loop.

```jsx
const cards = ["diamond", "spade", "heart", "club"];
let currentCard;

while (currentCard !== "spade") {
  currentCard = cards[Math.floor(Math.random() * 4)];
  console.log(currentCard);
}

while loops evaluate a condition for however long it’s true and the looping stops when the condition is false.
```

Make sure the loop condition will eventually become false to avoid **infinite loops**.

---

## `do…while` Loops

A **do…while** loop runs its body **at least once**, then keeps going while a condition is true.

```jsx
let cupsOfSugarNeeded = 3;
let cupsAdded = 0;

do {
  cupsAdded++;
  console.log(cupsAdded + " cup was added");
} while (cupsAdded < cupsOfSugarNeeded);
```

---

## The `break` Keyword

`break` lets you exit a loop **early**.

```jsx
const rapperArray = ["Lil' Kim", "Jay-Z", "Notorious B.I.G.", "Tupac"];

for (let i = 0; i < rapperArray.length; i++) {
  console.log(rapperArray[i]);
  if (rapperArray[i] === "Notorious B.I.G.") {
    break;
  }
}

console.log("And if you don't know, now you know.");
```

Useful for:

- Searching until you find something.
- Stopping once a condition is satisfied.

---

## Objects (Placeholder)


This section is a placeholder for your future notes on **objects** in JavaScript. When you cover objects in your course, you can expand it with:

- What objects are and why we use them
- Creating objects: object literals `{ }`
- Properties and methods
- Accessing and updating: dot notation and bracket notation
- Looping over objects

---

## Quick Review – Arrays and Loops

- **Arrays** store ordered lists of values and are zero‑indexed.
- Use `.length`, `.push()`, `.pop()`, and bracket notation `[]` to work with array data.
- Arrays are **mutable** and passed by **reference**, so functions can change them.
- **Nested arrays** let you build more complex data structures.
- **Loops** (`for`, `while`, `do…while`, nested loops) let you repeat actions efficiently.
- `break` lets you exit a loop early once a condition is met.

