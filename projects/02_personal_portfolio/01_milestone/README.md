
# **Milestone 5: HTML & CSS – Building a Personal Portfolio (Part 1/3)**

## **Objective**
- Create a personal portfolio website with a focus on **semantic structure**, **forms**, and **accessibility**.
- Learn advanced CSS selectors for styling specific elements.
- Implement a contact form with accessible features.

---

## **Project Overview**
This project marks the beginning of a personal portfolio website. It includes a landing page with an introduction and a contact form. The page will be styled using semantic HTML and CSS with accessibility considerations.

---

## 🗂️ Folder Structure

```plaintext
01_milestone/
│
├── index.html           # Main HTML file for the milestone
├── style.css            # CSS file for styling the HTML
└── README.md            # Milestone documentation
```

---

## **Project Code**

### **1. `index.html`**
This HTML file contains a clean and semantic structure with a header, a main section introducing the portfolio, and a contact form.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header Section -->
    <header class="site-header">
        <h1 class="site-title">My Portfolio</h1>
        <nav class="navbar">
            <a href="#about" class="nav-link">About</a>
            <a href="#contact" class="nav-link">Contact</a>
        </nav>
    </header>

    <!-- Main Content -->
    <main>
        <!-- About Section -->
        <section id="about" class="about-section">
            <h2>Welcome to My Portfolio</h2>
            <p>Hello! I’m a web developer passionate about building accessible and user-friendly websites.</p>
        </section>

        <!-- Contact Form Section -->
        <section id="contact" class="contact-section">
            <h2>Contact Me</h2>
            <form action="#" method="POST" class="contact-form">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required aria-required="true">

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required aria-required="true">

                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="5" required aria-required="true"></textarea>

                <button type="submit" class="submit-button">Send Message</button>
            </form>
        </section>
    </main>

    <!-- Footer -->
    <footer class="site-footer">
        <p>&copy; 2025 My Portfolio. All rights reserved.</p>
    </footer>
</body>
</html>
```

---

### **2. `style.css`**
The CSS file focuses on accessibility and form styling, utilizing advanced selectors.

```css
/* General Styles */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

h1, h2 {
    margin-bottom: 15px;
}

/* Header Styling */
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

/* About Section */
.about-section {
    padding: 20px;
    background-color: #f4f4f4;
    text-align: center;
}

/* Contact Form */
.contact-section {
    padding: 20px;
    background-color: #fff;
}

.contact-form label {
    display: block;
    margin: 10px 0 5px;
    font-weight: bold;
}

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

/* Footer */
.site-footer {
    text-align: center;
    padding: 10px;
    background-color: #333;
    color: white;
    margin-top: 20px;
}
```

---

## **Core Concepts Demonstrated**
1. **Semantic HTML**:
   - Header, main, and footer for structure.
   - Labels and inputs for form fields with `aria-required` for accessibility.

2. **Accessibility**:
   - `aria-required="true"` to assist screen readers.
   - Focus states to improve user experience.

3. **Advanced CSS Selectors**:
   - Use of `:hover` and `:focus` pseudo-classes for interaction.
   - Block-level form labels and styled inputs.

4. **Forms**:
   - Input validation (`required` attribute).
   - Consistent styling for form elements.

---

## **Resources**
1. **HTML Forms**: [MDN Web Docs - Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)  
2. **Accessibility Guide**: [Web Accessibility Initiative (WAI)](https://www.w3.org/WAI/)  
3. **CSS Selectors**: [CSS Tricks - Selectors](https://css-tricks.com/how-css-selectors-work/)  
4. **ARIA Roles**: [W3C ARIA Specification](https://www.w3.org/TR/wai-aria/)  

---

## **Expected Output**
- A personal portfolio landing page with:
  - An introduction section.
  - A functional and accessible contact form.
- Well-structured and clean HTML.
- A styled and user-friendly form with focus and hover effects.

---

## **Next Steps**
- Milestone 6 will focus on **animations, transitions**, and advanced CSS techniques to enhance the portfolio design.
