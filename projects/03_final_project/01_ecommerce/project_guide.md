# **Project 1: Responsive Design – TechStore Project Guide**

## **Overview**

This guide explains the implementation of a responsive online electronics marketplace called "TechStore." The project demonstrates the use of **modern CSS techniques** like grid layout, custom properties, and responsive design principles, ensuring the site adapts seamlessly to all devices.

---

## **Core Concepts Demonstrated**

1. **Responsive Design**

   - Ensures the layout adjusts for screens of various sizes, including desktops, tablets, and mobile devices.
   - Includes media queries to provide specific styles for devices under 1024px.

2. **CSS Grid and Flexbox**

   - A responsive product grid is created using `grid-template-columns` with `auto-fill` and `minmax()` for automatic column resizing.
   - Flexbox is utilized for the header and navigation elements.

3. **Custom Properties (CSS Variables)**

   - Simplifies theming with reusable variables for colors, background, and text styles.

4. **Interactive Elements**
   - Buttons and product cards with hover effects to enhance user interaction.
   - Actions for adding items to the cart and wishlist.

---

## **File Breakdown**

### **1. `index.html`**

The HTML structure follows semantic principles and includes key elements like a header, sidebar, and product grid.

**Key Features**

- **Header:** Includes a logo, a search bar, and navigation links.
- **Sidebar:** Displays a category menu for product browsing.
- **Main Section:** Features a responsive grid layout of product cards.

**Code Snippet:**

```html
<header class="header">
  <div class="header-content">
    <a href="#" class="logo">🛒 TechStore</a>
    <div class="search-container">
      <input type="text" placeholder="Search products, categories..." />
      <button>Search</button>
    </div>
    <nav class="nav-links">
      <a href="#">👤 Account</a>
      <a href="#">🛒 Cart (0)</a>
      <a href="#">❤️ Wishlist</a>
    </nav>
  </div>
</header>
```

---

### **2. `style.css`**

The CSS file employs custom properties for maintainability and includes comprehensive styling for all components.

#### **Header Styling**

- Sticky position ensures the header remains visible during scrolling.
- Search bar and navigation links are flexibly arranged.

**Code Snippet:**

```css
.header {
  background-color: var(--primary-color);
  color: white;
  padding: 15px 0;
  position: sticky;
  top: 0;
  z-index: 100;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}
```

#### **Sidebar and Category List**

- Categories are listed as clickable links with hover effects.

**Code Snippet:**

```css
.sidebar {
  width: 250px;
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  padding: 20px;
}

.category-list li a {
  text-decoration: none;
  color: var(--text-color);
  display: block;
  padding: 10px;
  border-radius: 4px;
  transition: background-color 0.3s;
}

.category-list li a:hover {
  background-color: #f0f0f0;
}
```

#### **Product Grid Layout**

- Utilizes CSS Grid for flexible column arrangement.
- Includes hover effects for product cards.

**Code Snippet:**

```css
.products-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 20px;
}

.product-card {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  padding: 20px;
  text-align: center;
  transition: transform 0.3s, box-shadow 0.3s;
}

.product-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
}
```

#### **Responsive Design**

- Media queries adjust the layout for smaller screens.

**Code Snippet:**

```css
@media (max-width: 1024px) {
  .main-container {
    flex-direction: column;
  }

  .sidebar {
    width: 100%;
  }

  .header-content {
    flex-direction: column;
    gap: 15px;
  }

  .search-container {
    width: 100%;
    margin: 10px 0;
  }
}
```

---

## **Core Concepts Explained**

1. **Responsive Design**

   - How media queries ensure adaptability across devices.
   - Importance of accessibility and usability.

2. **Grid and Flexbox**

   - Use of CSS Grid for complex layouts.
   - Flexbox for header and navigation flexibility.

3. **Custom Properties**
   - Streamlining the design with CSS variables.

---

## **Expected Outcome**

- A visually appealing and functional online store.
- A responsive design adapting to all screen sizes.
- Engaging user interactions with buttons and product cards.

---
