# HTML Forms

> Tags: html-forms  
> _Purpose:_ Learn how to build accessible, semantic HTML forms using best practices.

---

## My Understanding

HTML forms allow users to input and submit data, commonly used in:

- Contact pages
- Sign-up forms
- Surveys and feedback forms

---

### Key Elements & Attributes

- `<form>` → Container for all input elements.  
  - `action` → URL where form data is sent (e.g., `/submit`)  
  - `method` → `post` or `get` specifies how the data is submitted  

---

- `<label>` → Describes form inputs for users and screen readers.  
  - Must be explicitly linked to input via the `for` attribute matching the input's `id`

---

- `<input>` → Single-line text fields.  
  Common attributes:
  - `type="text"` → For names  
  - `type="email"` → For email addresses  
  - `required` → Ensures input must be filled  
  - `autocomplete` → Enables browser autofill  
  - `placeholder` → Shows sample input text inside the field  
  - `title` → Shows tooltip with extra info on hover or focus  

---

- `<textarea>` → Multi-line input for longer messages.  
  - Can include `placeholder` and `title`  
  - `autocomplete="off"` may be used for privacy (optional)

---

- `<fieldset>` → Groups related form inputs logically  
- `<legend>` → Describes the group within a `<fieldset>`  
- `<button type="submit">` → Submits the form data

---

### Accessibility & UX Notes

> [!note]
>
> - ✅ Use `aria-describedby` to associate a descriptive paragraph with the form (improves screen reader context).  
> - ✅ Always pair inputs with visible `<label>` elements. Never rely solely on `placeholder` or `title`.  
> - ✅ Use `autocomplete` to enhance user experience (name, email, etc.)  
> - ✅ Use `title` to provide optional guidance via tooltips.  
> - ✅ Placeholders offer example input but should not replace labels.  
> - ✅ `autocomplete="off"` is useful for privacy in sensitive fields (like messages).

---

> [!warning]
> Avoid using `aria-label` unnecessarily if there is already a visible heading and description that serve the same purpose.

---

> 🧠 _Tip:_ Use a combination of semantic tags, visible labels, ARIA attributes, placeholders, and titles to create forms that are both accessible and user-friendly.

---

### Code Links

- [Template code](01-template.html)  
- [Exercise code](02-exercise.html)

---
