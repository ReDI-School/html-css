# **Teacher Guide – Week 2: CSS Basics**

## **Introduction**

This guide is designed to help instructors teach students the basics of CSS by styling the e-commerce store skeleton built in Week 1. The lesson focuses on fundamental concepts like selectors, the box model, styling basics, and responsive design.

---

## **Teaching Objectives**

1. **Understand CSS Selectors**:

   - Teach the difference between element, class, and pseudo-class selectors.
   - Demonstrate their practical application in styling specific components.

2. **Apply the Box Model**:

   - Explain the concepts of padding, margin, borders, and `box-sizing`.
   - Show how these properties affect spacing and layout.

3. **Introduce Styling Basics**:

   - Guide students in adding colors, fonts, and background styles for better visual appeal.
   - Discuss the importance of cohesive design.

4. **Implement Responsive Design**:
   - Use CSS Grid to create a dynamic layout for product listings.
   - Highlight the role of `auto-fit` and `minmax` in making designs adaptable to screen sizes.

---

## **Classroom Flow**

### **1. CSS Fundamentals**

Start by explaining the role of CSS in enhancing HTML:

- **Why CSS Matters**: Introduce its role in styling and layout.
- **Basic Syntax**:
  - CSS Rules: Selectors, properties, and values.
  - Example:
    ```css
    body {
      font-family: Arial, sans-serif;
      color: #333;
    }
    ```

#### **Discussion Prompts**:

- What is the difference between inline, internal, and external CSS?
- Why is it a good practice to use external stylesheets?

---

### **2. Styling the Header**

Demonstrate how to style the `<header>` for branding and navigation:

- **Key Concepts**:
  - Flexbox for alignment and spacing.
  - Background and text color for contrast.

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
header nav a {
  color: white;
  text-decoration: none;
  margin-left: 15px;
}
```

#### **Teaching Tips**:

- Explain how `justify-content: space-between` ensures even spacing.
- Show how `text-decoration: none` improves readability of navigation links.

---

### **3. Styling the Main Section**

Guide students in styling the product listing section:

- **Key Concepts**:
  - Using CSS Grid for responsive layouts.
  - Adding borders and padding for clarity.

**Code Example**:

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

#### **Teaching Tips**:

- Explain the significance of `auto-fit` and `minmax` in creating flexible grid layouts.
- Discuss how `gap` improves spacing between grid items.

---

### **4. Adding Interactivity**

Introduce hover effects for buttons and links:

- **Key Concepts**:
  - Use of pseudo-classes like `:hover`.
  - Styling buttons to improve user interaction.

**Code Example**:

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

#### **Teaching Tips**:

- Emphasize the importance of visual feedback for interactive elements.
- Encourage students to experiment with different hover styles.

---

### **5. Styling the Footer**

Create a cohesive footer design that matches the header:

- **Key Concepts**:
  - Consistent background color and padding.
  - Center-aligned text for simplicity.

**Code Example**:

```css
footer {
  text-align: center;
  padding: 10px;
  background-color: #333;
  color: white;
  margin-top: 20px;
}
```

---

## **Common Mistakes to Address**

1. **Improper Use of Selectors**:
   - Ensure students understand when to use element, class, or ID selectors.
2. **Inconsistent Spacing**:
   - Highlight the role of `padding` and `margin` in maintaining uniformity.
3. **Neglecting Responsiveness**:
   - Stress the importance of testing designs on different screen sizes.

---

## **Learning Outcomes**

By the end of the lesson, students should:

1. Style the e-commerce store skeleton using CSS.
2. Apply the box model to manage spacing and layout.
3. Create responsive designs using CSS Grid.
4. Enhance user interaction with hover effects.

---

## **Additional Resources**

- **CSS Basics**: [MDN Web Docs - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- **CSS Grid Guide**: [CSS Tricks - Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
- **Flexbox Reference**: [CSS Tricks - Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

---
