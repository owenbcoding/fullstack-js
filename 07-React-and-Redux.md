# 07 – React and Redux (Outline) — Lesson 7

> **Main point:** This file is a structured outline for your upcoming **React** and **Redux** notes. As you work through the corresponding course units, you can replace and expand these sections with concrete examples.
>
> **Code blocks:** Fences use **triple tildes** (e.g. `~~~jsx`, `~~~text`, `~~~html`, `~~~css` … `~~~`) instead of triple backticks if the backtick key is awkward. For short snippets, many Markdown previews also accept HTML: `<pre><code class="language-js">…</code></pre>`.

## 07 – React and Redux (Outline) — Chapter 7 — 03/23/2026

*Use **Main notes** for explanations and code examples; use **Vocab** and **Important notes** when you review.*

---

## Main notes

### React Basics

Planned topics:

- What React is and why we use it.
- Components (functional components).
- JSX syntax.
- Props and state.

---

### Component Composition

- Building UIs from small, reusable components.
- Parent/child relationships and passing data via props.

---

### State and Hooks

Topics to fill in:

- `useState` for local component state.
- `useEffect` for side effects (fetching data, subscriptions).
- Derived state and lifting state up.

---

### React and the DOM

- Virtual DOM basics.
- Rendering lists.
- Handling events in React (`onClick`, `onChange`, etc.).

---

### Intro to Redux

Planned topics:

- Why Redux (global state management).
- Core principles: single store, actions, reducers.
- The Redux data flow: dispatch → reducer → new state.

---

### Using Redux with React

Sections to fill in:

- Setting up a Redux store.
- `Provider`, `useSelector`, and `useDispatch`.
- Splitting state into slices.

---

### Async Flows with Redux

Later you can add:

- Thunks (`redux-thunk`) or other middleware.
- Handling async API calls in Redux.

---

## Vocab

- **Lesson focus:** 07 – React and Redux (Outline).
- **Component** – reusable UI piece; often a function returning JSX.
- **JSX** – HTML-like syntax compiled to JavaScript function calls.
- **Props** – inputs to a component; read-only from the child’s perspective.
- **State** – data that can change and trigger re-renders (`useState`).
- **`useEffect`** – hook for side effects (fetching, subscriptions, DOM sync).
- **Redux store / reducer / action** – predictable global state updates.

---

## Important notes

> **Questions:** Write important questions you have in a box like this.

- Treat **props** as read-only; update UI through **state** or lifted state.
- **`useEffect`** dependencies matter—stale closures and infinite loops are common gotchas.


---

## Chapter 7 summary

When you review your notes, briefly summarize what you learned and what is important to retain from the full page of notes. That helps you internalize the information.

- **React** builds UIs from **components**; **JSX** describes what to render.
- **Props** pass data down; **state** (`useState`) and **effects** (`useEffect`) handle UI changes and side work.
- **Redux** centralizes **global state** with **actions**, **reducers**, and a single **store**.
