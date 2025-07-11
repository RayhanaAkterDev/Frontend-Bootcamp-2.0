# CSS Float & Clear

> Tags: css-basics, float-clear  
> _Purpose:_ Understand and practice how **floating child elements** and clearing floats affect layout in CSS.

---

## ✅ My Understanding

1. The `float` property is used to **move child elements** (like images or boxes) to the **left or right** inside a container. Text and inline content wraps around them.  
2. Floated elements are taken out of the normal document flow, which may cause layout issues (like collapsed parent height).  
3. The `clear` property is applied to **non-floated sibling elements** to make them move **below** floated elements.  
4. Clearfix is a special CSS technique that helps the **parent container detect and wrap around floated children**.

---

## 🔍 Key Tags & Purpose

```html
<!-- Example layout with float and clear -->
<div class="container clearfix">
    <div class="box left">Left Box</div>
    <div class="box right">Right Box</div>
    <div class="clear-box">I come below both</div>
</div>
```

```css
/* Move elements left or right — applied to child elements */
.left {
    float: left;
    width: 40%;
    background: lightblue;
}

.right {
    float: right;
    width: 40%;
    background: lightgreen;
}

/* Push this element below both floated boxes */
.clear-box {
    clear: both;
    background: lightgray;
    padding: 10px;
}

/* Fix parent container height when all children are floated */
.clearfix::after {
    content: '';
    display: block;
    clear: both;
}
```

> Helps align images or boxes next to text and fix layout breaking issues caused by floats. Mostly used in older or traditional layouts.

---

## ⚠️ Confusing Parts Explained

1. ✅ **`float` is applied to child elements**, not the parent. Floating a parent has no layout effect.  
2. ✅ `clear: both` should be applied to **non-floated siblings**, not on the floated element itself.  
3. 🔴 `clear: both` on a floated child does **nothing useful**.  
4. ✅ To fix the parent container’s collapsed height (when all children are floated), use this clearfix:

```css
.clearfix::after {
    content: '';
    display: block;
    clear: both;
}
```

> This pseudo-element is inserted after all children and clears their float, making the parent wrap them properly.

---

### ⛔ Incorrect Fix (Doesn't Work)

```css
.container {
    clear: both; /* ❌ Does nothing when used on parent */
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
