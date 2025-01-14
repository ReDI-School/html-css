# **Recap: Weeks 1, 2, and 3 – Project Guide**

## **Overview**

This guide summarizes the core concepts and project outputs from Weeks 1, 2, and 3. The focus was on creating an e-commerce store skeleton in Milestone 1, styling it with CSS basics in Milestone 2, and enhancing its layout with advanced techniques in Milestone 3.

---

## **Core Concepts Demonstrated**

1. **Semantic HTML (Milestone 1)**:

   - Using semantic elements (`<header>`, `<main>`, `<footer>`) to improve accessibility and document structure.
   - Creating a logical and readable HTML skeleton.

2. **CSS Fundamentals (Milestone 2)**:

   - Applying CSS selectors (element, class, ID) for targeted styling.
   - Understanding and using the box model (padding, margin, borders) to manage layout spacing.

3. **Advanced Layout Techniques (Milestone 3)**:
   - Using Flexbox for aligning content (e.g., navigation bar).
   - Implementing CSS Grid for responsive product layouts.
   - Introducing media queries to adapt designs for different screen sizes.

---

## **File Breakdown**

### **1. `index.html`**

The HTML file provides the structure for the e-commerce store, including sections for the header, product listings, and footer.

#### **Key Features**:

- Logical grouping of elements using semantic tags.
- Placeholder content for product listings.

**Code Snippet:**

```html
<header>
  <img src="logo.png" alt="E-Commerce Logo" />
  <nav>
    <a href="#">Home</a>
    <a href="#">Products</a>
    <a href="#">Contact</a>
  </nav>
</header>

<main>
  <section id="products">
    <article>
      <h2>Product 1</h2>
      <img src="product1.jpg" alt="Image of Product 1" />
      <p>Description of Product 1.</p>
      <a href="#">Add to Cart</a>
    </article>
  </section>
</main>

<footer>
  <p>Contact us: <a href="mailto:info@ecommerce.com">info@ecommerce.com</a></p>
</footer>
```

---

### **2. `style.css`**

This file progressively evolves across the three weeks, starting with basic styling and advancing to responsive layouts.

#### **Header Styling**

- **Purpose**: Create a visually appealing navigation bar.
- **Key Features**:
  - Flexbox alignment.
  - Styling links for better readability.

**Code Snippet:**

```css
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #333;
  color: white;
}
header nav a {
  color: white;
  text-decoration: none;
  margin-left: 15px;
}
```

#### **Product Section Styling**

- **Purpose**: Display products in a responsive grid layout.
- **Key Features**:
  - CSS Grid for structure.
  - Borders and padding to define product boundaries.

**Code Snippet:**

```css
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
```

#### **Footer Styling**

- **Purpose**: Create a cohesive footer that matches the header design.
- **Key Features**:
  - Background color for consistency.
  - Center-aligned text.

**Code Snippet:**

```css
footer {
  text-align: center;
  padding: 10px;
  background-color: #333;
  color: white;
}
```

#### **Interactive Elements**

- **Purpose**: Add hover effects for better user experience.
- **Key Features**:
  - Button-like styling for links.
  - Visual feedback using hover effects.

**Code Snippet:**

```css
main article a {
  display: inline-block;
  margin-top: 10px;
  padding: 5px 10px;
  background-color: #333;
  color: white;
  text-decoration: none;
  border-radius: 3px;
}
main article a:hover {
  background-color: #555;
}
```

---

## **Discussion Points**

1. **Semantic HTML**: Why are semantic tags essential for accessibility and SEO?
2. **Box Model**: How does `box-sizing: border-box` simplify layout spacing?
3. **Responsive Design**: How do Flexbox and Grid create adaptive layouts?
4. **Hover Effects**: How do pseudo-classes like `:hover` improve user interaction?

---

## **Expected Output**

By the end of Milestone 3, the e-commerce website should:

- Include a styled header, footer, and product section.
- Be fully responsive, adjusting to various screen sizes.
- Feature interactive buttons and links.

---
