# **Teacher Guide – Recap: Weeks 1, 2, and 3**

## **Introduction**

This guide is designed to help instructors recap the core concepts and techniques covered in Weeks 1, 2, and 3. Over these weeks, students built and styled an e-commerce store, learning the fundamentals of **HTML** and **CSS**, as well as advanced layout techniques.

---

## **Teaching Objectives**

1. **Understand Semantic HTML**:

   - Teach the importance of using semantic elements like `<header>`, `<main>`, and `<footer>` for accessibility and structure.
   - Show how semantic tags improve document readability and SEO.

2. **Apply CSS Fundamentals**:

   - Guide students in using selectors, the box model, and styling properties to create visually appealing designs.

3. **Explore Advanced Layouts**:

   - Use Flexbox for aligning navigation bars.
   - Implement CSS Grid for responsive product layouts.

4. **Introduce Responsive Design**:
   - Explain the role of media queries in adapting designs to different screen sizes.
   - Highlight mobile-first design principles.

---

## **Classroom Flow**

### **1. Semantic HTML (Week 1)**

Start by explaining the role of semantic HTML in creating accessible and maintainable web pages:

- **Key Elements**:
  - `<header>`: For branding and navigation.
  - `<main>`: For core content like product listings.
  - `<footer>`: For additional information like contact details.

**Code Example**:

```html
<header>
  <img src="logo.png" alt="E-Commerce Logo" />
  <nav>
    <a href="#">Home</a>
    <a href="#">Products</a>
    <a href="#">Contact</a>
  </nav>
</header>
```

#### **Discussion Prompts**:

- Why is semantic HTML important for accessibility?
- How do semantic tags improve SEO?

---

### **2. Styling Basics (Week 2)**

Explain how CSS enhances the structure built in Week 1:

- **Key Concepts**:
  - Selectors: Element, class, and ID selectors.
  - Box Model: Padding, borders, and margin for layout control.
  - Styling basics: Colors, fonts, and spacing.

**Code Example**:

```css
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #333;
  color: white;
}
```

#### **Teaching Tips**:

- Demonstrate the effect of the box model on layout and spacing.
- Show how flexbox properties like `justify-content` align content.

---

### **3. Advanced Layout Techniques (Week 3)**

Guide students in creating responsive layouts using Flexbox and Grid:

- **Key Concepts**:
  - Flexbox: Aligning navigation links and footer content.
  - CSS Grid: Structuring product listings dynamically.
  - Media Queries: Adapting designs to smaller screens.

**Code Example**:

```css
section {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

@media (max-width: 768px) {
  nav {
    flex-direction: column;
    align-items: flex-start;
  }
}
```

#### **Teaching Tips**:

- Explain the difference between `auto-fit` and `auto-fill` in grid layouts.
- Emphasize the importance of responsive design for user experience.

---

### **4. Adding Interactivity**

Introduce hover effects for navigation links and buttons:

- **Key Concepts**:
  - Pseudo-classes like `:hover` for interactive elements.
  - Visual feedback for buttons and links.

**Code Example**:

```css
main article a:hover {
  background-color: #555;
  color: white;
}
```

#### **Discussion Prompts**:

- Why is visual feedback important for user interaction?
- How can hover effects improve accessibility?

---

## **Common Mistakes to Address**

1. **Misuse of Selectors**:

   - Ensure students understand when to use element, class, or ID selectors.

2. **Inconsistent Spacing**:

   - Highlight the importance of uniform padding and margins.

3. **Neglecting Responsiveness**:
   - Stress the importance of testing designs on different screen sizes.

---

## **Learning Outcomes**

By the end of this recap, students should be able to:

1. Build semantic and accessible HTML structures.
2. Style layouts using CSS fundamentals and advanced techniques.
3. Create responsive designs with CSS Grid and media queries.
4. Add interactivity with hover effects.

---

## **Additional Resources**

- **HTML Basics**: [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- **CSS Selectors and Properties**: [CSS Tricks](https://css-tricks.com/)
- **Responsive Design**: [MDN Web Docs - Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)
- **CSS Grid**: [CSS Tricks - Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

---
