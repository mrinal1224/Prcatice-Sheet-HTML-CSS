* **Problem Description** (story-driven)
* **Starter (stub)** (with missing CSS/HTML for students)
* **Test cases**
* **Complete Solution**

Since 33 full questions with full HTML/CSS will be huge, I’ll deliver them in **batches of \~5–6 questions** so they’re readable and you can directly share them with your students.

Let’s start with **Q1 – Q6**.

---

# 📘 HTML & CSS Practice Sheet

---

## Q1) Center Stage

**Problem Description**
Imagine you are a stage designer setting up a performance. Three performers need to stand side by side in perfect alignment at the very center of the stage. The audience should see them arranged in the order 1, 2, 3, with equal spacing between each performer.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q1 - Center Stage</title>
<style>
  .container {
    width: 600px;
    height: 300px;
    background: #eee;
    border: 2px dashed #bbb;

    /* Write your code here */
  }
  .box {
    width: 80px;
    height: 80px;
    background: #4f46e5; /* indigo */
    color: white;
    display: grid;
    place-items: center;
    font: bold 16px/1 system-ui, sans-serif;
    border-radius: 8px;
  }
</style>
</head>
<body>
  <div class="container">
    <div class="box">1</div>
    <div class="box">2</div>
    <div class="box">3</div>
  </div>
</body>
</html>
```

**Test cases**

* The center of the middle box aligns with the container’s center (both axes).
* Equal spacing between boxes.
* Visual order: 1, 2, 3.

**Complete Solution**

```html
<style>
  .container {
    width: 600px;
    height: 300px;
    background: #eee;
    border: 2px dashed #bbb;

    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
  }
</style>
```

---

## Q2) Picture Perfect

**Problem Description**
You’re a photographer building an online gallery. Your task is to display an image centered on the screen. If the image doesn’t load, visitors should still see a text description.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q2 - Picture Perfect</title>
<style>
  body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background: #fafafa;
  }
</style>
</head>
<body>
  <!-- Write your code here -->
</body>
</html>
```

**Test cases**

* Image is centered.
* Image has `alt` text.
* If image is missing, alt text displays.

**Complete Solution**

```html
<body>
  <img src="cat.jpg" alt="Cute cat picture" width="300">
</body>
```

---

## Q3) Stylish Words

**Problem Description**
You’re designing a magazine. Some words need **bold emphasis**, and others should be *italicized* for softer impact.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q3 - Stylish Words</title>
</head>
<body>
  <p>
    <!-- Write your text here -->
  </p>
</body>
</html>
```

**Test cases**

* At least one **bold** word.
* At least one *italic* word.
* Both inside one paragraph.

**Complete Solution**

```html
<p>
  This is <b>bold</b> and this is <i>italic</i>.
</p>
```

---

## Q4) Grocery List

**Problem Description**
You’re creating a shopping list for your website. Fruits should appear as a bullet list, and instructions should appear as a numbered list.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q4 - Grocery List</title>
</head>
<body>
  <!-- Write your code here -->
</body>
</html>
```

**Test cases**

* Fruits shown in an unordered list.
* Steps shown in an ordered list.

**Complete Solution**

```html
<ul>
  <li>Apples</li>
  <li>Bananas</li>
</ul>
<ol>
  <li>Buy fruits</li>
  <li>Wash before eating</li>
</ol>
```

---

## Q5) People Table

**Problem Description**
You’re asked to display user details (Name, Age, City) in a table format.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q5 - People Table</title>
</head>
<body>
  <!-- Write your code here -->
</body>
</html>
```

**Test cases**

* Table has 1 header row and 1 data row.
* Columns: Name, Age, City.

**Complete Solution**

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>
  <tr>
    <td>John</td>
    <td>25</td>
    <td>Delhi</td>
  </tr>
</table>
```

---

## Q6) Identity Form

**Problem Description**
Your client wants a simple form to collect a person’s name and gender, with a submit button at the end.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q6 - Identity Form</title>
</head>
<body>
  <!-- Write your code here -->
</body>
</html>
```

**Test cases**

* Text input for name.
* Two radio buttons for gender.
* Submit button present.

**Complete Solution**

```html
<form>
  <label>Name:</label>
  <input type="text" name="name"><br><br>

  <label>Gender:</label>
  <input type="radio" name="gender" value="male"> Male
  <input type="radio" name="gender" value="female"> Female<br><br>

  <button type="submit">Submit</button>
</form>
```

---

Perfect 👍
Let’s move forward with the next batch: **Q7 – Q12**.
(Same format → Problem → Starter Stub → Test Cases → Complete Solution)

---

# 📘 HTML & CSS Practice Sheet (Q7 – Q12)

---

## Q7) Country Picker

**Problem Description**
You’re building a travel website. On the signup form, users must select their country from a dropdown list. For now, support only **India, USA, Japan**.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q7 - Country Picker</title>
</head>
<body>
  <!-- Write your code here -->
</body>
</html>
```

**Test cases**

* Dropdown menu present.
* Three options: India, USA, Japan.
* User can select only one country.

**Complete Solution**

```html
<select>
  <option>India</option>
  <option>USA</option>
  <option>Japan</option>
</select>
```

---

## Q8) Blog Layout

**Problem Description**
You’re creating a blog page. The page should have:

* A `<header>` with the blog title.
* An `<article>` with a post.
* A `<footer>` with copyright text.

This structure uses semantic tags for better accessibility and SEO.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q8 - Blog Layout</title>
</head>
<body>
  <!-- Write your code here -->
</body>
</html>
```

**Test cases**

* Blog has a header, article, and footer.
* Each section uses correct semantic tags.

**Complete Solution**

```html
<header><h1>My Blog</h1></header>
<article>
  <h2>First Post</h2>
  <p>This is my blog post.</p>
</article>
<footer>© 2025 My Blog</footer>
```

---

## Q9) Div vs Section

**Problem Description**
You need to explain to your class the difference between `<div>` (generic container) and `<section>` (semantic block).

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q9 - Div vs Section</title>
</head>
<body>
  <!-- Write your code here -->
</body>
</html>
```

**Test cases**

* `<section>` contains meaningful content.
* `<div>` is used for styling only.

**Complete Solution**

```html
<section>
  <h2>About Us</h2>
  <p>This is semantic content.</p>
</section>
<div style="background: lightgray;">Just a container</div>
```

---

## Q10) Blue Announcement

**Problem Description**
You are tasked with creating an announcement paragraph styled in blue text, with font size `20px`.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q10 - Blue Announcement</title>
</head>
<body>
  <!-- Write your code here -->
</body>
</html>
```

**Test cases**

* Text color is blue.
* Font size is 20px.

**Complete Solution**

```html
<p style="color: blue; font-size: 20px;">
  This is an important announcement!
</p>
```

---

## Q11) External Stylesheet

**Problem Description**
You are creating a professional website. Instead of inline styles, you must connect an **external stylesheet (style.css)** that changes the background color of the page.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q11 - External Stylesheet</title>
<!-- Link CSS file here -->
</head>
<body>
  <p>Hello World</p>
</body>
</html>
```

**Test cases**

* CSS file is linked correctly.
* Body background color changes.

**Complete Solution**

```html
<!-- index.html -->
<link rel="stylesheet" href="style.css">
```

```css
/* style.css */
body {
  background-color: lightyellow;
}
```

---

## Q12) Centered Title

**Problem Description**
You’re asked to build a landing page where the main heading must always be centered horizontally.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q12 - Centered Title</title>
<style>
  /* Write CSS here */
</style>
</head>
<body>
  <h1>Welcome!</h1>
</body>
</html>
```

**Test cases**

* Heading is horizontally centered.
* Works for all screen sizes.

**Complete Solution**

```html
<style>
  h1 {
    text-align: center;
  }
</style>
```

---

Great 👍
Here’s the next batch: **Q13 – Q18** (Box Model + Intro to Flexbox).
Same structure: **Problem → Starter → Test Cases → Complete Solution**

---

# 📘 HTML & CSS Practice Sheet (Q13 – Q18)

---

## Q13) The Box Model

**Problem Description**
You’re designing a profile card. To make it look neat, you must apply **padding** inside the box, a **border** around it, and a **margin** outside it.

This exercise teaches the **box model** — one of the most fundamental CSS concepts.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q13 - Box Model</title>
<style>
  div {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <div>Profile Card</div>
</body>
</html>
```

**Test cases**

* Box has padding inside.
* Box has a border.
* Box has margin outside.

**Complete Solution**

```css
div {
  padding: 20px;
  border: 5px solid black;
  margin: 15px;
}
```

---

## Q14) Consistent Box Size

**Problem Description**
You’re building a button container that must always stay **200px wide**, even if padding is applied. Use `box-sizing` to ensure the width stays consistent.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q14 - Box Sizing</title>
<style>
  div {
    width: 200px;
    padding: 20px;
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <div>Button</div>
</body>
</html>
```

**Test cases**

* Total width remains `200px`.
* Padding is included inside the box.

**Complete Solution**

```css
div {
  width: 200px;
  padding: 20px;
  box-sizing: border-box;
  border: 2px solid #444;
}
```

---

## Q15) Modern Card

**Problem Description**
Design a modern “card” UI element with a **border, padding, margin, rounded corners, and shadow** (like those seen on e-commerce sites).

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q15 - Modern Card</title>
<style>
  .card {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <div class="card">Product Information</div>
</body>
</html>
```

**Test cases**

* Card has border and padding.
* Card has margin.
* Card has shadow + rounded corners.

**Complete Solution**

```css
.card {
  border: 1px solid #ddd;
  padding: 20px;
  margin: 15px;
  border-radius: 8px;
  box-shadow: 2px 2px 6px gray;
}
```

---

## Q16) Navigation Bar

**Problem Description**
You’re asked to create a **horizontal navigation bar** where links are spaced evenly. This is a common use of **Flexbox**.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q16 - Navigation Bar</title>
<style>
  nav {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>
</body>
</html>
```

**Test cases**

* Links are displayed horizontally.
* Equal spacing between them.

**Complete Solution**

```css
nav {
  display: flex;
  justify-content: space-around;
  background: #4f46e5;
  padding: 10px;
}
nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}
```

---

## Q17) Vertical Alignment

**Problem Description**
You need to build a hero section where a **message box is vertically centered** inside the page.

This is a very common flexbox trick.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q17 - Vertical Centering</title>
<style>
  .container {
    height: 300px;
    background: #eee;
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <div class="container">
    <div class="box">Welcome Message</div>
  </div>
</body>
</html>
```

**Test cases**

* Box is vertically centered inside container.
* Box remains centered even if container height changes.

**Complete Solution**

```css
.container {
  display: flex;
  align-items: center;
  justify-content: center;
}
.box {
  background: #4f46e5;
  color: white;
  padding: 20px;
  border-radius: 6px;
}
```

---

## Q18) Equal Columns

**Problem Description**
You’re creating a 3-column layout where each column must take equal width, regardless of content size.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q18 - Equal Columns</title>
<style>
  .container {
    /* Write your CSS here */
  }
  .box {
    border: 1px solid #000;
    padding: 10px;
  }
</style>
</head>
<body>
  <div class="container">
    <div class="box">Column 1</div>
    <div class="box">Column 2</div>
    <div class="box">Column 3</div>
  </div>
</body>
</html>
```

**Test cases**

* All 3 boxes are equal width.
* Layout uses flexbox.

**Complete Solution**

```css
.container {
  display: flex;
}
.container .box {
  flex: 1;
}
```

---
Perfect 🚀
Let’s continue with **Q19 – Q24 (CSS Grid, Media Queries, Positioning & Specificity)**.
Same structure: **Problem → Starter → Test Cases → Complete Solution**

---

# 📘 HTML & CSS Practice Sheet (Q19 – Q24)

---

## Q19) Photo Grid

**Problem Description**
You’re designing a photo gallery where images should be arranged in a **2x2 grid layout**.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q19 - Photo Grid</title>
<style>
  .gallery {
    /* Write your CSS here */
  }
  .photo {
    background: #4f46e5;
    color: white;
    display: grid;
    place-items: center;
    height: 100px;
  }
</style>
</head>
<body>
  <div class="gallery">
    <div class="photo">1</div>
    <div class="photo">2</div>
    <div class="photo">3</div>
    <div class="photo">4</div>
  </div>
</body>
</html>
```

**Test cases**

* 4 boxes arranged in 2x2 grid.
* Equal spacing between boxes.

**Complete Solution**

```css
.gallery {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
}
```

---

## Q20) Responsive Stack

**Problem Description**
On a large screen, two content boxes should sit **side by side**, but on small screens (mobile), they should **stack vertically**.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q20 - Responsive Stack</title>
<style>
  .container {
    display: grid;
    /* Write default grid here */
  }
  .box {
    background: #4f46e5;
    color: white;
    padding: 20px;
    text-align: center;
  }
</style>
</head>
<body>
  <div class="container">
    <div class="box">Box 1</div>
    <div class="box">Box 2</div>
  </div>
</body>
</html>
```

**Test cases**

* Two columns on desktop.
* One column on mobile (≤600px).

**Complete Solution**

```css
.container {
  grid-template-columns: 1fr 1fr;
  gap: 10px;
}
@media (max-width: 600px) {
  .container {
    grid-template-columns: 1fr;
  }
}
```

---

## Q21) Gallery of Nine

**Problem Description**
You’re creating a **gallery of 9 images** in a 3-column grid layout.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q21 - Gallery of Nine</title>
<style>
  .gallery {
    /* Write your CSS here */
  }
  .item {
    background: #4f46e5;
    color: white;
    height: 80px;
    display: grid;
    place-items: center;
  }
</style>
</head>
<body>
  <div class="gallery">
    <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>
    <div class="item">4</div>
    <div class="item">5</div>
    <div class="item">6</div>
    <div class="item">7</div>
    <div class="item">8</div>
    <div class="item">9</div>
  </div>
</body>
</html>
```

**Test cases**

* 3 equal columns.
* Items arranged neatly with gaps.

**Complete Solution**

```css
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}
```

---

## Q22) Corner Box

**Problem Description**
You are designing a dashboard widget. A small **notification box** must appear at the **top-right corner** of a larger container.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q22 - Corner Box</title>
<style>
  .container {
    width: 400px;
    height: 200px;
    background: #eee;
    position: relative;
  }
  .box {
    width: 80px;
    height: 40px;
    background: #4f46e5;
    color: white;
    display: grid;
    place-items: center;
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <div class="container">
    <div class="box">Hi</div>
  </div>
</body>
</html>
```

**Test cases**

* Box is positioned at the top-right corner inside container.

**Complete Solution**

```css
.box {
  position: absolute;
  top: 10px;
  right: 10px;
}
```

---

## Q23) Sticky Navbar

**Problem Description**
You’re building a blog with a **navigation bar** that stays at the top of the screen even when scrolling (sticky behavior).

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q23 - Sticky Navbar</title>
<style>
  nav {
    background: #4f46e5;
    color: white;
    padding: 10px;
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <nav>My Sticky Navbar</nav>
  <div style="height:1500px;">Scroll down...</div>
</body>
</html>
```

**Test cases**

* Navbar sticks to the top when scrolling.
* Content scrolls below it.

**Complete Solution**

```css
nav {
  position: sticky;
  top: 0;
}
```

---

## Q24) Style Fight

**Problem Description**
You’re testing CSS **specificity rules**. A paragraph has 3 styles:

* Element selector (blue)
* Class selector (green)
* ID selector (red)

Which one will win?

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q24 - Style Fight</title>
<style>
  p { color: blue; }
  .text { color: green; }
  #unique { /* Write your CSS here */ }
</style>
</head>
<body>
  <p id="unique" class="text">This is styled text.</p>
</body>
</html>
```

**Test cases**

* The paragraph text should be red because ID > Class > Element.

**Complete Solution**

```css
#unique {
  color: red;
}
```

---
Perfect 👍
Here’s the **final stretch (Q25 – Q33: Mixed Practice, Forms, Buttons, Hero Section, Responsive Cards)**.
Same structure: **Problem → Starter → Test Cases → Complete Solution**

---

# 📘 HTML & CSS Practice Sheet (Q25 – Q33)

---

## Q25) Login Box

**Problem Description**
You’re creating a login form for a website. It should have:

* A username field
* A password field
* A login button
  All inside a **styled centered box**.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q25 - Login Box</title>
<style>
  .login {
    width: 200px;
    margin: auto;
    margin-top: 100px;
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <form class="login">
    <!-- Write your code here -->
  </form>
</body>
</html>
```

**Test cases**

* Form has username + password inputs.
* Button labeled “Login”.
* Box has border and padding.

**Complete Solution**

```html
<form class="login">
  <input type="text" placeholder="Username"><br>
  <input type="password" placeholder="Password"><br>
  <button>Login</button>
</form>

<style>
  .login {
    width: 200px;
    margin: auto;
    margin-top: 100px;
    padding: 20px;
    border: 1px solid gray;
    border-radius: 8px;
  }
  .login input {
    display: block;
    margin: 10px 0;
    width: 100%;
  }
</style>
```

---

## Q26) Responsive Flex Columns

**Problem Description**
You need a **3-column layout** that shrinks gracefully on smaller screens using **flexbox wrapping**.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q26 - Responsive Flex Columns</title>
<style>
  .container {
    display: flex;
    /* Write your CSS here */
  }
  .box {
    background: #4f46e5;
    color: white;
    padding: 20px;
    margin: 10px;
  }
</style>
</head>
<body>
  <div class="container">
    <div class="box">1</div>
    <div class="box">2</div>
    <div class="box">3</div>
  </div>
</body>
</html>
```

**Test cases**

* 3 columns side by side on desktop.
* Boxes wrap into rows on smaller screens.

**Complete Solution**

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
.box {
  flex: 1 1 30%;
}
```

---

## Q27) Footer Bar

**Problem Description**
You’re building a **website footer**. It should span full width, have dark background, and white text, centered horizontally.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q27 - Footer Bar</title>
<style>
  footer {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <footer>© 2025 My Website</footer>
</body>
</html>
```

**Test cases**

* Footer has dark background.
* Text is centered and white.

**Complete Solution**

```css
footer {
  background: #222;
  color: white;
  text-align: center;
  padding: 10px;
}
```

---

## Q28) Hover Button

**Problem Description**
Create a button with a **hover effect**. On hover, its background should darken.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q28 - Hover Button</title>
<style>
  button {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <button>Click Me</button>
</body>
</html>
```

**Test cases**

* Button has initial background.
* On hover, background becomes darker.

**Complete Solution**

```css
button {
  background: blue;
  color: white;
  padding: 10px;
  border: none;
  border-radius: 5px;
}
button:hover {
  background: darkblue;
}
```

---

## Q29) Hero Section

**Problem Description**
You need a **hero section** for a landing page. It should use a **background image**, center the text inside, and have large white text.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q29 - Hero Section</title>
<style>
  .hero {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <div class="hero">
    <h1>Welcome to Our Website</h1>
  </div>
</body>
</html>
```

**Test cases**

* Background image covers whole hero area.
* Text is centered (both axes).
* Text color is white.

**Complete Solution**

```css
.hero {
  background: url('hero.jpg') no-repeat center/cover;
  height: 400px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-size: 2em;
}
```

---

## Q30) Responsive Cards

**Problem Description**
You’re making a **card grid** that adapts:

* 4 cards per row on desktop
* 2 per row on tablet
* 1 per row on mobile

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q30 - Responsive Cards</title>
<style>
  .cards {
    /* Write your CSS here */
  }
  .card {
    background: #4f46e5;
    color: white;
    height: 100px;
    display: grid;
    place-items: center;
  }
</style>
</head>
<body>
  <div class="cards">
    <div class="card">1</div>
    <div class="card">2</div>
    <div class="card">3</div>
    <div class="card">4</div>
  </div>
</body>
</html>
```

**Test cases**

* 4 columns on desktop.
* 2 columns on tablet.
* 1 column on mobile.

**Complete Solution**

```css
.cards {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
}
@media (max-width: 800px) {
  .cards {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media (max-width: 500px) {
  .cards {
    grid-template-columns: 1fr;
  }
}
```

---

## Q31) Colored Boxes

**Problem Description**
You are asked to create **three boxes** of equal size arranged side by side with different background colors (red, green, blue).

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q31 - Colored Boxes</title>
<style>
  .container {
    /* Write your CSS here */
  }
  .box {
    flex: 1;
    height: 100px;
  }
</style>
</head>
<body>
  <div class="container">
    <div class="box" style="background:red;"></div>
    <div class="box" style="background:green;"></div>
    <div class="box" style="background:blue;"></div>
  </div>
</body>
</html>
```

**Test cases**

* Boxes are side by side.
* Each takes equal width.

**Complete Solution**

```css
.container {
  display: flex;
}
```

---

## Q32) Notification Badge

**Problem Description**
Create a **bell icon with a red circular badge** at its top-right corner showing “3” notifications.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q32 - Notification Badge</title>
<style>
  .icon {
    position: relative;
    font-size: 40px;
  }
  .badge {
    /* Write your CSS here */
  }
</style>
</head>
<body>
  <div class="icon">🔔
    <span class="badge">3</span>
  </div>
</body>
</html>
```

**Test cases**

* Badge is a small red circle.
* Badge positioned at top-right of bell.

**Complete Solution**

```css
.badge {
  position: absolute;
  top: -5px;
  right: -10px;
  background: red;
  color: white;
  border-radius: 50%;
  padding: 2px 6px;
  font-size: 12px;
}
```

---

## Q33) Equal Height Columns

**Problem Description**
You are asked to create 3 columns with different text lengths, but they must all have the **same height** using flexbox.

**Starter (stub)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Q33 - Equal Height Columns</title>
<style>
  .container {
    /* Write your CSS here */
  }
  .col {
    flex: 1;
    border: 1px solid #000;
    padding: 10px;
  }
</style>
</head>
<body>
  <div class="container">
    <div class="col">Short text</div>
    <div class="col">This column has more text than the first one.</div>
    <div class="col">This one has the longest text, but should still match height.</div>
  </div>
</body>
</html>
```

**Test cases**

* All columns same height.
* Uses flexbox, not fixed heights.

**Complete Solution**

```css
.container {
  display: flex;
  align-items: stretch;
}
```

---








