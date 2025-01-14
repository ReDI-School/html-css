# **Milestone 1: HTML Fundamentals – Building the Skeleton of an E-Commerce Store**

## **Objective**

By the end of this milestone, you will:

1. Understand the basics of semantic HTML structure.
2. Build the skeleton of an e-commerce website with a header, footer, and product listings.
3. Use Git for version control and CLI for managing project files.

---

## **Project Overview**

We will create the foundational structure of an e-commerce website. The focus will be on writing semantic, well-organized HTML. Styling and layout will be added in later weeks.


--- 

## 🗂️ Folder Structure

```plaintext
01_milestone/
│
├── index.html           # Main HTML file for the milestone
├── logo.svg             # Logo image used in the header
├── .jpg                 # Sample Product images 
├── project_guide.md     # Guide for completing the milestone
└── README.md            # Milestone documentation
```

---

## **Step-by-Step Guide**

### **1. Project Setup**

#### **Create Your Project Folder**

1. Open your terminal/command line interface (CLI).
2. Navigate to the folder where you want to create your project:
   ```bash
   cd path/to/your/folder
   ```
3. Create a new folder for your project:
   ```bash
   mkdir ecommerce-store
   ```
4. Navigate into the folder:
   ```bash
   cd ecommerce-store
   ```

#### **Initialize a Git Repository**

1. Initialize Git in your project folder:
   ```bash
   git init
   ```
2. Create your first file:
   ```bash
   touch index.html
   ```
3. Stage and commit your initial file:
   ```bash
   git add index.html
   git commit -m "Initial commit with index.html"
   ```

---

### **2. Write the HTML Structure**

#### **HTML Boilerplate**

Create a basic HTML structure inside `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>E-Commerce Store</title>
  </head>
  <body>
    <!-- Add content here -->
  </body>
</html>
```

---

#### **Header Section**

1. Add a logo and navigation bar in the `<header>`:
   ```html
   <header>
     <img src="logo.png" alt="E-Commerce Logo" width="100" />
     <nav>
       <a href="#">Home</a>
       <a href="#">Products</a>
       <a href="#">Contact</a>
     </nav>
   </header>
   ```
   > **Tip**: Use placeholder links (`#`) for now.

---

#### **Main Section**

1. Create a section to list products:
   ```html
   <main>
     <section>
       <article>
         <h2>Product 1</h2>
         <img src="product1.jpg" alt="Image of Product 1" width="150" />
         <p>A short description of Product 1.</p>
         <a href="#">Add to Cart</a>
       </article>
       <article>
         <h2>Product 2</h2>
         <img src="product2.jpg" alt="Image of Product 2" width="150" />
         <p>A short description of Product 2.</p>
         <a href="#">Add to Cart</a>
       </article>
       <!-- Add more products as needed -->
     </section>
   </main>
   ```

---

#### **Footer Section**

1. Add contact information in the `<footer>`:
   ```html
   <footer>
     <p>
       Contact us: <a href="mailto:info@ecommerce.com">info@ecommerce.com</a>
     </p>
     <p>&copy; 2025 E-Commerce Store</p>
   </footer>
   ```

---

#### **Final HTML Structure**

Your completed `index.html` should look like this:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>E-Commerce Store</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header>
      <img src="logo.png" alt="E-Commerce Logo" width="100" />
      <nav>
        <a href="#">Home</a>
        <a href="#">Products</a>
        <a href="#">Contact</a>
      </nav>
    </header>
    <main>
      <section>
        <article>
          <h2>Product 1</h2>
          <img src="product1.jpg" alt="Image of Product 1" width="150" />
          <p>A short description of Product 1.</p>
          <a href="#">Add to Cart</a>
        </article>
        <article>
          <h2>Product 2</h2>
          <img src="product2.jpg" alt="Image of Product 2" width="150" />
          <p>A short description of Product 2.</p>
          <a href="#">Add to Cart</a>
        </article>
      </section>
    </main>
    <footer>
      <p>
        Contact us: <a href="mailto:info@ecommerce.com">info@ecommerce.com</a>
      </p>
      <p>&copy; 2025 E-Commerce Store</p>
    </footer>
  </body>
</html>
```

---

### **3. Version Control with Git**

As you build, commit your progress regularly:

1. After completing the header:
   ```bash
   git add index.html
   git commit -m "Add header section"
   ```
2. After completing the main section:
   ```bash
   git add index.html
   git commit -m "Add main section with product listings"
   ```
3. After completing the footer:
   ```bash
   git add index.html
   git commit -m "Add footer section"
   ```

---

### **4. Prepare for Milestone 2**

1. Create a blank CSS file for styling in Milestone 2:
   ```bash
   touch style.css
   ```
2. Link the CSS file in your `index.html` (even though it’s empty for now):
   ```html
   <head>
     <link rel="stylesheet" href="style.css" />
   </head>
   ```

---

## **Checklist**

Ensure the following before submission:

- The HTML file includes semantic tags (`header`, `main`, `footer`).
- Each product is wrapped in an `<article>` with:
  - A `<h2>` for the product name.
  - An `<img>` for the product image (placeholder allowed).
  - A `<p>` for the product description.
  - An `<a>` for the "Add to Cart" button.
- A Git repository is initialized with at least three commits:
  1. Initial setup.
  2. Header section.
  3. Main and footer sections.

---

## **Resources**

1. **HTML Reference**: [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
2. **Git Basics**: [Git Documentation](https://git-scm.com/doc)
3. **Images**: [Picsum Photos](https://picsum.photos/)

---

## **Expected Output**

By the end of this milestone, you should have:

1. A functional HTML skeleton for an e-commerce website.
2. A linked (empty) CSS file for future styling.
3. A GitHub repository with your progress.
