# **Milestone 2: CSS Basics – Styling the E-Commerce Store**

## **Objective**

- Apply **CSS fundamentals** to style the HTML skeleton of the e-commerce store built in Milestone 1.
- Focus on:
  - CSS **selectors** and **properties**.
  - The **box model** for spacing and layout.
  - Adding **colors**, **fonts**, and **basic spacing**.

---

## **Project Overview**

This project enhances the HTML skeleton created in Milestone 1 by adding styles using CSS. The focus is on the fundamental concepts of CSS to make the website visually appealing and structured.


## 🗂️ Folder Structure

```plaintext
02_milestone/
│
├── index.html           # Main HTML file for the milestone
├── style.css            # CSS file for styling the HTML
├── logo.png             # Logo image used in the header
├── .jpg                 # Sample Product images
└── README.md            # Milestone documentation
```

---

## **Updated Project Code**

### **1. Updated `index.html`**

We link the `style.css` file created in Milestone 1 and update the file structure slightly for styling purposes.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>E-Commerce Store</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header>
      <img src="logo.png" alt="E-Commerce Logo" width="100" />
      <nav>
        <a href="#">Home</a>
        <a href="#">Products</a>
        <a href="#">Contact</a>
      </nav>
    </header>
    <main>
      <section>
        <article>
          <h2>Product 1</h2>
          <img src="product1.jpg" alt="Image of Product 1" width="150" />
          <p>A short description of Product 1.</p>
          <a href="#">Add to Cart</a>
        </article>
        <article>
          <h2>Product 2</h2>
          <img src="product2.jpg" alt="Image of Product 2" width="150" />
          <p>A short description of Product 2.</p>
          <a href="#">Add to Cart</a>
        </article>
        <article>
          <h2>Product 3</h2>
          <img src="product3.jpg" alt="Image of Product 3" width="150" />
          <p>A short description of Product 3.</p>
          <a href="#">Add to Cart</a>
        </article>
        <article>
          <h2>Product 4</h2>
          <img src="product4.jpg" alt="Image of Product 4" width="150" />
          <p>A short description of Product 4.</p>
          <a href="#">Add to Cart</a>
        </article>
      </section>
    </main>
    <footer>
      <p>
        Contact us: <a href="mailto:info@ecommerce.com">info@ecommerce.com</a>
      </p>
      <p>&copy; 2025 E-Commerce Store</p>
    </footer>
  </body>
</html>
```

---

### **2. `style.css`**

We style the e-commerce store using CSS. Focus on colors, fonts, and spacing, as well as the box model.

```css
/* General styles */
body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Header styles */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #333;
  color: white;
}

header img {
  height: 50px;
}

header nav a {
  color: white;
  text-decoration: none;
  margin-left: 15px;
}

/* Main content styles */
main {
  padding: 20px;
}

main section {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

main article {
  border: 1px solid #ddd;
  padding: 15px;
  text-align: center;
  background-color: #f9f9f9;
  border-radius: 5px;
}

main article img {
  max-width: 100%;
  height: auto;
}

main article a {
  display: inline-block;
  margin-top: 10px;
  padding: 5px 10px;
  background-color: #333;
  color: white;
  text-decoration: none;
  border-radius: 3px;
}

/* Footer styles */
footer {
  text-align: center;
  padding: 10px;
  background-color: #333;
  color: white;
  margin-top: 20px;
}
```

---

## **Core Concepts Demonstrated**

1. **CSS Selectors**:

   - Element selectors (e.g., `body`, `header`, `footer`).
   - Class selectors (e.g., `.article`).
   - Pseudo-classes (e.g., `a:hover`).

2. **Box Model**:

   - Padding and margin for spacing.
   - Borders for visual boundaries.
   - `box-sizing` to ensure predictable layouts.

3. **Styling Basics**:

   - Background colors for elements (e.g., header and footer).
   - Font customization using `font-family`.
   - Button and link styling.

4. **Responsive Layout**:
   - Grid layout with `grid-template-columns`.
   - Use of `auto-fit` and `minmax` for flexible, responsive design.

---

## **Resources**

1. **CSS Flexbox**: [CSS Tricks Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
2. **Responsive Layouts**: [CSS Tricks Responsiveness](https://css-tricks.com/responsive-layouts-fewer-media-queries/)

---

## **Expected Output**

A styled e-commerce website skeleton with:

- A colored and spaced header.
- Styled product listings with borders, padding, and consistent spacing.
- A footer with a consistent color theme.
- Responsive design for product listings using a grid layout.
