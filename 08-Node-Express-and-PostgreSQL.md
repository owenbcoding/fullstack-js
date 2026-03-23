# 08 – Node, Express, and PostgreSQL — Lesson 8

> **Main point:** This file pulls your existing **Node runtime** and **local Node setup** notes into one place and provides placeholders for future Express and PostgreSQL content.
>
> **Code blocks:** Fences use **triple tildes** (e.g. `~~~jsx`, `~~~text`, `~~~html`, `~~~css`, `~~~bash` … `~~~`) instead of triple backticks if the backtick key is awkward. For short snippets, many Markdown previews also accept HTML: `<pre><code class="language-js">…</code></pre>`.

## 08 – Node, Express, and PostgreSQL — Chapter 8 — 03/23/2026

*Use **Main notes** for explanations and code examples; use **Vocab** and **Important notes** when you review.*

---

## Main notes

### Node Runtime Environment

A **runtime environment** is where your program executes. It determines:

- Which **global objects** your code can access.
- How your program interacts with the **OS**, **network**, and **filesystem**.

JavaScript commonly runs in two environments:

1. **Browser runtime** – front‑end apps, access to the `window` object, DOM, etc.
2. **Node runtime** – back‑end apps, access to the filesystem, environment variables, and network APIs.

#### Browser example

In an HTML file:

~~~html
<html>
  <body>
    <h1>My Website</h1>
    <script>
      window.alert("Hello World");
    </script>
  </body>
</html>
~~~

When the browser loads the page, it executes the embedded JavaScript in the **browser runtime**:

- `window.alert()` is available because of the browser environment.
- The `window` object exposes many browser‑specific APIs (DOM, history, etc.).

#### Node example

Node runs JavaScript *outside* the browser, so:

- `window` and DOM APIs are **not** available.
- You get other globals like `process`, `__dirname`, and module utilities.

~~~jsx
// my-app.js
console.log(process.env.PWD);
~~~

- `process` – object with information about the current Node process.
- `process.env` – environment variables (e.g. `PWD` for “print working directory” in many shells).

Run this with:

~~~bash
node my-app.js
~~~

---

### Setting Up Node Locally

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

~~~jsx
console.log("Hello, World!");
~~~

6. **Run with Node**

~~~bash
node hello.js
~~~

If Node is correctly installed and you’re in the right folder, you’ll see `Hello, World!` in the terminal.

---

### Express (Placeholder)

As you move into Express, you can expand these sections:

- What Express is (a minimal web framework for Node).
- Creating an Express app and basic routes.
- Middleware (`app.use`).
- Handling JSON (`express.json()`).
- Error handling patterns.

---

### PostgreSQL (Placeholder)

Planned topics:

- What a relational database is.
- Basic SQL: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.
- Connecting Node/Express to PostgreSQL.
- Running queries safely (parameterized queries).

---

### Full‑Stack PERN Overview (Placeholder)

Later, you can add:

- How React (front‑end) talks to Express (API).
- How Express talks to PostgreSQL (database).
- Environment variables and configuration.

---

## Vocab

- **Lesson focus:** 08 – Node, Express, and PostgreSQL.
- **Runtime** – environment where JS executes (browser vs Node).
- **`global` / `window` / `process`** – environment-specific globals.
- **Module** – file whose exports can be imported elsewhere (`require` / `import`).
- **Express** – Node web framework for HTTP routing and middleware.
- **PostgreSQL** – relational database; **SQL** for queries.
- **PERN** – Postgres, Express, React, Node stack pattern.

---

## Important notes

> **Questions:** Write important questions you have in a box like this.

- Never build SQL with raw string concatenation from user input—use **parameters**.
- Keep **secrets** in **environment variables**, not in source code.


---

## Chapter 8 summary

When you review your notes, briefly summarize what you learned and what is important to retain from the full page of notes. That helps you internalize the information.

- **Node** runs JavaScript on the server with different **globals** than the browser.
- **Express** is a minimal framework for **routes** and **middleware**.
- **PostgreSQL** stores relational data; pair it with **parameterized queries** for safe access from Node.
