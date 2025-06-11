# HTML Accessibility

> Tags: html-basics, accessibility  
> _Purpose:_ Understand and practice the core principles and best practices of HTML accessibility.

---

## My understanding

### 1. Semantic HTML and Landmarks

- Use semantic HTML5 elements (`<header>`, `<nav>`, `<main>`, `<footer>`, etc.) to define meaningful page structure.
- These landmarks help assistive technologies and users navigate content easily.

### 2. Images and Alternative Text

- Provide descriptive `alt` attributes on images for screen readers.
- Alt text should be concise and meaningful without redundant phrases like “image of.”

### 3. Forms and Labels

- Always associate form inputs with `<label>` elements.
- Use ARIA attributes such as `aria-required` to indicate required fields.
- Provide additional instructions via screen reader-only text where necessary.

### 4. Keyboard Navigation

- Include skip links (`<a href="#main-content" class="sr-only">`) to allow users to bypass repetitive navigation.
- Ensure keyboard focus is visually distinct using CSS outlines or styles.

### 5. Dynamic Content Updates

- Use ARIA live regions (`aria-live="polite"`) to notify screen readers of dynamic changes without interrupting the user.

### 6. Accessible Tables

- Use `<caption>`, `<thead>`, and `<th scope="col">` to provide context and structure.
- Proper markup improves navigation for assistive tools.

---

> [!note]
>
> - Always test your site’s accessibility using screen readers and keyboard navigation to ensure usability.  
> - Prioritize semantic HTML before applying ARIA attributes.  
> - Visible focus indicators and skip links enhance keyboard usability.  
> - Accessibility also positively impacts SEO and user reach.

---

### Code links

- [Template code](01-template.html)  
- [Exercise code](02-exercise.html)

---
