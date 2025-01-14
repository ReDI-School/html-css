# **Milestone 3: CSS Layout – Project Guide**

## **Overview**

This guide explains the enhancements made to the e-commerce store in Milestone 3. The focus is on CSS layout strategies, introducing Flexbox, Grid, classes, IDs, and responsive design. The project emphasizes structuring a professional and mobile-friendly website.

---

## **Core Concepts Demonstrated**

1. **Classes and IDs**

   - **Classes**: Applied to groups of elements for reusable styling (e.g., `.product-card`, `.nav-link`).
   - **IDs**: Used for unique elements (e.g., `#product-1`, `#product-2`).

2. **Flexbox**

   - Used for the navigation bar (`.navbar`):
     - Aligns links horizontally on larger screens.
     - Adjusts to vertical alignment on smaller screens.

3. **CSS Grid**

   - Used for the product listing section (`.product-grid`):
     - Automatically adapts the number of columns based on screen size.
     - Implements a flexible and responsive layout.

4. **Responsive Design**

   - **Media Queries**:
     - Adjust styles for screens smaller than 768px.
     - Ensure mobile-friendly navigation and product display.

5. **Hover Effects**
   - Enhance interactivity for buttons and links.

---

## **File Breakdown**

### **1. `index.html`**

The structure remains similar to Weeks 1 and 2 but now includes **classes** and **IDs**.

#### **Key Updates**

- **Classes**: Added for consistent and reusable styling (e.g., `.product-card`, `.navbar`).
- **IDs**: Assigned to specific elements for unique styling or identification.

**Code Snippet:**

```html
<article class="product-card" id="product-1">
  <h2 class="product-title">Product 1</h2>
  <img src="product1.jpg" alt="Image of Product 1" class="product-image" />
  <p class="product-description">A short description of Product 1.</p>
  <a href="#" class="product-button">Add to Cart</a>
</article>
```

---

### **2. `style.css`**

The CSS file introduces advanced layout techniques using **Flexbox**, **CSS Grid**, and **media queries**.

#### **Header and Navigation Bar**

- Flexbox is used to align the logo and navigation links.
- Media queries adjust the navigation bar to a vertical layout on smaller screens.

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

.navbar {
  display: flex;
  gap: 15px;
}

@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }
}
```

#### **Product Grid Layout**

- CSS Grid is used for the product listing section.
- The layout dynamically adjusts the number of columns based on screen size.

**Code Snippet:**

```css
.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}
```

#### **Hover Effects**

- Buttons and links have hover states to improve interactivity.

**Code Snippet:**

```css
.product-button:hover {
  background-color: #555;
}
.nav-link:hover {
  text-decoration: underline;
}
```

---

## **Discussion Points**

1. **Classes vs IDs**: Why are classes preferred for reusable styles, while IDs are used for unique elements?
2. **Flexbox vs Grid**: When should Flexbox be used (e.g., navigation bars) versus Grid (e.g., multi-column layouts)?
3. **Responsive Design**: How do media queries improve usability on smaller screens?
4. **User Experience**: How do hover effects make the interface more engaging?

---

## **Expected Output**

- A fully styled and responsive e-commerce store:
  - Navigation adjusts for mobile devices.
  - Product grid layout adapts to screen sizes.
  - Interactive links and buttons.
- Enhanced structure using classes and IDs.

---
