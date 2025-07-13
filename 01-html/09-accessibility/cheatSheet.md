# 🧩 HTML Accessibility Cheatsheet

## ✅ 1. Semantic HTML Tags

| Tag        | Purpose                            |
|------------|------------------------------------|
| `<header>` | Page or section header             |
| `<nav>`    | Navigation links                   |
| `<main>`   | Main content area                  |
| `<section>`| Thematic grouping of content       |
| `<article>`| Self-contained content block       |
| `<aside>`  | Sidebar or related content         |
| `<footer>` | Footer of page or section          |
| `<button>` | Clickable button                   |
| `<form>`   | Form container                     |
| `<label>`  | Label for input                    |

---

## 🎯 2. ARIA Roles

| Role          | Purpose                         |
|---------------|----------------------------------|
| `button`      | Interactive button              |
| `link`        | Navigational link               |
| `list`        | Container for list items        |
| `listitem`    | Item inside a list              |
| `dialog`      | Modal or pop-up window          |
| `navigation`  | Section with nav links          |
| `banner`      | Site-wide header                |
| `main`        | Primary content area            |
| `alert`       | Important message               |

---

## 🔤 3. ARIA Attributes

| Attribute         | Purpose                                        | Values                      |
|-------------------|------------------------------------------------|-----------------------------|
| `aria-label`      | Custom label for screen readers                | `"Open menu"`               |
| `aria-labelledby` | Refers to an element that labels this one     | `id of another element`     |
| `aria-describedby`| Refers to element that describes this one      | `id of description`         |
| `aria-hidden`     | Hides element from screen reader               | `true`, `false`             |
| `aria-expanded`   | Element’s expanded/collapsed state             | `true`, `false`             |
| `aria-checked`    | Checkbox/radio state                           | `true`, `false`, `mixed`    |
| `aria-disabled`   | Marks element as inactive                      | `true`, `false`             |
| `aria-required`   | Marks input as required                        | `true`, `false`             |
| `aria-controls`   | Points to controlled element                   | `id of target`              |
| `aria-live`       | Announces dynamic content                      | `off`, `polite`, `assertive`|
| `aria-haspopup`   | Indicates presence of a popup/menu             | `true`, `menu`, etc.        |
| `aria-modal`      | Marks dialog as modal                          | `true`, `false`             |

---

## 🧪 4. Accessibility Tips

| Task                                | Tip                                      |
|-------------------------------------|-------------------------------------------|
| Image                               | Use `alt` attribute                       |
| Decorative icon                     | Use `aria-hidden="true"`                  |
| Custom dropdown                     | Add `role="listbox"` and `aria-expanded` |
| Form input                          | Use `<label>` or `aria-label`            |
| Button                              | Use `<button>` or `role="button"`        |
| Headings                            | Use proper `<h1>` to `<h6>` hierarchy    |
| Keyboard navigation                 | Ensure all actions are keyboard-accessible |
| Skip to content                     | Add a “skip to main” link at top         |
