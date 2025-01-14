
# **Milestone 6: CSS Advanced – Enhancing the Personal Portfolio (Part 2/3)**

## **Objective**
- Enhance the personal portfolio website by introducing **animations**, **transitions**, and advanced **pseudo-classes**.
- Add visual appeal and interactivity while maintaining accessibility.
- Style specific elements with advanced CSS selectors.

---

## **Project Overview**
This project builds on the Milestone 5 portfolio by adding animations and transitions to elements like navigation links, buttons, and the contact form. Advanced CSS selectors and pseudo-classes are used to refine the design.

---

## **Project Code**

### **1. Updated `index.html`**
The structure remains similar to Milestone 5 but is filled with additional placeholder text to improve the layout's appearance.

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
            <a href="#projects" class="nav-link">Projects</a>
            <a href="#contact" class="nav-link">Contact</a>
        </nav>
    </header>

    <!-- Main Content -->
    <main>
        <!-- About Section -->
        <section id="about" class="about-section">
            <h2>Welcome to My Portfolio</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed euismod, sapien in vehicula tincidunt, est justo tempus nulla, non dictum ex magna nec mauris.</p>
        </section>

        <!-- Projects Section -->
        <section id="projects" class="projects-section">
            <h2>My Work</h2>
            <div class="project-card">
                <h3>Project 1</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            </div>
            <div class="project-card">
                <h3>Project 2</h3>
                <p>Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
            </div>
            <div class="project-card">
                <h3>Project 3</h3>
                <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris.</p>
            </div>
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

### **2. Updated `style.css`**
The CSS file introduces animations, transitions, and advanced styling techniques.

```css
/* General Styles */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background: linear-gradient(to bottom, #f4f4f4, #ffffff);
    animation: fadeIn 1s ease-in-out;
}

/* Keyframe Animations */
@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}

h1, h2 {
    margin-bottom: 15px;
    text-align: center;
    animation: slideIn 1s ease-in-out;
}

@keyframes slideIn {
    from {
        transform: translateY(-20px);
        opacity: 0;
    }
    to {
        transform: translateY(0);
        opacity: 1;
    }
}

/* Header Styling */
.site-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
    background-color: #333;
    color: white;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.navbar .nav-link {
    color: white;
    text-decoration: none;
    margin-left: 20px;
    transition: color 0.3s ease;
}

.navbar .nav-link:hover {
    color: #ffa500;
    text-decoration: underline;
}

/* Projects Section */
.projects-section {
    padding: 20px;
    background-color: #f8f8f8;
    display: flex;
    justify-content: space-around;
    gap: 20px;
}

.project-card {
    width: 30%;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 10px;
    background-color: white;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
    transform: scale(1.05);
    box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.2);
}

/* Contact Form */
.contact-section {
    padding: 20px;
    background-color: #fff;
    animation: fadeIn 1.5s ease-in-out;
}

.contact-form input,
.contact-form textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
    border: 1px solid #ccc;
    border-radius: 5px;
    transition: border-color 0.3s ease;
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
    transition: background-color 0.3s ease;
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
1. **Animations and Keyframes**:
   - `@keyframes` for element entrance effects like `fadeIn` and `slideIn`.

2. **Transitions**:
   - Smooth transitions for hover effects on links and project cards.

3. **Advanced Selectors**:
   - Styling interactive elements with `:hover` and `:focus` pseudo-classes.

4. **Enhancing Visual Appeal**:
   - Adding gradients and box shadows for a modern, polished design.

---

## **Resources**
1. **CSS Animations**: [MDN Web Docs - Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)  
2. **CSS Transitions**: [CSS Tricks - Transitions](https://css-tricks.com/almanac/properties/t/transition/)  
3. **CSS Pseudo-Classes**: [MDN Web Docs - Pseudo-classes](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)  
4. **CSS Gradients**: [CSS Gradient Generator](https://cssgradient.io/)  

---

## **Expected Output**
- A visually appealing and interactive portfolio website with:
  - Smooth animations for page content.
  - Hover effects on links and project cards.
  - A polished layout with transitions and gradients.

---

## **Next Steps**
- Milestone 7 will focus on responsive design, ensuring the portfolio looks great on all screen sizes.
