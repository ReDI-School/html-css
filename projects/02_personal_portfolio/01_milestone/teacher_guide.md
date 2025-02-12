# **Teacher Guide – Milestone 1: HTML & CSS – Personal Portfolio**

## **Introduction**

This guide helps instructors teach students how to create the foundation of a personal portfolio website. The focus is on semantic HTML, accessible forms, and advanced CSS styling, ensuring students build a well-structured, user-friendly webpage.

---

## **Teaching Objectives**

1. **Semantic HTML**:

   - Teach the importance of semantic tags like `<header>`, `<section>`, `<form>`, and `<footer>` for clear structure and accessibility.
   - Guide students in organizing content logically with proper labels and grouping.

2. **Accessibility**:

   - Explain the use of ARIA attributes like `aria-required="true"` to assist users with screen readers.
   - Demonstrate how focus states improve usability for keyboard navigation.

3. **Advanced CSS Selectors**:

   - Introduce pseudo-classes like `:hover` and `:focus` for interactivity.
   - Show how to style forms and inputs for consistency and accessibility.

4. **Forms**:
   - Guide students in creating accessible and functional forms with input validation using the `required` attribute.

---

## **Classroom Flow**

### **1. Semantic HTML**

Start by explaining the importance of semantic HTML for accessibility and SEO:

- **Key Concepts**:
  - Use of `<header>` for branding and navigation.
  - `<section>` for logical grouping of content.
  - `<form>` for collecting user input.

**Teaching Tips**:

- Highlight how `<label>` improves accessibility by associating text with input fields.
- Show how semantic tags enhance document readability and maintainability.

**Code Example**:

```html
<section id="contact" class="contact-section">
  <h2>Contact Me</h2>
  <form action="#" method="POST" class="contact-form">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required aria-required="true" />

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required aria-required="true" />

    <label for="message">Message:</label>
    <textarea
      id="message"
      name="message"
      rows="5"
      required
      aria-required="true"
    ></textarea>

    <button type="submit" class="submit-button">Send Message</button>
  </form>
</section>
```

---

### **2. Styling with CSS**

Guide students in styling the layout and forms using CSS:

- **Header and Navigation**:
  - Flexbox for aligning logo and navigation links.
  - Hover effects for links to improve interactivity.

**Code Example**:

```css
.site-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #333;
  color: white;
}

.navbar .nav-link {
  color: white;
  text-decoration: none;
  margin-left: 20px;
}

.navbar .nav-link:hover {
  text-decoration: underline;
}
```

- **Contact Form Styling**:
  - Use block-level labels for clarity.
  - Add focus styles for accessibility and better user experience.

**Code Example**:

```css
.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 15px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.contact-form input:focus,
.contact-form textarea:focus {
  border-color: #333;
  outline: none;
}
```

---

### **3. Accessibility Features**

Explain how to implement ARIA attributes and focus styles:

- **Key Concepts**:
  - `aria-required="true"` ensures screen readers communicate required fields.
  - Focus styles provide visual feedback for users navigating with a keyboard.

**Code Example**:

```css
.submit-button {
  padding: 10px 20px;
  background-color: #333;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.submit-button:hover {
  background-color: #555;
}
```

---

## **Common Mistakes to Address**

1. **Missing Labels**:
   - Emphasize the importance of `<label>` for accessibility and usability.
2. **Inconsistent Form Styles**:
   - Guide students in maintaining uniform padding, borders, and colors.
3. **Neglecting Focus Styles**:
   - Stress the importance of `:focus` for accessible navigation.

---

## **Learning Outcomes**

By the end of the lesson, students should:

1. Create a semantic HTML structure for a personal portfolio.
2. Style the page using advanced CSS selectors.
3. Build accessible forms with proper labels, ARIA attributes, and focus styles.
4. Understand the importance of accessibility in web design.

---

## **Additional Resources**

- **HTML Accessibility**: [W3C Accessibility Guidelines](https://www.w3.org/WAI/)
- **CSS Forms**: [CSS Tricks - Forms](https://css-tricks.com/snippets/css/form-inputs/)
- **ARIA Practices**: [W3C ARIA Practices](https://www.w3.org/TR/wai-aria-practices/)

---
