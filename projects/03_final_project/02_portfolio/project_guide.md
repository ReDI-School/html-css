# **Project 2: Portfolio**

## **Overview**

This project demonstrates the implementation of a personal portfolio website for a creative developer. The website includes responsive design, engaging animations, and a modern layout to showcase projects, skills, and contact information.

---

## **Core Features**

### **1. Navigation Bar**

- Fixed at the top of the page with smooth scrolling to sections.
- Includes links to Home, Projects, Skills, and Contact sections.
- Hover animations for a modern touch.

### **2. Hero Section**

- A full-screen hero section introducing the developer's role.
- Includes a call-to-action for viewing projects and contacting the developer.

### **3. Projects Section**

- Displays a grid of project cards with hover effects.
- Each card includes a project image, title, and brief description.

---

## **Key Code Components**

### **HTML**

```html
<nav class="navbar">
  <div class="navbar-container">
    <a href="#" class="logo">Name Surname</a>
    <div class="nav-links">
      <a href="#home">Home</a>
      <a href="#projects">Projects</a>
      <a href="#skills">Skills</a>
      <a href="#contact">Contact</a>
    </div>
  </div>
</nav>

<section id="home" class="hero">
  <div class="hero-content">
    <h1>Creative Developer</h1>
    <p>
      Transforming ideas into beautiful, functional digital experiences with
      innovative design and cutting-edge technology.
    </p>
    <div class="cta-buttons">
      <a href="#projects" class="btn btn-primary">View My Work</a>
      <a href="#contact" class="btn btn-secondary">Get in Touch</a>
    </div>
  </div>
</section>
```

### **CSS**

#### Global Styles

```css
:root {
  --primary-color: #2c3e50;
  --accent-color: #3498db;
  --text-color: #333;
  --background-color: #f4f4f4;
  --transition-speed: 0.3s;
}

body {
  font-family: "Inter", sans-serif;
  color: var(--text-color);
  background-color: var(--background-color);
  line-height: 1.6;
}
```

#### Navigation Bar

```css
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background: rgba(255, 255, 255, 0.9);
  backdrop-filter: blur(15px);
  box-shadow: 0 2px 15px rgba(0, 0, 0, 0.05);
  z-index: 1000;
  padding: 20px 0;
}

.nav-links a:hover {
  color: var(--accent-color);
}
```

#### Hero Section

```css
.hero {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  background: linear-gradient(
    135deg,
    rgba(52, 152, 219, 0.05),
    rgba(44, 62, 80, 0.05)
  );
}

.hero h1 {
  font-size: 4.5rem;
  color: var(--primary-color);
}
```

#### Projects Section

```css
.projects {
  background-color: white;
  padding: 100px 0;
}

.projects-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
}
```

---

## **Expected Outcome**

- A visually appealing, fully responsive portfolio website.
- Smooth scrolling, hover animations, and engaging project cards.

---
