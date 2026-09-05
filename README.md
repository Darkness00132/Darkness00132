<div align="center">

# Mustafa Mohamed Anwar

### Full-Stack .NET Developer

**Backend-focused · Building production-oriented web applications**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat\&logo=linkedin\&logoColor=white)](https://linkedin.com/in/mustafa-mohamed-anwar)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-111111?style=flat\&logo=vercel\&logoColor=white)](https://mustafa-mohamed-anwar.vercel.app)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=flat\&logo=gmail\&logoColor=white)](mailto:mustafamohamedanwar1@gmail.com)

</div>

---

## About Me

I am a **fourth-year Information Technology Management student at Port Said University**, with a **3.4 / 4.0 GPA (Very Good)**.

I started programming with C++ and problem solving, then explored Python, Node.js, React, and Next.js before specializing in **C# and .NET**.

Today, I focus primarily on **backend development with ASP.NET Core**, while continuing to build full-stack applications using modern frontend frameworks.

I am particularly interested in building systems that go beyond basic CRUD — systems with clear architecture, secure authentication, data consistency, testing, caching, and deployment workflows.

---

## What I Build

I prefer using GitHub as a record of **what I actually built**, not just a list of technologies.

Across my projects, I have worked on:

* backend systems with clear separation of domain, application, infrastructure, and API concerns
* authentication flows using access/refresh tokens, secure cookies, OAuth, roles, and policies
* transactional business workflows such as credit-based advertising and inventory operations
* automated testing across architectural boundaries
* caching strategies that account for changing underlying data
* CI/CD workflows and cloud-oriented infrastructure
* full-stack applications where the frontend is built around the API rather than tightly coupled to it

---

## Featured Projects

### ⚡ ElectroShop — Enterprise E-Commerce Backend

**A production-oriented e-commerce backend for electronics retail, currently under active development.**

[![Repository](https://img.shields.io/badge/Backend-Repository-181717?style=flat\&logo=github\&logoColor=white)](https://github.com/Darkness00132/EcommerceApi)
[![Frontend](https://img.shields.io/badge/Angular-Frontend-DD0031?style=flat\&logo=angular\&logoColor=white)](https://github.com/Darkness00132/ecommerce-ui)

The main goal of this project is not simply implementing an online store, but designing the backend so it can evolve as the system grows.

#### Engineering work

* **Structured the backend around architectural boundaries**, keeping the domain isolated while organizing application code around business features and use cases.
* **Separated commands and queries** so write operations can enforce business rules while read operations can be optimized independently.
* **Built domain-focused business logic** for carts, orders, discounts, inventory, payments, procurement, and reviews.
* **Designed inventory workflows with concurrent checkout scenarios in mind**, including stock validation and reservation-related rules intended to prevent overselling.
* **Added hybrid caching with explicit invalidation on data changes**, rather than relying only on cache expiration.
* **Implemented secure authentication flows** with JWT access tokens, refresh sessions, HttpOnly cookies for web refresh tokens, roles, and authorization policies.
* **Separated infrastructure concerns behind application contracts**, allowing integrations such as storage and external services to be replaced without changing business logic.
* **Built automated tests across architectural boundaries** with separate test projects for the **Domain, Application, and Infrastructure** layers.
* **Kept domain tests independent from databases and external infrastructure**, while using infrastructure-level tests where integration behavior actually matters.
* **Added GitHub Actions workflows** to automate build and test verification.
* **Designed the system for cloud deployment**, including Azure-oriented storage and database infrastructure.
* **Documented the domain model and requirements** alongside the implementation instead of treating the database as an afterthought.

> The repository is intentionally public so the implementation can be reviewed, discussed, and improved through future contributions.

---

### 🏠 Aqark — Real Estate Marketplace

**A full-stack Arabic real estate marketplace for brokers and property owners.**

[![Frontend](https://img.shields.io/badge/Frontend-Next.js-000000?style=flat\&logo=next.js\&logoColor=white)](https://github.com/Darkness00132/AqarkV2-frontend)
[![Backend](https://img.shields.io/badge/Backend-ASP.NET%20Core-512BD4?style=flat\&logo=dotnet\&logoColor=white)](https://github.com/Darkness00132/AqarkV2_Backend)
[![Live Demo](https://img.shields.io/badge/Live-Demo-000000?style=flat\&logo=vercel\&logoColor=white)](https://aqark.vercel.app)

The platform is designed around a broker-driven marketplace where users can publish property advertisements, discover listings, manage their profiles, and interact with reviews.

#### What I built

* **Designed a multi-criteria property filtering system** covering location, listing type, property type, price range, rooms, bathrooms, space, and sorting.
* **Implemented a credit-based advertising model**, where publishing and certain advertisement changes consume credits based on business rules.
* **Made critical advertisement operations transactional**, so operations such as image upload, credit deduction, and ad creation can roll back together when something fails.
* **Added failure cleanup for uploaded files** so external storage does not accumulate orphaned media after failed operations.
* **Implemented SEO-friendly Arabic slugs** instead of exposing database IDs in property URLs.
* **Built authentication with JWT, refresh tokens, Google OAuth, and role-based authorization.**
* **Added pagination, reviews, broker profiles, and image-based listing workflows.**
* **Built the frontend with Next.js and TypeScript** around an API-driven architecture with validation and reusable client-side logic.
* **Designed the frontend as an Arabic RTL experience** with property-focused search and filtering.

**Payment integration with Paymob: in progress.**

---

### 📦 Inventory Management System

**An ASP.NET Core MVC application for managing inventory operations from purchasing to sales.**

[![Repository](https://img.shields.io/badge/Repository-181717?style=flat\&logo=github\&logoColor=white)](https://github.com/Darkness00132/InverntoryManagement)
[![Live Demo](https://img.shields.io/badge/Live-Demo-1F6FEB?style=flat\&logo=google-chrome\&logoColor=white)](https://inventory-management.runasp.net/)

This project focuses on implementing a complete internal business application rather than only CRUD screens.

#### What I built

* **Implemented the complete inventory workflow** covering products, categories, suppliers, purchases, and sales.
* **Added automatic stock deduction** when sales are recorded.
* **Implemented reorder thresholds and low-stock reporting** to make inventory state visible to users.
* **Built dashboards and reports** for inventory value, sales revenue, purchasing history, category distribution, and low-stock items.
* **Added role-based access control** with separate Admin and Employee capabilities.
* **Implemented account management and locking** through ASP.NET Core Identity.
* **Organized ViewModels by business feature** instead of keeping one large shared model layer.

---

## Development Approach

I care more about **how a system is designed** than how many technologies are written in its README.

Some examples from my work:

```text
Business Rules
     ↓
Domain
     ↓
Application / Use Cases
     ↓
Infrastructure
     ↓
API / Presentation
```

For larger projects, I combine this dependency direction with **feature-based organization**, so a business capability owns the code needed for its use cases instead of scattering related logic across unrelated folders.

I also try to make engineering decisions based on the problem:

* use transactions where multiple operations must succeed or fail together
* isolate domain behavior from infrastructure concerns
* project only the data a client actually needs
* invalidate cached data when the underlying state changes
* test business behavior without requiring external systems
* keep external integrations replaceable
* treat authentication and authorization as part of system design rather than controller-level checks

---

## Technologies I Work With

<p align="center">
  <img src="https://skillicons.dev/icons?i=cs,dotnet,postgres,sqlserver,redis,angular,react,nextjs,ts,js,html,css,docker,git,github,azure&perline=8" />
</p>

My strongest area is **ASP.NET Core backend development**, while I use **Next.js / React and Angular** to build and integrate frontend applications.

---

## Training

**ITI — Full-Stack .NET Training**
144 hours · completed
Covered C#, OOP, SQL fundamentals, MVC, ERD, AI prompting, and freelancing.

**DEPI — Full-Stack .NET Web Developer**
6-month training · ongoing
Focused on deeper .NET development alongside software engineering practices, testing, Docker, Web APIs, MVC, and freelancing/coaching.

---

## Education

**Port Said University**
B.Sc. in Information Technology Management
Expected Graduation: **2027**
GPA: **3.4 / 4.0 — Very Good**

---

## Find Me

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-Darkness00132-181717?style=flat\&logo=github\&logoColor=white)](https://github.com/Darkness00132)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mustafa%20Mohamed%20Anwar-0A66C2?style=flat\&logo=linkedin\&logoColor=white)](https://linkedin.com/in/mustafa-mohamed-anwar)
[![Portfolio](https://img.shields.io/badge/Portfolio-mustafa--mohamed--anwar.vercel.app-111111?style=flat\&logo=vercel\&logoColor=white)](https://mustafa-mohamed-anwar.vercel.app)
[![Email](https://img.shields.io/badge/Email-mustafamohamedanwar1%40gmail.com-EA4335?style=flat\&logo=gmail\&logoColor=white)](mailto:mustafamohamedanwar1@gmail.com)

</div>
