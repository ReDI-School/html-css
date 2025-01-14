# **BONUS MILESTONE: Personal Portfolio Website**

## **Overview**

This project focuses on building a fully responsive and accessible personal portfolio website. Across Milestone 1, 2 and 3, students learn to implement semantic HTML, advanced CSS techniques, and responsive design to create an interactive and visually appealing portfolio.

This fourth milestone is a bonus milestone. That means you don't need to complete it to hand in the project. If you completed milestone 1-3, then we recommend you to work on the BONUS milestone. If you haven't completed milestone 1-3, then finish them first. 


---

## 🗂️ Folder Structure

```plaintext
04_milestone/
│
├── index.html           # Main HTML file for the milestone
├── style.css            # CSS file for styling the HTML
└── README.md            # Milestone documentation
```


---

## **Key Features**

1. **Accessibility**:

   - Semantic structure with `<header>`, `<section>`, and `<footer>` elements.
   - ARIA attributes to improve form usability.

2. **Interactivity**:

   - Animations and transitions to enhance visual appeal.
   - Hover effects for buttons and links.

3. **Responsive Design**:
   - CSS Grid and Flexbox for adaptable layouts.
   - Media queries to ensure mobile-first design.

---

## **Project Requirements**

1. **HTML Structure**:

   - A header with navigation links.
   - Sections for "About," "Projects," and "Contact."
   - A functional contact form with labeled input fields.

2. **CSS Styling**:

   - Consistent styling for text, buttons, and layout.
   - Responsive grid for the "Projects" section.
   - Animations for headers and hover effects for interactive elements.

3. **Responsive Layout**:
   - Ensure the website adapts to screen sizes smaller than 768px.
   - Use media queries to adjust navigation and grid layouts.

---

## **Expected Outcome**

By completing this project, students will have a fully functional and visually engaging portfolio website that demonstrates their skills in HTML, CSS, and responsive web design.

---

## **Steps to Complete the Project**

### **1. Build the HTML Skeleton**

- Use semantic tags to create the structure for:
  - Header with logo and navigation.
  - About section with a brief introduction.
  - Projects section with a responsive grid layout.
  - Contact form with input fields for name, email, and message.

**Code Example:**

```html
<header>
  <h1>My Portfolio</h1>
  <nav>
    <a href="#about">About</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>
</header>
```

---

### **2. Apply Basic CSS Styling**

- Style the header, about section, projects, and contact form using:
  - Colors and fonts for a cohesive theme.
  - Padding and margins for spacing.

**Code Example:**

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

---

### **3. Add Interactivity with CSS Animations**

- Implement keyframe animations for headers and transitions for buttons.

**Code Example:**

```css
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
h2 {
  animation: fadeIn 1s ease-in-out;
}
```

---

### **4. Make the Website Responsive**

- Use CSS Grid for the projects section with `repeat(auto-fit, minmax())`.
- Add media queries to adjust layouts for smaller screens.

**Code Example:**

```css
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

@media (max-width: 768px) {
  .project-grid {
    grid-template-columns: 1fr;
  }
}
```

---

## **Submission Guidelines**

Students must submit:

1. `index.html` file with a semantic structure.
2. `style.css` file with animations, transitions, and responsive design.
3. A live demo or screenshots of the final portfolio.

---

## **Evaluation Criteria**

1. **HTML Semantics** (25%):

   - Proper use of semantic tags and structure.

2. **CSS Styling** (25%):

   - Cohesive and visually appealing design.

3. **Interactivity** (25%):

   - Effective use of animations and hover effects.

4. **Responsive Design** (25%):
   - Website adapts seamlessly to various screen sizes.

---

## **Resources**

1. **HTML Basics**: [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
2. **CSS Animations**: [MDN Web Docs - CSS Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)
3. **CSS Grid**: [CSS Tricks - Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
4. **Responsive Design**: [CSS Tricks - Responsive Design](https://css-tricks.com/snippets/css/a-guide-to-responsive-design/)

---
