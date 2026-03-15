# 06 – Async JavaScript and APIs (Outline)

This file is a placeholder for your future notes on **asynchronous JavaScript** and working with **APIs**. When you cover these topics in your course, you can flesh out each section.

---

## Synchronous vs Asynchronous Code

- Synchronous code runs **top‑to‑bottom**, one line at a time.
- Asynchronous code can **start work now** and **finish later** without blocking the main thread.

Topics to add:

- The event loop (high‑level understanding).
- Callbacks vs promises vs `async`/`await`.

---

## Callbacks

- Functions passed as arguments and invoked when some work completes.

Examples you can add later:

- `setTimeout`, `setInterval`.
- Basic callback patterns and common pitfalls (“callback hell”).

---

## Promises

- A Promise represents a **value that may be available now, later, or never**.

Sections to fill in:

- Creating promises.
- States: `pending`, `fulfilled`, `rejected`.
- Chaining with `.then()` and `.catch()`.

---

## `async` / `await`

- Syntactic sugar on top of promises.
- Lets async code look more like synchronous code.

Topics to expand:

- Declaring `async` functions.
- Using `await` to pause until a promise settles.
- Error handling with `try { ... } catch (error) { ... }`.

---

## Fetching Data from APIs

- Using the `fetch()` API to make HTTP requests.

Things to document as you learn them:

- Basic GET requests and parsing JSON: `response.json()`.
- Handling errors and loading states.
- Sending data with POST/PUT/PATCH/DELETE.

---

## Practical Patterns

Later you can add real examples like:

- Fetching data on page load and rendering it.
- Handling user input and then calling an API.
- Working with third‑party APIs (e.g., Reddit, weather, etc.).

