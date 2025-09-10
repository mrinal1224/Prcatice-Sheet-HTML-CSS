
---

# 📘 Advanced CSS Practice: Pseudo-classes & Buttons

---

## Q34) Hover Highlight

**Problem Description**
You’re designing a navigation menu. When the user hovers over a link, its background should turn yellow.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q34 - Hover Highlight</title>
<style>
  a {
    text-decoration: none;
    padding: 10px;
    display: inline-block;
  }
  /* Write your CSS here */
</style>
</head>
<body>
  <a href="#">Home</a>
  <a href="#">About</a>
</body>
</html>
```

**Test cases**

* Links display normally.
* On hover, background becomes yellow.

**Complete Solution**

```css
a:hover {
  background: yellow;
}
```

---

## Q35) Input Focus Glow

**Problem Description**
When the user **focuses on an input field**, add a glowing blue border to highlight it.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q35 - Input Focus Glow</title>
<style>
  input {
    padding: 8px;
    border: 1px solid #ccc;
    outline: none;
  }
  /* Write your CSS here */
</style>
</head>
<body>
  <input type="text" placeholder="Enter name">
</body>
</html>
```

**Test cases**

* Input looks normal by default.
* On focus, border glows blue.

**Complete Solution**

```css
input:focus {
  border-color: blue;
  box-shadow: 0 0 5px blue;
}
```

---

## Q36) Active Button Press

**Problem Description**
Create a button that looks like it gets **pressed down** when clicked (active state).

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q36 - Active Button</title>
<style>
  button {
    background: #4f46e5;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
  }
  /* Write your CSS here */
</style>
</head>
<body>
  <button>Click Me</button>
</body>
</html>
```

**Test cases**

* Button has normal state.
* On click, it looks pressed.

**Complete Solution**

```css
button:active {
  transform: translateY(2px);
  background: #3730a3;
}
```

---

## Q37) Decorative Line Before Title

**Problem Description**
Add a **blue line before a heading** using `::before`.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q37 - ::before Example</title>
<style>
  h2::before {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <h2>Section Title</h2>
</body>
</html>
```

**Test cases**

* Blue line appears before heading.
* Line is decorative (not actual text).

**Complete Solution**

```css
h2::before {
  content: "— ";
  color: blue;
}
```

---

## Q38) Decorative Line After Title

**Problem Description**
Add a **red line after a heading** using `::after`.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q38 - ::after Example</title>
<style>
  h2::after {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <h2>Important Notice</h2>
</body>
</html>
```

**Test cases**

* Red line appears after heading.
* Decorative only.

**Complete Solution**

```css
h2::after {
  content: " —";
  color: red;
}
```

---

## Q39) Button with Icon

**Problem Description**
Create a button that shows a **🔍 search icon before the text** using `::before`.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q39 - Button with Icon</title>
<style>
  button::before {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <button>Search</button>
</body>
</html>
```

**Test cases**

* Button has icon + text.
* Icon is added with CSS only.

**Complete Solution**

```css
button::before {
  content: "🔍 ";
}
```

---

## Q40) Button Hover Glow

**Problem Description**
Design a button that **glows with shadow** when hovered.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q40 - Hover Glow</title>
<style>
  button {
    background: #4f46e5;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 6px;
  }
  /* Write your CSS here */
</style>
</head>
<body>
  <button>Hover Me</button>
</body>
</html>
```

**Test cases**

* Normal button has no glow.
* On hover, button glows with shadow.

**Complete Solution**

```css
button:hover {
  box-shadow: 0 0 10px #4f46e5;
}
```

---

## Q41) Floating Label Input

**Problem Description**
Design a text field where the label moves **above the input** when the input is focused.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q41 - Floating Label</title>
<style>
  .field {
    position: relative;
    margin: 20px;
  }
  label {
    position: absolute;
    top: 10px;
    left: 10px;
    transition: 0.3s;
    color: gray;
  }
  input {
    padding: 10px;
  }
  /* Write your CSS here */
</style>
</head>
<body>
  <div class="field">
    <input type="text" id="name">
    <label for="name">Name</label>
  </div>
</body>
</html>
```

**Test cases**

* Label starts inside input.
* On focus, label moves up.

**Complete Solution**

```css
input:focus + label {
  top: -10px;
  font-size: 12px;
  color: blue;
}
```

---

## Q42) Primary & Secondary Buttons

**Problem Description**
Create two button styles:

* **Primary (blue background, white text)**
* **Secondary (white background, blue border, blue text)**

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q42 - Button Styles</title>
<style>
  .btn {
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
  }
  /* Write your CSS here */
</style>
</head>
<body>
  <button class="btn primary">Primary</button>
  <button class="btn secondary">Secondary</button>
</body>
</html>
```

**Test cases**

* Primary button: solid blue.
* Secondary button: outlined blue.

**Complete Solution**

```css
.primary {
  background: blue;
  color: white;
  border: none;
}
.secondary {
  background: white;
  color: blue;
  border: 2px solid blue;
}
```

---

## Q43) Animated Button Hover

**Problem Description**
Create a button that **changes background color smoothly** on hover using transition.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q43 - Animated Button</title>
<style>
  button {
    background: blue;
    color: white;
    padding: 10px 20px;
    border: none;
    transition: 0.3s;
  }
  /* Write your CSS here */
</style>
</head>
<body>
  <button>Hover Me</button>
</body>
</html>
```

**Test cases**

* Button background animates smoothly on hover.
* Uses `transition`.

**Complete Solution**

```css
button:hover {
  background: darkblue;
}
```

---


