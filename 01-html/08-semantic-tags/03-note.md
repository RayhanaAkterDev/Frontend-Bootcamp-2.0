# HTML Semantic Tags

> Tags: semantic-tags  
> _Purpose:_ Understand the core of HTML5 semantic elements and accessibility enhancements.

---

## My understanding

- Semantic tags describe the purpose and structure of content, making it meaningful for browsers, search engines, and assistive technologies. Examples include:

  - `<header>`: Contains introductory content or navigation links, typically at the top of a page or section.
  - `<nav>`: Defines a section containing major navigation links.
  - `<main>`: Represents the main content unique to the document, excluding repeated elements like sidebars or navigation.
  - `<section>`: Groups related thematic content, usually with a heading that defines the section.
  - `<article>`: Contains self-contained, independent content such as blog posts, news articles, or user-generated content that can be syndicated or distributed independently.
  - `<aside>`: Contains content tangentially related to the main content, often displayed as a sidebar or call-out box.
  - `<footer>`: Defines the footer for a page or section, often containing copyright info, related links, or contact info.

- Using semantic elements improves document readability, search engine optimization (SEO), and accessibility for screen readers and other assistive devices.

- A **skip link** allows keyboard and screen reader users to bypass repetitive content (like navigation menus) and jump directly to the main content, improving navigation efficiency.

```html
<!-- Skip Link: Initially hidden off-screen, becomes visible on keyboard focus -->
<a href="#main-content" class="skip-link">Skip to Main Content</a>

<main id="main-content" tabindex="-1">
  <!-- Main page content here -->
</main>

<style>
  .skip-link {
    position: absolute;
    top: -40px; /* Hide off-screen */
    left: 0;
    background: #000;
    color: #fff;
    padding: 8px;
    z-index: 100;
    transition: top 0.3s ease;
  }
  .skip-link:focus {
    top: 0; /* Slide into view on keyboard focus */
  }
</style>
```

---

> [!note]
>
> - Prefer semantic tags over generic `<div>` and `<span>` where possible, as they provide meaning and improve accessibility. Use `<div>` only for grouping content when no semantic element fits.
> - Add ARIA roles or labels when semantic tags are insufficient for describing the content to assistive technologies.
> - The skip link should be the first focusable element in the document and visually hidden until focused, as shown in the example above.
> - Use `tabindex="-1"` on the main element to allow programmatic focus when the skip link is activated, without including it in the normal tab order.

---

### Code links

- [Template code](01-template.html)
- [Exercise code](02-exercise.html)

---
