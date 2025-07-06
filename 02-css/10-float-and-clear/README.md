# CSS Float & Clear

> Tags: css-basics, float-clear  
> _Purpose:_ Understand and practice how floating elements and clearing floats affect layout in CSS.

---

## ✅ My Understanding

- The `float` property allows elements (like images or boxes) to be aligned left or right, and text/content wraps around them.  
- Floated elements are taken out of the normal document flow, which may cause layout issues.  
- The `clear` property is used to prevent elements from sitting next to floated ones and forces them below.  
- Clearfix is a technique used to fix parent height issues when all child elements are floated.

---

## 🔍 Key Tags & Purpose

```css
/* Move element left or right */
float: left;
float: right;

/* Push an element below all floated siblings */
clear: both;

/* Clearfix to fix parent container collapse */
.clearfix::after {
    content: '';
    display: block;
    clear: both;
}
```

> Helps align images or boxes next to text and fix layout breaking issues caused by floats. Used more in traditional layouts.

---

## ⚠️ Confusing Parts Explained

1. ✅ `clear: both` is for **non-floated siblings** only. It doesn't fix the parent's collapsed height.  
2. 🔴 `clear: both` on the floated element itself does **nothing**.  
3. ✅ To fix a parent with only floated children, use this clearfix:

```css
.clearfix::after {
    content: '';
    display: block;
    clear: both;
}
```

> This invisible pseudo-element clears floats, so the parent wraps around its children properly.

---

### ⛔ Incorrect Fix (Doesn't Work)

```css
.container {
    clear: both; /* ❌ Useless on parent containers */
}
```

### ✅ Correct Fix (Works)

```css
.container::after {
    content: '';
    display: block;
    clear: both;
}
```

---

## 🔗 Code Links

- [Template code](./template/template.html)  
- [Practice code](./practice/index.html)

---
