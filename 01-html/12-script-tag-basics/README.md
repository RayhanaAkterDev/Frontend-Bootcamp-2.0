# Script Tag Basics

> Tags: script-tag, javascript  
> _Purpose:_ Learn how to use the HTML `<script>` tag to add JavaScript to web pages.

---

## My understanding

- The `<script>` tag is used to include JavaScript in HTML documents.
- JavaScript code can be written inline inside the `<script>` tag or linked as an external file using the `src` attribute.
- Inline scripts can manipulate HTML content dynamically, such as changing text or responding to user interactions.
- `<script>` tags can be placed in the `<head>` or `<body>`, but placing them just before the closing `</body>` tag is common to avoid blocking page loading.
- Console messages help debug and confirm that scripts are running correctly.

---

> [!note]
>
> - Use inline scripts for small snippets or quick demos.
> - For larger JavaScript code, external `.js` files keep HTML cleaner and easier to maintain.
> - The `defer` and `async` attributes on `<script>` tags control script loading behavior (advanced topic).
> - Always place `<script>` tags at the end of the `<body>` or use `defer` to prevent blocking HTML parsing.

---

> [!tip]
> The external script file `script.js` can be linked like this:  
> `<script src="script.js"></script>`

---

### Code links

- [Template code](01-template.html)  
- [Exercise code](02-exercise.html)

---
