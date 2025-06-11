# Block vs Inline Elements

> Tags: html-basics  
> _Purpose:_ Understand and practice the core of block and inline elements in HTML.

---

## My understanding

- Block elements take up the **entire width** of their container and always start on a **new line**.
- Inline elements only take up as much **width as needed** and stay **within the same line** as surrounding content.
- Some elements like `<div>`, `<p>`, `<section>` are block-level, while `<span>`, `<a>`, `<strong>`, `<em>` are inline-level.

---

### 🧩 Common Block vs Inline Elements

| Block Elements                      | Inline Elements                                  |
|-------------------------------------|--------------------------------------------------|
| `<div>` – Generic container         | `<span>` – Generic inline container              |
| `<p>` – Paragraph                   | `<a>` – Hyperlink                                |
| `<h1>` to `<h6>` – Headings         | `<strong>` – Important text (bold)               |
| `<section>` – Page section          | `<em>` – Emphasis (italic)                       |
| `<article>` – Independent content   | `<b>` / `<i>` – Bold / Italic                    |
| `<header>` / `<footer>`             | `<img>` – Image                                  |
| `<nav>` – Navigation links          | `<input>` – Form input                           |
| `<aside>` – Sidebar info            | `<label>` – Label for form field                 |
| `<ul>` / `<ol>` / `<li>` – Lists    | `<select>` / `<textarea>`\* – Inline by default  |
| `<form>` – Form container           | `<code>`, `<kbd>`, `<samp>` – Code tags          |
| `<table>` and child tags            | `<abbr>`, `<cite>`, `<mark>` – Text markup       |
| `<blockquote>` – Quotation          | `<small>`, `<sub>`, `<sup>` – Text size/position |
| `<hr>` – Horizontal rule            | `<br>` – Line break (no visual width)            |

---

> [!note]
>
> - `<select>` and `<textarea>` behave like inline-block by default but are usually styled as block elements.
> - Do not put block elements inside inline elements — this causes invalid HTML.

---

### Code links

- [Template code](01-template.html)
- [Exercise code](02-exercise.html)

---
