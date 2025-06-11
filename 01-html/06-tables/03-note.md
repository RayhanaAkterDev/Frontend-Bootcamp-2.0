# HTML Tables

> Tags: html-tables  
> _Purpose:_ Understand the core concept and structure of HTML tables.

---

## My Understanding

- `<table>` → Defines a table.
- `<caption>` → Adds a title above the table (helps with accessibility).
- `<thead>` → Groups the header row(s) of a table.
- `<tbody>` → Groups the main content rows.
- `<tr>` → Table row container (inside `<thead>`, `<tbody>`, or `<tfoot>`).
- `<th>` → Table header cell (bold, centered by default).
- `<td>` → Table data cell (regular cell).
- `scope` → Attribute used in `<th>` to define if it's a header for a row or column (`scope="col"` or `scope="row"`).
- `<tfoot>` → Groups footer rows in a table (e.g., totals or summary).  

> ⚠️ Appears at the bottom when rendered, even if placed before `<tbody>`. No visual difference by default — use CSS to style it if needed.
  
---

> 🧠 _Tip:_
> Always use semantic elements like `<thead>`, `<tbody>`, `<caption>`, and `scope` attributes for better screen reader support and clarity.

---

## Good Practice Reminders

- Avoid using old table attributes like `border`, `cellspacing`, or `cellpadding`.  
  👉 Use CSS for styling instead.
- Don’t put visual elements (like `<hr>`) inside `<caption>`.
- Use `<th scope="row">` in the first column if it describes the row content.

---

### Code Links

- [Template code](01-template.html) – Clean and semantic table example
- [Exercise code](02-exercise.html) – Practice version with variations

---
