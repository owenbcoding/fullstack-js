# 05 – DOM and Events (Outline) — Lesson 5

> **Main point:** This file is a placeholder for your upcoming notes on the **DOM (Document Object Model)** and **events** in JavaScript. As you continue your course, you can expand each section with more detailed examples.
>
> **Code blocks:** Fences use **triple tildes** (e.g. `~~~jsx`, `~~~text`, `~~~html`, `~~~css` … `~~~`) instead of triple backticks if the backtick key is awkward. For short snippets, many Markdown previews also accept HTML: `<pre><code class="language-js">…</code></pre>`.

## 05 – DOM and Events (Outline) — Chapter 5 — 03/23/2026

*Use **Main notes** for explanations and code examples; use **Vocab** and **Important notes** when you review.*

---

## Main notes

### The DOM (Document Object Model)

- The DOM is a **tree‑like representation** of the HTML in a page.
- JavaScript can **read** and **modify** this structure at runtime.

Topics to fill in:

- Selecting elements: `document.getElementById`, `querySelector`, `querySelectorAll`
- Reading and changing content: `textContent`, `innerHTML`
- Editing attributes and classes: `setAttribute`, `classList.add/remove/toggle`

---

### Modifying Styles

- Use the `.style` property or add/remove CSS classes.

Examples to add later:

- Change colors, sizes, visibility.
- Show/hide elements based on user input.

---

### Events & Event Listeners

- Events represent **user interactions** (clicks, key presses, form submissions, etc.).
- Use `addEventListener` to respond to events.

Topics to fill in:

- Click events on buttons and links.
- Keyboard events (`keydown`, `keyup`).
- Form submit handling and validation.

---

### Event Propagation (Bubble & Capture)

- How events move through the DOM tree.
- Stopping propagation with `event.stopPropagation()`.

---

### Default Browser Behavior

- Preventing defaults (e.g., form submission, link navigation) with `event.preventDefault()`.

---

### DOM + Events Patterns

As you learn them, you can document:

- Building interactive components (modals, dropdowns, tabs).
- Handling input and updating the UI dynamically.

---

## Vocab

- **Lesson focus:** 05 – DOM and Events (Outline).
- **DOM** – Document Object Model; tree of nodes mirroring HTML.
- **Element / node** – pieces of the document tree you can select and update.
- **`querySelector` / `querySelectorAll`** – CSS-selector based lookups.
- **`textContent` / `innerHTML`** – read or change element text or markup.
- **`classList`** – add/remove/toggle CSS classes from JS.
- **Event listener** – function registered to run when an event fires.

---

## Important notes

> **Questions:** Write important questions you have in a box like this.

- When learning the DOM, keep **DevTools Elements + Console** open.
- Separate **structure (HTML)**, **style (CSS)**, and **behavior (JS)**.


---

## Chapter 5 summary

When you review your notes, briefly summarize what you learned and what is important to retain from the full page of notes. That helps you internalize the information.

- The **DOM** is a tree of nodes representing HTML; scripts can **select** and **change** elements.
- **Events** (click, keypress, submit) drive interactivity; use **`addEventListener`** and know **`preventDefault`** / **`stopPropagation`**.
- Prefer **classes** and structure over inline styles when you update the UI from JavaScript.
