# **Recap: Weeks 1, 2, and 3 – Building and Styling an E-Commerce Store**

## **Overview**

In the first three weeks, we progressively built and styled an e-commerce store using **HTML** and **CSS**. This recap summarizes the key objectives, concepts, and steps covered in each Milestone.

---

## **Milestone 1: Building the Skeleton**

### **Objective**

- Create the foundational HTML structure for the e-commerce store.
- Use **semantic HTML** for better accessibility and maintainability.

### **Key Features**

- **Header**: Logo and navigation links.
- **Main Content**: Product listing section with semantic tags (`<article>`, `<section>`).
- **Footer**: Contact information.

### **Key Code Snippet**

```html
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
      <img src="product1.jpg" alt="Image of Product 1" />
      <p>A short description of Product 1.</p>
      <a href="#">Add to Cart</a>
    </article>
  </section>
</main>

<footer>
  <p>Contact us: <a href="mailto:info@ecommerce.com">info@ecommerce.com</a></p>
  <p>&copy; 2025 E-Commerce Store</p>
</footer>
```

---

## **Milestone 2: Adding Basic Styling**

### **Objective**

- Style the HTML skeleton using **CSS**.
- Focus on basic concepts like **selectors**, **properties**, and the **box model**.

### **Key Features**

- Added colors, fonts, and spacing to enhance visual appeal.
- Styled the header, main content, and footer.
- Introduced **hover effects** for links.

### **Key Code Snippet**

```css
/* Header */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #333;
  color: white;
}

nav a {
  color: white;
  text-decoration: none;
  margin-left: 15px;
}

/* Product Card */
article {
  border: 1px solid #ddd;
  padding: 15px;
  background-color: #f9f9f9;
  border-radius: 5px;
}
```

---

## **Milestone 3: Advanced Layout**

### **Objective**

- Enhance the layout using **Flexbox**, **Grid**, and responsive design techniques.
- Add **classes** and **IDs** for better code organization and specific styling.

### **Key Features**

- **Navigation Bar**: Aligned using Flexbox.
- **Product Section**: Styled with CSS Grid for a dynamic and responsive layout.
- Added **media queries** to ensure responsiveness.

### **Key Code Snippet**

```css
/* Responsive Grid */
section {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

/* Media Queries */
@media (max-width: 768px) {
  nav {
    flex-direction: column;
  }
}
```

---

## **Key Concepts Recap**

1. **Semantic HTML**

   - Tags like `<header>`, `<section>`, and `<footer>` improve accessibility and structure.

2. **CSS Fundamentals**

   - Selectors: Element, class, and ID selectors.
   - Box Model: Padding, border, margin, and content.
   - Pseudo-classes: `:hover` for interactive effects.

3. **Advanced Layout**
   - Flexbox: Aligning navigation links.
   - Grid: Creating a responsive product layout.
   - Media Queries: Ensuring the design adapts to all screen sizes.

---

## **Challenges and Learnings**

- Structuring content semantically improves readability and accessibility.
- Basic CSS styling lays the groundwork for advanced layout techniques.
- Responsive design ensures the site is user-friendly on all devices.

---

## **Resources**

1. **HTML Basics**: [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
2. **CSS Selectors and Properties**: [CSS Tricks](https://css-tricks.com/)
3. **Responsive Design**: [MDN Web Docs - Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)
4. **CSS Grid**: [CSS Tricks - Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

---
