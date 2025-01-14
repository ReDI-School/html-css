# **Milestone 7: Responsive Design – Project Guide**

## **Overview**

This guide provides an explanation of the Milestone 7 project, which focuses on completing the personal portfolio website with responsive design. The design adapts seamlessly to various screen sizes, ensuring a mobile-friendly and visually appealing experience. The "Projects" section is structured using CSS Grid, and media queries are implemented for layout adjustments.

---

## **Core Concepts Demonstrated**

1. **CSS Grid Layout**

   - Use of `repeat(auto-fit, minmax())` for responsive columns in the "Projects" section.
   - Adjusting grid templates for different screen sizes.

2. **Media Queries**

   - Adapting layouts for devices smaller than 768px and 480px.
   - Ensuring navigation, project cards, and forms are mobile-friendly.

3. **Mobile-First Design**

   - Designing styles for smaller screens first and progressively enhancing for larger screens.

4. **Responsive Navigation**
   - Adjusting the header and navigation bar for smaller devices using `flex-direction`.

---

## **File Breakdown**

### **1. `index.html`**

The structure remains consistent with Milestone 6 but includes additional project cards for demonstrating grid responsiveness.

#### **Key Features**

- Projects are displayed using a grid layout with semantic `<div>` containers.
- The navigation and contact form retain accessibility features.

**Code Snippet:**

```html
<div class="projects-grid">
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
  <div class="project-card">
    <h3>Project 4</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  </div>
</div>
```

---

### **2. `style.css`**

The CSS file is updated with media queries and grid properties for responsiveness.

#### **Projects Section**

- The "Projects" section uses a grid layout that adjusts automatically based on screen width.

**Code Snippet:**

```css
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
```

#### **Media Queries**

- Media queries adjust the layout for screens smaller than 768px and 480px.

**Code Snippet:**

```css
@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }

  .projects-grid {
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
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

#### **Contact Form**

- The form inputs and buttons are styled to fit smaller screens.

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

---

## **Discussion Points**

1. **CSS Grid**

   - How does `repeat(auto-fit, minmax())` create a responsive grid layout?
   - Why is CSS Grid a preferred choice for multi-column layouts?

2. **Media Queries**

   - How do media queries ensure a consistent design across different devices?
   - What are the advantages of mobile-first design?

3. **Responsive Navigation**

   - How does adjusting `flex-direction` improve the usability of navigation on smaller screens?

4. **Responsive Design**
   - Discuss the importance of responsive design for accessibility and usability.

---

## **Resources**

1. **Responsive Design**: [MDN Web Docs - Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)
2. **CSS Grid**: [CSS Tricks - Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
3. **Media Queries**: [MDN Web Docs - Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)

---

## **Expected Output**

- A fully responsive portfolio that adapts seamlessly to all screen sizes.
- A mobile-friendly navigation bar.
- A clean, grid-based layout for the projects section.

---
