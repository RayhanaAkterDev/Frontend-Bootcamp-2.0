# Fluid Layouts

> **Tags**: css-layouts, responsive-design  
> _**Purpose**_: Understand and implement fluid layouts using percentages and viewport units to create flexible, responsive designs.

---

## My Understanding

1. A **fluid layout** uses **relative units** such as percentages (`%`) and viewport units (`vw`, `vh`) instead of fixed pixels.
2. This approach allows the layout to **adapt automatically** to different screen sizes or browser windows.
3. Unlike fixed layouts, fluid layouts are **inherently responsive**, often without needing media queries for every breakpoint.

---

> [!note]
>
> - `%` is relative to the **parent element’s size**.
> - `vw` and `vh` are relative to the **browser viewport** (the visible portion of the page).
> - To avoid layouts becoming **too wide or too narrow**, combine fluid units with `max-width` or `min-width`.

---

### 🔑 Key Tags & Purpose (🧠 Easy Revision)

| Tag / Term  | Purpose                                          |
|-------------|--------------------------------------------------|
| `%`         | Scales based on the parent element’s width       |
| `vw / vh`   | Scales based on the browser’s viewport dimensions|
| `max-width` | Limits how wide an element can grow              |
| `min-width` | Prevents an element from shrinking too much      |

---

### 🧪 Code Links

- [🔗 Template Code](./template/template.html)  
- [🔗 Practice Code](./practice/index.html)
