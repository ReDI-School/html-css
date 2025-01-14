
# **Milestone 2: CSS Basics – Project Guide**

## **Overview**
This guide explains the updated e-commerce project from Milestone 2, focusing on fundamental CSS concepts. The enhancements include styling the HTML skeleton created in Milestone 1 by applying colors, fonts, spacing, and responsive design using the box model.

---

## **Core Concepts Demonstrated**

1. **CSS Selectors**
   - Element selectors (e.g., `header`, `footer`).
   - Class selectors for flexible styling.
   - Pseudo-classes like `:hover` for interactive elements.

2. **Box Model**
   - Visualizing and managing space around elements using padding, margin, and borders.
   - Applying `box-sizing: border-box` for predictable element sizing.

3. **Styling Fundamentals**
   - Adding background colors and fonts for a cohesive theme.
   - Button styling to improve user interaction.

4. **Responsive Design**
   - Using CSS Grid to make the product listing section responsive.
   - Implementing `grid-template-columns` with `auto-fit` and `minmax` for flexible layouts.

---

## **File Breakdown**

### **1. `index.html`**
The structure remains largely unchanged from Milestone 1. However, we link the updated `style.css` file and prepare it for new styles.

#### **Key Updates**
- Addition of the `style.css` link in the `<head>` section.
- Organized content to ensure styling is applied effectively.

**Code Snippet:**
```html
<link rel="stylesheet" href="style.css">
```

---

### **2. `style.css`**
The primary focus of this week’s project is the `style.css` file, which introduces basic styling concepts.

#### **Header Styling**
- **Purpose**: Enhance branding and navigation.
- **Key Features**:
  - Background color for contrast.
  - Flexbox for alignment.
  - Styling for navigation links.

**Code Snippet:**
```css
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
    background-color: #333;
    color: white;
}
header nav a {
    color: white;
    text-decoration: none;
    margin-left: 15px;
}
```

#### **Main Content Styling**
- **Purpose**: Improve readability and layout for product listings.
- **Key Features**:
  - CSS Grid for a responsive layout.
  - Padding and borders to define product boundaries.
  - Background color for a light, neutral look.

**Code Snippet:**
```css
main section {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
}
main article {
    border: 1px solid #ddd;
    padding: 15px;
    text-align: center;
    background-color: #f9f9f9;
    border-radius: 5px;
}
```

#### **Footer Styling**
- **Purpose**: Create a cohesive footer design.
- **Key Features**:
  - Background color matching the header.
  - Text alignment for simplicity.

**Code Snippet:**
```css
footer {
    text-align: center;
    padding: 10px;
    background-color: #333;
    color: white;
    margin-top: 20px;
}
```

#### **Interactive Elements**
- **Purpose**: Add interaction to buttons and links.
- **Key Features**:
  - Button-like styling for links.
  - Hover effects to improve user experience.

**Code Snippet:**
```css
main article a {
    display: inline-block;
    margin-top: 10px;
    padding: 5px 10px;
    background-color: #333;
    color: white;
    text-decoration: none;
    border-radius: 3px;
}
main article a:hover {
    background-color: #555;
}
```

---

## **Discussion Points**

1. **Selectors**: How do different types of selectors (e.g., element, class) allow for flexible and modular styling?  
2. **Box Model**: Why is `box-sizing: border-box` recommended for consistent layout design?  
3. **Responsive Design**: How does the `auto-fit` and `minmax` approach in CSS Grid adapt to various screen sizes?  
4. **User Experience**: How do hover effects improve interactivity?  

---

## **Expected Output**
By the end of this Milestone:
- The e-commerce website has a styled header, footer, and product listing section.  
- Responsive product layout adjusts to different screen sizes.  
- Buttons and links are visually distinct and interactive.  

---

## **Next Steps**
- Milestone 3 will introduce advanced layout techniques, including Flexbox and advanced responsive design.
