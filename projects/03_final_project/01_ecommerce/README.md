# **Project 1: TechStore Responsive Design Project**

## **Objective**

- Build a fully responsive e-commerce web application.
- Ensure adaptability for devices of all screen sizes.
- Implement interactive and accessible UI elements.

---

## **Core Features**

### **1. Header Section**

- Sticky header with logo, search bar, and navigation links.
- Includes a fully responsive search bar.

### **2. Sidebar**

- Lists product categories with hover effects.
- Adjusts to fit the screen width in smaller devices.

### **3. Product Grid**

- Displays product cards using CSS Grid layout.
- Responsive design with dynamic columns based on screen size.

### **4. Responsive Design**

- Implemented using media queries for tablets and mobile devices.

---

## 🗂️ Folder Structure

```plaintext
01_ecommerce/
│
├── index.html           # Main HTML file
├── style.css            # CSS file for styling the HTML
└── README.md            # Documentation
```

---

## **Key Code Components**

### **HTML**

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

<section class="products-grid">
  <div class="product-card">
    <img
      src="https://dummyimage.com/600x400/000/fff&text=Smartphone"
      alt="Smartphone"
    />
    <h4>Advanced Pro Smartphone</h4>
    <p class="product-price">$599.99</p>
    <div class="product-actions">
      <button class="btn-cart">Add to Cart</button>
      <button class="btn-wishlist">♡ Wishlist</button>
    </div>
  </div>
</section>
```

### **CSS**

#### Header

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
```

#### Product Grid

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

#### Responsive Design

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
}
```

---

## **Expected Outcome**

- A functional, responsive e-commerce layout.
- Interactive elements with hover effects and responsive adjustments.

---
