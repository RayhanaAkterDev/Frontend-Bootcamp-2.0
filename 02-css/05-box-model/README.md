# CSS Box Model Explained

> Tags: css-fundamentals, box-model  
> _Purpose:_ Learn how CSS box model defines element dimensions and spacing to control layout precisely.

---

## Core Concept

Every HTML element is treated as a rectangular box composed of four layers stacked from inside out:

1. **Content:** The actual stuff inside the box, like text or images.
2. **Padding:** The inner space around the content, pushing the border outward.
3. **Border:** The line wrapping around padding and content.
4. **Margin:** The outer space outside the border that separates this box from others.

---

## How These Affect Layout

- The element’s total size is the sum of content size + padding + border + margin.
- Padding and border increase the visible size beyond content dimensions.
- Margin creates space between neighboring elements.
- Changing any of these values affects page spacing and alignment.

---

## Box-sizing Property

- By default (`content-box`), width and height apply only to the content area.
- With `box-sizing: border-box`, width and height include padding and border, simplifying size calculations.

---

## Visual Model

```text
[ Margin ] [ Border ] [ Padding ] [ Content ]
```

---

### Code links

- [Template code](./template/template.html)  
- [Practice code](./practice/index.html)

---
