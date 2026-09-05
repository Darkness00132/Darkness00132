<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=220&section=header&text=Mustafa%20Mohamed%20Anwar&fontSize=42&fontAlignY=38&animation=fadeIn&desc=Full-Stack%20.NET%20Developer&descAlignY=61&descSize=19" width="100%"/>

<a href="https://readme-typing-svg.demolab.com/">
<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=19&duration=2800&pause=1200&color=58A6FF&center=true&vCenter=true&width=700&height=42&lines=Backend-focused+Full-Stack+Developer;Building+real-world+.NET+applications;Architecture+%7C+Security+%7C+Testing+%7C+Performance" alt="Typing SVG"/>
</a>

</div>

<p align="center">
  <a href="https://linkedin.com/in/mustafa-mohamed-anwar" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:mustafamohamedanwar1@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <a href="https://mustafa-mohamed-anwar.vercel.app" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/>
  </a>
  <a href="https://github.com/Darkness00132" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
</p>

## 👋 About Me

I'm a fourth-year **Information Technology Management** student at **Port Said University**, currently focusing on **backend development with C# and ASP.NET Core** while continuing to build full-stack applications.

My path started with programming fundamentals and problem solving, then moved through Python, Node.js, React, and Next.js before I chose **.NET as my main backend ecosystem**.

That shift changed what I wanted from my projects. Instead of only building applications that work, I became more interested in **how they behave under real requirements**:

* keeping business rules separate from infrastructure
* designing authentication and authorization deliberately
* handling data consistency and transactional operations
* testing behavior without coupling tests to implementation details
* thinking about caching and performance before problems appear
* making external services replaceable instead of hard-wired into the application

Most of what you see in my repositories comes from trying to solve those problems in actual projects.

---

## 🛠️ What I Do

### Backend

I mainly build APIs and business applications with **ASP.NET Core**, with a strong focus on the application and domain layers.

I use patterns such as **CQRS and Vertical Slice Architecture** when they make the use cases easier to evolve, while keeping the dependency direction and business rules clear.

I'm particularly interested in problems around:

**authentication & authorization · transactional workflows · inventory · caching · data access · validation · exception handling · API design**

### Testing

Testing is part of how I develop, not something added at the end.

In my main e-commerce project, I separated tests according to architectural boundaries:

* **Domain tests** run without database or infrastructure dependencies.
* **Application tests** focus on application behavior and use-case logic.
* **Infrastructure tests** cover integration behavior where external dependencies actually matter.

The project uses **xUnit, Moq, FluentAssertions**, and integration testing rather than trying to unit-test every implementation detail.

### Performance & Reliability

I try to solve performance and reliability problems at the design level.

For example, in ElectroShop I implemented **hybrid caching with explicit invalidation when underlying data changes**, rather than treating expiration as the only cache strategy.

I also design DTOs and projections around **the data the client actually needs**, instead of returning entire entities by default.

### Security

My projects include practical security concerns such as:

**JWT access/refresh authentication · secure HttpOnly cookies · role-based authorization · CORS · rate limiting · account protection**

The goal is not simply to "add authentication", but to make the authentication model fit the client and application flow.

### Full-Stack

Although backend is where I spend most of my time, I build the frontend needed to complete my applications.

I've worked with **Next.js, React, TypeScript, and Angular**, especially when integrating a frontend with APIs I designed myself.

---

## 🚀 Main Projects

### ⚡ ElectroShop

[![Backend](https://img.shields.io/badge/Backend-Repository-181717?style=flat\&logo=github\&logoColor=white)](https://github.com/Darkness00132/EcommerceApi)
[![Frontend](https://img.shields.io/badge/Frontend-Repository-181717?style=flat\&logo=github\&logoColor=white)](https://github.com/Darkness00132/ecommerce-ui)

An enterprise-style e-commerce backend for electronics, currently under active development.

The project covers much more than products and orders. It includes identity, catalog, carts, checkout, payments, inventory, procurement, reviews, promotions, and media handling.

What makes it important to me is the engineering behind it:

* Clean Architecture with domain/application/infrastructure separation
* CQRS and Vertical Slice organization
* hybrid caching with change-based invalidation
* inventory workflows designed around concurrent operations
* secure web and native authentication flows
* separate Domain, Application, and Infrastructure test projects
* GitHub Actions CI
* infrastructure contracts for replaceable external services
* Azure Blob Storage as the production storage target

---

### 🏠 Aqark

[![Backend](https://img.shields.io/badge/Backend-Repository-181717?style=flat\&logo=github\&logoColor=white)](https://github.com/Darkness00132/AqarkV2_Backend)
[![Frontend](https://img.shields.io/badge/Frontend-Repository-181717?style=flat\&logo=github\&logoColor=white)](https://github.com/Darkness00132/AqarkV2-frontend)
[![Live](https://img.shields.io/badge/Live-Demo-000000?style=flat\&logo=vercel\&logoColor=white)](https://aqark.vercel.app)

A full-stack Arabic real-estate marketplace built for brokers and property owners.

The project is centered around property discovery, and one of the larger pieces I implemented was a **multi-criteria filtering system** supporting location, listing type, property type, rooms, bathrooms, price, space, and sorting.

Other work includes:

* SEO-friendly property URLs using slugs
* JWT and Google OAuth authentication
* role-based authorization
* transactional credit-based advertising
* property images and broker profiles
* reviews and pagination
* Arabic RTL frontend built with Next.js and TypeScript

**Paymob payment integration is currently in progress.**

---

## 🔭 Currently Building

I'm continuing work on both **ElectroShop** and **Aqark**, while deepening my backend engineering skills through the ongoing **DEPI Full-Stack .NET Web Developer** program.

My current focus is less about collecting technologies and more about getting better at:

**designing systems · writing testable code · handling real business rules · understanding trade-offs · building applications that can evolve**

---

## 🧰 Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=cs,dotnet,sqlserver,postgres,redis,nextjs,react,angular,ts,docker,git,github,azure&perline=7" />
</p>

---

<div align="center">

### Thanks for stopping by.

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer&animation=fadeIn" width="100%"/>

</div>
