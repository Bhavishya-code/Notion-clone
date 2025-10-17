# 📝 Notion Clone: Noter

<p align="center">
<img src="https://img.shields.io/badge/Next.js-14-black?style=for-the-badge&logo=nextdotjs" alt="Next.js">
<img src="https://img.shields.io/badge/TypeScript-5-blue?style=for-the-badge&logo=typescript" alt="TypeScript">
<img src="https://img.shields.io/badge/CSS3-100%25-blue?style=for-the-badge&logo=css3" alt="CSS">
<img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel" alt="Vercel">
</p>

A sleek, minimalist web application inspired by **Notion**, offering a versatile and clean workspace for note-taking and project management. Built with a modern Next.js stack, the application emphasizes a fluid user experience and responsive design.

## 🌟 Live Demo

Check out the live version [here](https://noter-sepia.vercel.app/).



## ✨ Core Features

* **Document Management:** Seamlessly create, edit, and delete notes and documents with a focus on simplicity.
* **Rich Text Formatting:** Support for modern text editing, allowing users to format content easily.
* **Hierarchical Structure:** Full support for **nested pages and sub-pages**, enabling complex project organization akin to a true workspace tree.
* **Intuitive Reordering:** An intuitive **drag-and-drop interface** for managing page hierarchy and organizing documents.
* **Performance:** Built with **Next.js** for optimized performance and improved SEO (Search Engine Optimization).
* **Responsive Design:** Optimized for a seamless experience across desktop, tablet, and mobile devices.

---

## 🏗️ Architecture Overview

The application follows a modern component-based architecture built on the Next.js App Router, emphasizing a highly interactive user interface characteristic of a rich editor application.

### 1. Frontend & Rendering

* **Framework:** **Next.js** leverages its App Router to define dynamic routes for different pages/documents (e.g., `/docs/[id]`).
* **Strategy:** A combination of **Server Components** (for static navigation structure and initial page shell) and **Client Components** (for the rich text editor, drag-and-drop functionality, and interactive state).
* **Interactivity:** All core editing and interaction logic, including the rich text editor and drag-and-drop hierarchy, is handled client-side using **React** and **JavaScript** to ensure a fast, fluid, and responsive experience.

### 2. Data Flow (Implied for Persistence)

* **API Layer:** A dedicated API layer (built into Next.js or external) is responsible for handling all CRUD (Create, Read, Update, Delete) operations for the pages, document content, and the hierarchical page structure.
* **Content Handling:** Document content is managed within the **RichTextEditor** component, which handles the complex internal state before serializing the data (e.g., to JSON or Markdown) for storage in the database.

---
