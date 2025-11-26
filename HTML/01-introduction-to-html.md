# 📌 **What is HTML?**

**HTML (HyperText Markup Language)** is the standard language used to **structure content** on the web.
It is NOT a programming language — it **doesn’t contain logic** like loops or conditions.
Instead, HTML **describes what content is**: headings, paragraphs, images, buttons, links, etc.

Think of HTML as:

* **The skeleton of a webpage**
* Defines *what* appears on the page
* Works together with **CSS** (appearance) and **JavaScript** (behavior)

---

# 📌 **Why HTML is used?**

HTML is used to:

### ✔️ **Structure content**

Example:

* Title → `<h1>`
* Paragraph → `<p>`
* Image → `<img>`
* Section → `<section>`

### ✔️ **Define meaning (semantic HTML)**

Elements like `<header>`, `<main>`, `<article>`, `<nav>` help browsers & screen readers understand the page.

### ✔️ **Link pages together**

Using `<a href="...">`.

### ✔️ **Embed media**

Images, videos, audio.

### ✔️ **Make pages interactive when combined with JavaScript**

HTML provides objects that JS can manipulate.

### ✔️ **Platform independence**

Every device with a browser can read HTML.

---

# 📌 **How browsers read HTML (Render Pipeline)**

When you open a webpage, the browser follows these steps:

---

### 🧠 **1. Load the HTML file**

Browser downloads `index.html`.

---

### 🧠 **2. Parse HTML → Build the DOM**

DOM = **Document Object Model**
It is a tree-like structure created from HTML.

Example HTML:

```html
<h1>Hello World</h1>
<p>This is a page</p>
```

DOM representation:

```
Document
 └── html
      └── body
           ├── h1 ("Hello World")
           └── p ("This is a page")
```

---

### 🧠 **3. Load & parse CSS → Build the CSSOM**

CSS rules (color, layout, fonts) form another tree.

---

### 🧠 **4. Combine DOM + CSSOM → Render Tree**

Browser calculates:

* Size
* Position
* Colors
* Fonts

For every element.

---

### 🧠 **5. Painting**

Browser draws the pixels on screen.

---

### 🧠 **6. JavaScript executes**

JS can update the DOM (like when a button is clicked), and the browser re-renders only changed parts.

---

# 📌 **HTML File Structure (`index.html`)**

Every HTML page has a basic skeleton.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Page</title>
</head>
<body>

    <h1>Hello World</h1>
    <p>This is my first HTML page.</p>

</body>
</html>
```

### Breakdown:

| Part              | Meaning                                |
| ----------------- | -------------------------------------- |
| `<!DOCTYPE html>` | Tells browser this is an HTML5 file    |
| `<html>`          | Root of the entire webpage             |
| `<head>`          | Metadata (title, links, character set) |
| `<title>`         | Appears on browser tab                 |
| `<meta>`          | Info for browser & SEO                 |
| `<body>`          | ALL visible content goes here          |

---

# 📌 **Tags, Elements, Attributes**

HTML is built using **tags**.

Example:

```html
<p>Hello</p>
```

## ✔️ **Tag**

`<p>` and `</p>` are tags.

## ✔️ **Element**

The complete structure (opening tag + content + closing tag) is an **element**.

```html
<p>Hello</p>
```

This whole thing is a **paragraph element**.

## ✔️ **Attributes**

Attributes give **extra information** about elements.

Example:

```html
<img src="photo.jpg" alt="A photo" width="300">
```

Here:

| Attribute | Meaning                                                 |
| --------- | ------------------------------------------------------- |
| `src`     | Path to image file                                      |
| `alt`     | Text shown if image fails (important for accessibility) |
| `width`   | Sets size                                               |

Attributes always appear inside the **opening tag**.

---
