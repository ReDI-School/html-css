# **Milestone 5: HTML & CSS – Project Guide**

## **Overview**

This guide provides an explanation of the Milestone 5 project, which involves creating the foundation of a personal portfolio website. The focus is on building a semantic HTML structure with accessible forms and advanced CSS styling.

---

## **Core Concepts Demonstrated**

1. **Semantic HTML**

   - Use of meaningful HTML tags such as `<header>`, `<section>`, `<footer>`, and `<form>` to ensure clear document structure.
   - Proper labeling of form elements for accessibility.

2. **Accessibility**

   - Implementation of ARIA attributes (`aria-required="true"`) to improve the experience for users relying on assistive technologies.
   - Focus and hover styles for better usability.

3. **Advanced CSS Selectors**

   - Use of pseudo-classes such as `:hover` and `:focus` for interactivity.
   - Block-level styling of form labels and inputs.

4. **Forms**
   - Creation of a contact form with fields for name, email, and message.
   - Input validation using the `required` attribute.

---

## **File Breakdown**

### **1. `index.html`**

This file includes a semantic structure with sections for an introduction and a contact form.

#### **Key Features**

- Semantic `<header>` for the site title and navigation.
- `<section>` tags for logically grouping the "About" and "Contact" sections.
- A well-structured `<form>` with proper `<label>` and input fields.

**Code Snippet:**

```html
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
```

---

### **2. `style.css`**

This file focuses on styling the layout and form, ensuring an accessible and visually appealing design.

#### **Key Features**

- **Header and Navigation Bar**:
  - Flexbox used for alignment and spacing.
  - Hover effects for navigation links.

**Code Snippet:**

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

- **Contact Form**:
  - Styled inputs and buttons for consistency.
  - Focus styles to enhance usability.

**Code Snippet:**

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

- **Hover Effects**:
  - Buttons change background color on hover for better feedback.

**Code Snippet:**

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

## **Discussion Points**

1. **Semantic HTML**:

   - Why is it important to use tags like `<section>`, `<label>`, and `<form>`?
   - How do semantic tags improve accessibility and SEO?

2. **Accessibility**:

   - What role do ARIA attributes like `aria-required` play in enhancing accessibility?
   - How do focus styles contribute to usability?

3. **CSS Pseudo-Classes**:

   - How can pseudo-classes like `:hover` and `:focus` improve the user experience?

4. **Forms**:
   - Why is input validation using `required` important?

---

## **Resources**

1. **HTML Accessibility**: [W3C Accessibility Guidelines](https://www.w3.org/WAI/)
2. **ARIA Roles**: [ARIA Practices](https://www.w3.org/TR/wai-aria-practices/)
3. **CSS Selectors**: [MDN Web Docs - CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)
4. **Forms in HTML**: [MDN Web Docs - Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)

---

## **Expected Output**

- A functional landing page with:
  - A welcoming introduction.
  - A contact form that is accessible and user-friendly.
- A styled layout with responsive and interactive elements.

---
