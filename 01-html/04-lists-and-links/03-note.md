# HTML Lists & Links

> Tags: html-lists-&-links  
> _Purpose:_ Understand the concept of HTML lists & links.

---

## My understanding

HTML lists organize content using bullets, numbers, or definition formats.

- `<ul>`: Defines an unordered list (bullet points).
- `<ol>`: Defines an ordered list (numbered items).
- `<li>`: Used inside `<ul>` or `<ol>` to define each list item.
- Nested list: A list placed inside an `<li>`.
- `<dl>`: Defines a description list, with:
  - `<dt>`: Term (name of the item).
  - `<dd>`: Description.
  - For accessibility, use `role="list"` on `<dl>` and `role="listitem"` on `<dd>`.

```html
<dl role="list">
    <dt>HTML</dt>
    <dd role="listitem">HyperText Markup Language</dd>
</dl>
```

---

- The `<a>` tag creates hyperlinks. These can be internal (within the site or page) or external (to another website).
- Some commonly used attributes:
  - `href`: Defines the link’s destination.
  - `target="_blank"`: Opens the link in a new tab.
  - `rel="noopener noreferrer"`: Used for external links to prevents tab-napping attacks _(required with `target="blank"`)_.
  - `download`: Allows users to download the linked file _(e.g., PDF, image)_.
  - To link to a specific section within the same page, use `#section-id` in the href attribute. This is known as an _internal anchor link_.

---

> Note: List types (e.g., disc, circle, decimal) are defined using CSS `list-style-type`. This will be discussed in CSS topics.

---

### Code links

- [Template code](01-template.html)
- [Exercise code](02-exercise.html)

---
