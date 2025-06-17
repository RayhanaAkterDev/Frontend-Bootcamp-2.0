# CSS Selectors and Specificity

> Tags: `css-core`, `selectors`, `specificity`  
> _Purpose:_ Understand how CSS selectors work and how specificity determines which styles get applied when multiple rules target the same element.

---

## My understanding

- **CSS Selectors** are used to target and style HTML elements. There are various types like type, class, ID, attribute, pseudo-class, pseudo-element, etc.
- **Specificity** defines the priority of CSS rules. When more than one rule applies to the same element, the one with higher specificity wins.
- If two rules have the same specificity, the one that comes **later** in the CSS file overrides the earlier one.

---

### Specificity Hierarchy

1. Universal selector (`*`) — **0**
2. Type selectors (`div`, `p`) & pseudo-elements (`::before`) — **1**
3. Class selectors (`.class`), attributes (`[type="text"]`), pseudo-classes (`:hover`) — **10**
4. ID selectors (`#id`) — **100**
5. Inline styles (`style="..."`) — **1000**

---

### Key Tags & Purpose (simplified)

| Selector Type       | Example                   | Purpose                        |
|---------------------|---------------------------|--------------------------------|
| Universal           | `*`                       | Target all elements            |
| Type                | `p`, `h1`                 | Target specific tags           |
| Class               | `.box`, `.btn`            | Reusable group styles          |
| ID                  | `#header`, `#login-form`  | Style unique elements          |
| Attribute           | `input[type="text"]`      | Target elements with attribute |
| Pseudo-class        | `:hover`, `:focus`        | Apply style on interaction     |
| Pseudo-element      | `::after`, `::before`     | Style generated content        |
| Descendant          | `div span`                | Target child elements inside   |
| Child               | `ul > li`                 | Direct children only           |
| Group               | `h1, h2, p`               | Apply same style to many       |
| Negation            | `p:not(.special)`         | Exclude specific items         |

---

### Code links

- [Template HTML](./template/template.html) – used to list examples in one file  
- [Practice Page](./practice/index.html) – contains real examples for selectors & specificity  
- [CSS File](./practice/style.css) – where all selector types and specificity levels are applied
