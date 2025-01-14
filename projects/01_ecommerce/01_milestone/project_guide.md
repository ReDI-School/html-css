
# **Milestone 1: HTML Project Guide – E-Commerce Skeleton**

## **Overview**
This guide outlines the structure and key concepts demonstrated in the Milestone 1 project: building the skeleton of an e-commerce store. It focuses on semantic HTML and the creation of a clean, well-organized document.

---

## **Core Concepts Demonstrated**

1. **HTML Boilerplate**
   - Basic structure of an HTML5 document.
   - Key tags: `<!DOCTYPE html>`, `<html>`, `<head>`, `<meta>`, `<title>`, and `<body>`.

2. **Semantic Elements**
   - The importance of semantic tags for accessibility and SEO.
   - Tags used:
     - `<header>`: Contains the site logo and navigation links.
     - `<main>`: Main content area for product listings.
     - `<section>`: Groups products logically.
     - `<article>`: Individual product containers.
     - `<footer>`: Contact information and footer content.

3. **Placeholder Content**
   - Use of placeholder content for images, text, and links.
   - Images: Placeholder images (`product1.jpg`, etc.) simulate product visuals.
   - Links: Dummy links (`#`) for navigation and buttons.

4. **Code Structure**
   - Logical and clean organization of elements.
   - Use of indentation to enhance readability.

---

## **File Breakdown**

### **1. `index.html`**

#### **Header**
- Purpose: Site navigation and branding.
- Key Elements:
   - `<img>`: Placeholder for a company logo.
   - `<nav>`: Navigation links.

**Code:**
```html
<header>
    <img src="logo.png" alt="E-Commerce Logo" width="100">
    <nav>
        <a href="#">Home</a>
        <a href="#">Products</a>
        <a href="#">Contact</a>
    </nav>
</header>
```

#### **Main Content**
- Purpose: Display product listings.
- Organized into:
   - `<section>`: Groups the content.
   - `<article>`: Represents an individual product.

**Code:**
```html
<main>
    <section>
        <article>
            <h2>Product 1</h2>
            <img src="product1.jpg" alt="Image of Product 1" width="150">
            <p>A short description of Product 1.</p>
            <a href="#">Add to Cart</a>
        </article>
        <article>
            <h2>Product 2</h2>
            <img src="product2.jpg" alt="Image of Product 2" width="150">
            <p>A short description of Product 2.</p>
            <a href="#">Add to Cart</a>
        </article>
    </section>
</main>
```

#### **Footer**
- Purpose: Contact information and copyright details.

**Code:**
```html
<footer>
    <p>Contact us: <a href="mailto:info@ecommerce.com">info@ecommerce.com</a></p>
    <p>&copy; 2025 E-Commerce Store</p>
</footer>
```

---

## **Why Semantic HTML Matters**
- **Accessibility**: Screen readers rely on semantic tags to convey content meaning.
- **SEO Benefits**: Search engines prioritize semantic structures to index content effectively.
- **Maintainability**: Logical HTML structure makes the code easier to read and maintain.

---

## **Explaining Key Elements**

| **Element**     | **Purpose**                                                                 | **Notes**                                       |
|------------------|-----------------------------------------------------------------------------|------------------------------------------------|
| `<!DOCTYPE>`    | Declares the document type and version (HTML5).                            | Ensures browser compatibility.                 |
| `<header>`      | Represents introductory content or navigation links.                       | Contains logo and site navigation.             |
| `<main>`        | The central content of the page, excluding repeated elements (header/footer). | Improves document structure.                   |
| `<section>`     | Groups related content.                                                    | Used to logically divide product listings.     |
| `<article>`     | Represents self-contained content (individual products).                   | Reusable and independent content.              |
| `<footer>`      | Defines footer content, such as contact details and copyright.             | Appears at the bottom of the page.             |
| `<img>`         | Displays images for visual content.                                        | Includes `alt` text for accessibility.         |
| `<a>`           | Anchor tags for links (navigation, buttons).                               | `href="#"` is used as a placeholder.           |

---

## **Discussion Points**
1. Why are semantic tags like `<header>`, `<main>`, and `<footer>` important for modern web development?
2. How does organizing content into sections and articles make the page more readable and maintainable?
3. What role does the `alt` attribute of `<img>` play in accessibility?

---

## **Next Steps**
- In Milestone 2, styles will be applied using CSS to enhance the visual appeal of the skeleton structure.
- Responsive design and layout techniques (e.g., Flexbox and Grid) will follow in Milestone 3.
