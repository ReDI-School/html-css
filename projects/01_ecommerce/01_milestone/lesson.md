# **Teacher Guide – Milestone 1: HTML Fundamentals**

## **Introduction**

This guide is designed to help instructors teach students the foundational aspects of HTML by building an e-commerce website skeleton. The lesson emphasizes semantic HTML, clean code organization, and the use of Git for version control.

---

## **Teaching Objectives**

1. **Explain Semantic HTML**:

   - Highlight the importance of semantic tags for accessibility, SEO, and maintainability.
   - Demonstrate how tags like `<header>`, `<main>`, and `<footer>` improve document structure.

2. **Introduce HTML Boilerplate**:

   - Ensure students understand the purpose of key tags like `<!DOCTYPE>`, `<html>`, `<head>`, and `<body>`.

3. **Build and Organize HTML**:

   - Guide students in creating a clean, hierarchical structure using sections and articles.
   - Emphasize the role of placeholder content for planning and prototyping.

4. **Integrate Git Version Control**:
   - Demonstrate basic Git commands for versioning the project’s progress.

---

## **Classroom Flow**

### **1. Setting the Stage: What is Semantic HTML?**

Start by explaining the concept of semantic HTML:

- **Why it matters**: Accessibility, SEO, and future-proofing code.
- **Common semantic tags**:
  - `<header>`: For branding and navigation.
  - `<main>`: To enclose the central content.
  - `<footer>`: For contact information and copyright.

#### **Discussion Prompts**:

- What are the benefits of using `<section>` and `<article>` instead of `<div>`?
- How does semantic HTML help search engines understand content?

---

### **2. Hands-On: Building the E-Commerce Skeleton**

#### **Header Section**

- Introduce the `<header>` tag as the container for the site’s branding and navigation.
- Guide students in adding a placeholder logo and navigation links.

**Key Teaching Points**:

- The importance of the `alt` attribute in `<img>` for accessibility.
- Using placeholder links (`href="#"`) during initial development.

**Code Example**:

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

#### **Main Content**

- Explain how `<main>` represents the core content and is vital for accessibility.
- Show how to group products into `<section>` and represent each product with `<article>`.

**Code Example**:

```html
<main>
  <section>
    <article>
      <h2>Product 1</h2>
      <img src="product1.jpg" alt="Image of Product 1" width="150" />
      <p>A short description of Product 1.</p>
      <a href="#">Add to Cart</a>
    </article>
  </section>
</main>
```

#### **Footer**

- Use `<footer>` for contact information and copyright details.
- Highlight the role of anchor links and email links in web development.

**Code Example**:

```html
<footer>
  <p>Contact us: <a href="mailto:info@ecommerce.com">info@ecommerce.com</a></p>
  <p>&copy; 2025 E-Commerce Store</p>
</footer>
```

---

### **3. Version Control with Git**

- Explain why version control is essential in modern web development.
- Teach students the basic Git workflow:
  1. `git init`: Initialize the repository.
  2. `git add`: Stage files.
  3. `git commit`: Save progress with descriptive messages.

#### **Suggested Commit Messages**:

1. "Initial commit with index.html"
2. "Added header section"
3. "Completed main section and footer"

---

### **4. Classroom Activities**

- **Activity 1**: Have students write the boilerplate and header structure on their own.
- **Activity 2**: Pair students to create and organize product listings using `<section>` and `<article>`.
- **Activity 3**: Discuss and implement the footer as a class.

---

## **Common Mistakes to Address**

1. **Missing or Misused Semantic Tags**:
   - Emphasize when to use `<section>`, `<article>`, and `<div>`.
2. **No Alt Text for Images**:
   - Remind students that `<img>` should always include an `alt` attribute for screen readers.
3. **Disorganized HTML Structure**:
   - Encourage proper indentation and logical grouping of content.

---

## **Learning Outcomes**

By the end of the lesson, students should:

1. Understand and use semantic HTML tags.
2. Build a skeleton e-commerce website with clean, organized HTML.
3. Utilize Git for version control with multiple commits.

---

## **Additional Resources**

- **Semantic HTML Guide**: [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- **Git Basics**: [Git Documentation](https://git-scm.com/doc)
- **Placeholder Images**: [Picsum Photos](https://picsum.photos/)

---
