# 06 – Async JavaScript and APIs (Outline) — Lesson 6

> **Main point:** This file is a placeholder for your future notes on **asynchronous JavaScript** and working with **APIs**. When you cover these topics in your course, you can flesh out each section.
>
> **Code blocks:** Fences use **triple tildes** (e.g. `~~~jsx`, `~~~text`, `~~~html`, `~~~css` … `~~~`) instead of triple backticks if the backtick key is awkward. For short snippets, many Markdown previews also accept HTML: `<pre><code class="language-js">…</code></pre>`.

## 06 – Async JavaScript and APIs (Outline) — Chapter 6 — 03/23/2026

*Use **Main notes** for explanations and code examples; use **Vocab** and **Important notes** when you review.*

---

## Main notes

### Synchronous vs Asynchronous Code

- Synchronous code runs **top‑to‑bottom**, one line at a time.
- Asynchronous code can **start work now** and **finish later** without blocking the main thread.

Topics to add:

- The event loop (high‑level understanding).
- Callbacks vs promises vs `async`/`await`.

---

### Callbacks

- Functions passed as arguments and invoked when some work completes.

Examples you can add later:

- `setTimeout`, `setInterval`.
- Basic callback patterns and common pitfalls (“callback hell”).

---

### Promises

- A Promise represents a **value that may be available now, later, or never**.

Sections to fill in:

- Creating promises.
- States: `pending`, `fulfilled`, `rejected`.
- Chaining with `.then()` and `.catch()`.

---

### `async` / `await`

- Syntactic sugar on top of promises.
- Lets async code look more like synchronous code.

Topics to expand:

- Declaring `async` functions.
- Using `await` to pause until a promise settles.
- Error handling with `try { ... } catch (error) { ... }`.

---

### Fetching Data from APIs

- Using the `fetch()` API to make HTTP requests.

Things to document as you learn them:

- Basic GET requests and parsing JSON: `response.json()`.
- Handling errors and loading states.
- Sending data with POST/PUT/PATCH/DELETE.

---

### Practical Patterns

Later you can add real examples like:

- Fetching data on page load and rendering it.
- Handling user input and then calling an API.
- Working with third‑party APIs (e.g., Reddit, weather, etc.).

---

## Vocab

- **Lesson focus:** 06 – Async JavaScript and APIs (Outline).
- **Callback** – function passed to run when async work finishes.
- **Promise** – object representing a future success or failure.
- **`async` / `await`** – syntax for promise-based async code.
- **`fetch`** – browser API for HTTP requests.
- **JSON** – common text format for API data (`JSON.parse` / `response.json()`).

---

## Important notes

> **Questions:** Write important questions you have in a box like this.

- Always handle **rejected promises** (`.catch` or `try/catch` with `await`).
- **`fetch`** only rejects on **network errors**, not on HTTP 4xx/5xx—check **`response.ok`**.


---

## Chapter 6 summary

When you review your notes, briefly summarize what you learned and what is important to retain from the full page of notes. That helps you internalize the information.

- **Async** work can finish later without blocking the rest of your script.
- **Callbacks** pass functions into other functions; **promises** model future results; **`async`/`await`** makes promise code easier to read.
- **`fetch`** is the usual way to call **HTTP APIs** and parse **JSON** responses.
