# **Recap: Weeks 5, 6, and 7 – Project Guide**

## **Overview**

This guide summarizes the core concepts and project outputs from Weeks 5, 6, and 7. Over these weeks, students enhanced their personal portfolio project, focusing on accessibility, animations, and responsive design.

---

## **Core Concepts Demonstrated**

1. **HTML & Accessibility (Milestone 5)**:

   - Structuring a personal portfolio website with semantic HTML.
   - Implementing accessible forms using ARIA attributes and proper labeling.

2. **Advanced CSS (Milestone 6)**:

   - Adding animations and transitions for dynamic effects.
   - Using pseudo-classes like `:hover` and `:focus` to enhance interactivity.

3. **Responsive Design (Milestone 7)**:
   - Using CSS Grid and Flexbox for adaptable layouts.
   - Applying media queries for a mobile-first design approach.

---

## **File Breakdown**

### **1. `index.html`**

The HTML file provides the structure for the personal portfolio, including sections for the header, about, projects, and contact.

#### **Key Features**:

- Semantic structure for better readability and accessibility.
- Placeholder content for projects and a functional contact form.

**Code Snippet:**

```html
<header>
  <h1>My Portfolio</h1>
  <nav>
    <a href="#about">About</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<main>
  <section id="about">
    <h2>About Me</h2>
    <p>
      Welcome to my portfolio! I’m a web developer passionate about creating
      user-friendly websites.
    </p>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="project-grid">
      <div class="project-card">
        <h3>Project 1</h3>
        <p>Description of Project 1.</p>
      </div>
      <div class="project-card">
        <h3>Project 2</h3>
        <p>Description of Project 2.</p>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <form>
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required />

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required />

      <label for="message">Message:</label>
      <textarea id="message" name="message" rows="4"></textarea>

      <button type="submit">Send</button>
    </form>
  </section>
</main>

<footer>
  <p>&copy; 2025 My Portfolio</p>
</footer>
```

---

### **2. `style.css`**

This file evolves across the three weeks, integrating advanced CSS techniques like animations, transitions, and responsive design.

#### **Header and Navigation**

- **Purpose**: Create a sticky and responsive navigation bar.
- **Key Features**:
  - Flexbox for alignment.
  - Sticky positioning for better usability.

**Code Snippet:**

```css
header {
  position: sticky;
  top: 0;
  background-color: #333;
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
}
nav a {
  color: white;
  text-decoration: none;
  margin: 0 10px;
}
nav a:hover {
  text-decoration: underline;
}
```

#### **Project Section Styling**

- **Purpose**: Create a responsive grid for projects.
- **Key Features**:
  - CSS Grid for layout.
  - Hover effects for interactivity.

**Code Snippet:**

```css
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}
.project-card {
  border: 1px solid #ddd;
  border-radius: 5px;
  padding: 10px;
  text-align: center;
  transition: transform 0.3s;
}
.project-card:hover {
  transform: scale(1.05);
}
```

#### **Animations and Transitions**

- **Purpose**: Add dynamic effects to elements.
- **Key Features**:
  - Keyframes for fade-in and slide-in effects.
  - Smooth transitions for hover states.

**Code Snippet:**

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

#### **Responsive Design**

- **Purpose**: Ensure the layout adapts to all screen sizes.
- **Key Features**:
  - Media queries for small screens.
  - Adjustments to the navigation and grid layout.

**Code Snippet:**

```css
@media (max-width: 768px) {
  nav {
    flex-direction: column;
    align-items: flex-start;
  }
  .project-grid {
    grid-template-columns: 1fr;
  }
}
```

---

## **Discussion Points**

1. **Accessibility**: How do semantic HTML and ARIA attributes improve user experience?
2. **Animations**: How do keyframes and transitions enhance visual appeal?
3. **Responsive Design**: Why is mobile-first design critical in modern web development?
4. **User Experience**: How do hover effects and sticky navigation improve usability?

---
