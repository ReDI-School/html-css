# **Milestone 3: Responsive Design – Completing the Personal Portfolio (Part 3/3)**

## **Objective**

- Make the personal portfolio fully **responsive**, ensuring it looks great on all devices.
- Focus on **mobile-first design** principles.
- Use **media queries** to adjust layouts for different screen sizes.
- Implement a grid layout for the "Projects" section to improve usability.

---

## **Project Overview**

This project completes the personal portfolio by making it responsive. The design adapts seamlessly to various screen sizes, ensuring a mobile-friendly experience. The "Projects" section uses a CSS Grid layout that adjusts based on the screen width.

---

## 🗂️ Folder Structure

```plaintext
03_milestone/
│
├── index.html           # Main HTML file for the milestone
├── style.css            # CSS file for styling the HTML
└── README.md            # Milestone documentation
```

---

## **Project Code**

### **1. Updated `index.html`**

The structure remains consistent with Milestone 2, focusing on the responsiveness of existing elements.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Personal Portfolio</title>
    <link rel="stylesheet" href="style.css" />
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
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed euismod,
          sapien in vehicula tincidunt, est justo tempus nulla, non dictum ex
          magna nec mauris.
        </p>
      </section>

      <!-- Projects Section -->
      <section id="projects" class="projects-section">
        <h2>My Work</h2>
        <div class="projects-grid">
          <div class="project-card">
            <h3>Project 1</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
          </div>
          <div class="project-card">
            <h3>Project 2</h3>
            <p>
              Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
          </div>
          <div class="project-card">
            <h3>Project 3</h3>
            <p>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco
              laboris.
            </p>
          </div>
          <div class="project-card">
            <h3>Project 4</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
          </div>
        </div>
      </section>

      <!-- Contact Form Section -->
      <section id="contact" class="contact-section">
        <h2>Contact Me</h2>
        <form action="#" method="POST" class="contact-form">
          <label for="name">Name:</label>
          <input
            type="text"
            id="name"
            name="name"
            required
            aria-required="true"
          />

          <label for="email">Email:</label>
          <input
            type="email"
            id="email"
            name="email"
            required
            aria-required="true"
          />

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

The CSS file is updated to include responsive design using media queries and a grid layout for the "Projects" section.

```css
/* General Styles */
body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background: linear-gradient(to bottom, #f4f4f4, #ffffff);
}

/* Header Styling */
.site-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #333;
  color: white;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.navbar .nav-link {
  color: white;
  text-decoration: none;
  margin-left: 20px;
}

/* About Section */
.about-section {
  padding: 20px;
  background-color: #f8f8f8;
  text-align: center;
}

/* Projects Section */
.projects-section {
  padding: 20px;
  background-color: #fff;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

.project-card {
  border: 1px solid #ccc;
  border-radius: 10px;
  padding: 15px;
  background-color: #f9f9f9;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
  transform: scale(1.05);
  box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.2);
}

/* Contact Form */
.contact-section {
  padding: 20px;
  background-color: #f4f4f4;
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

/* Media Queries */
@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }

  .projects-grid {
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  }

  .project-card {
    padding: 10px;
  }
}

@media (max-width: 480px) {
  .site-header {
    flex-direction: column;
    align-items: flex-start;
  }

  .nav-link {
    margin: 10px 0;
  }
}
```

---

## **Core Concepts Demonstrated**

1. **CSS Grid Layout**:

   - Flexible grid system for the "Projects" section.
   - `repeat(auto-fit, minmax())` for responsive columns.

2. **Media Queries**:

   - Adjusting layouts for screens smaller than 768px and 480px.
   - Ensuring navigation, project cards, and forms are mobile-friendly.

3. **Mobile-First Design**:
   - Designing styles for smaller screens first and enhancing for larger screens.

---

## **Resources**

1. **Responsive Design**: [MDN Web Docs - Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)
2. **CSS Grid**: [CSS Tricks - Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
3. **Media Queries**: [MDN Web Docs - Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)

---

## **Expected Output**

- A fully responsive portfolio that adapts to all screen sizes.
- Clean, mobile-friendly navigation and layouts.
- A well-structured and visually appealing project section.

---
