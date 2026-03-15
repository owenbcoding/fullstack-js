# 08 – Node, Express, and PostgreSQL

This file pulls your existing **Node runtime** and **local Node setup** notes into one place and provides placeholders for future Express and PostgreSQL content.

---

## Node Runtime Environment

A **runtime environment** is where your program executes. It determines:

- Which **global objects** your code can access.
- How your program interacts with the **OS**, **network**, and **filesystem**.

JavaScript commonly runs in two environments:

1. **Browser runtime** – front‑end apps, access to the `window` object, DOM, etc.
2. **Node runtime** – back‑end apps, access to the filesystem, environment variables, and network APIs.

### Browser example

In an HTML file:

```html
<html>
  <body>
    <h1>My Website</h1>
    <script>
      window.alert("Hello World");
    </script>
  </body>
</html>
```

When the browser loads the page, it executes the embedded JavaScript in the **browser runtime**:

- `window.alert()` is available because of the browser environment.
- The `window` object exposes many browser‑specific APIs (DOM, history, etc.).

### Node example

Node runs JavaScript *outside* the browser, so:

- `window` and DOM APIs are **not** available.
- You get other globals like `process`, `__dirname`, and module utilities.

```jsx
// my-app.js
console.log(process.env.PWD);
```

- `process` – object with information about the current Node process.
- `process.env` – environment variables (e.g. `PWD` for “print working directory” in many shells).

Run this with:

```bash
node my-app.js
```

---

## Setting Up Node Locally

Node.js is a JavaScript runtime that lets you run JS **outside the browser**.

High‑level steps (matching your notes):

1. **Create a projects folder**
   - e.g. `Projects` or `dev` directory where all your code lives.
2. **Make a new project folder**
   - Example: `helloJavaScript/`.
3. **Open the folder in VS Code**
   - Use the Explorer → “Open Folder…” and select your project.
4. **Create a JavaScript file**
   - Example: `hello.js`.
5. **Write a simple program**

```jsx
console.log("Hello, World!");
```

6. **Run with Node**

```bash
node hello.js
```

If Node is correctly installed and you’re in the right folder, you’ll see `Hello, World!` in the terminal.

---

## Express (Placeholder)

As you move into Express, you can expand these sections:

- What Express is (a minimal web framework for Node).
- Creating an Express app and basic routes.
- Middleware (`app.use`).
- Handling JSON (`express.json()`).
- Error handling patterns.

---

## PostgreSQL (Placeholder)

Planned topics:

- What a relational database is.
- Basic SQL: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.
- Connecting Node/Express to PostgreSQL.
- Running queries safely (parameterized queries).

---

## Full‑Stack PERN Overview (Placeholder)

Later, you can add:

- How React (front‑end) talks to Express (API).
- How Express talks to PostgreSQL (database).
- Environment variables and configuration.

