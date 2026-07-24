# Tickets.com

**Company:** Tickets.com  
**Role:** Software Engineer II (Consultant → Full-Time Employee)  
**Duration:** 2007 – 2012

---

# Career Context

Tickets.com was my first long-term software engineering role and the position where I developed confidence in my ability to build and maintain large commercial software systems.

I initially joined as a consultant after completing a six-month engagement at ProUnlimited. My manager at Tickets.com strongly advocated for converting me to a full-time employee, giving me the opportunity to establish myself within a mature engineering organization and contribute to a major software platform over several years.

The application I helped develop was **ProVenue**, Tickets.com’s digital ticketing and event-management platform. Tickets.com is a wholly owned subsidiary of Major League Baseball and provides ticketing technology for sports teams, entertainment venues, theatres, arenas, universities, museums, festivals, and arts organizations worldwide. The company reports supporting more than one million live events and approximately 95 million ticket sales annually.

During my tenure, ProVenue was being developed as a new generation of the company’s ticketing platform. My work included user interfaces, services, and operational tools supporting venues, events, patrons, ticket transactions, reporting, and large-scale ticket-management processes.

This role marked the point at which software engineering became not simply a career choice, but a profession in which I knew I could succeed.

---

# Executive Summary

At Tickets.com, I contributed to the design and development of ProVenue, an enterprise ticketing and event-management platform used by professional sports organizations, entertainment venues, and arts organizations.

My work covered both frontend and backend development. I built administrative interfaces for managing core ticketing entities, developed services supporting operational and transactional workflows, and contributed tools for researching order history, processing bulk ticket returns, and managing report access and templates.

The role gave me sustained exposure to a large, commercially important Java application with interconnected business domains and complex operational requirements. It was where I learned to navigate an established codebase, translate ticketing operations into software, collaborate within a professional engineering team, and take responsibility for features used as part of a broader enterprise platform.

---

# Business Context

Tickets.com develops ticketing technology for sports organizations, entertainment venues, theatres, universities, museums, festivals, and other live-event operators. The company is a wholly owned subsidiary of Major League Baseball and operates ProVenue as its primary ticketing and event-management platform. :contentReference[oaicite:1]{index=1}

Unlike a consumer-facing website concerned only with ticket purchases, ProVenue supports the broader operational lifecycle behind ticketing. Venue and event personnel use the platform to configure venues, create and manage events, maintain patron information, research transactions, process ticket operations, and access operational reports.

The system therefore had to represent and coordinate several interconnected business domains:

- venues and their seating or operational structures;
- events and performances;
- patrons and customer records;
- orders and ticket transactions;
- ticket returns and exchanges;
- reporting and report-template access;
- administrative and operational workflows.

ProVenue served organizations whose ticketing operations could involve high transaction volumes, large event inventories, and complex customer-service workflows. This required the application to provide not only customer-facing ticketing capabilities but also reliable tools for venue administrators, box-office personnel, and support teams.

My contributions were primarily within these operational and administrative parts of the platform.

---

# Engineering Problem

The engineering challenge was to help build a new ticketing platform capable of representing complex venue and event operations while remaining usable by the personnel responsible for managing them.

Ticketing is more than issuing a seat for an event. The platform needed to coordinate relationships among venues, events, patrons, orders, tickets, reports, and operational processes. Actions such as researching an order or returning a group of tickets could involve multiple records and business rules while still needing to present a clear workflow to the user.

My work focused on translating these business operations into maintainable web interfaces and supporting services.

The principal problems included:

- creating administrative interfaces for complex ticketing entities;
- exposing backend functionality through maintainable service and controller layers;
- supporting transaction and order-history research;
- processing bulk ticket-return operations;
- managing reporting access and report templates;
- maintaining consistency between user-facing workflows and underlying ticketing data;
- contributing within an evolving enterprise Java platform developed by multiple engineers.

---

# Architecture Overview

ProVenue was developed as a Java enterprise web application using a layered architecture.

My work primarily involved:

- browser-based administrative interfaces built with JavaScript, Prototype, JST, AJAX, and JSON;
- Java web controllers and application functionality built with Spring MVC;
- J2EE services supporting ticketing and operational workflows;
- integration between user-interface components and backend business operations.

A simplified view of the areas in which I worked is:

```text
Venue and Event Personnel
          |
          v
Administrative Web Interfaces
JavaScript / Prototype / JST / AJAX
          |
          v
Spring MVC Controllers and Services
          |
          v
Ticketing Business Operations
Venues | Events | Patrons | Orders | Returns | Reports
          |
          v
ProVenue Platform Data and Services
```

The architecture emphasized:

- Transactional consistency
- Reliable order processing
- Responsive user interfaces
- Integration with enterprise backend systems

---

# My Responsibilities

During my time at Tickets.com, I contributed to several customer-facing and administrative applications.

Responsibilities included:

- developing frontend components and administrative views for ProVenue;
- implementing Java and Spring MVC backend functionality;
- building interfaces for managing venues, events, patrons, and related ticketing data;
- developing services supporting ticket transaction and order-history research;
- implementing functionality for batched bulk ticket returns;
- contributing report-access and report-template management features;
- diagnosing defects across frontend and backend layers;
- collaborating with product, quality-assurance, and engineering team members;
- maintaining and extending features within a large existing application.

As my experience grew, I took on increasingly complex work and became a trusted contributor within the engineering team.

---

# Key Engineering Contributions

### ProVenue Platform Development

Contributed to the development of ProVenue, Tickets.com’s enterprise ticketing and event-management platform.

The platform supported core operational domains such as venues, events, patrons, orders, ticket transactions, and reporting. My work crossed the user-interface and service layers, giving me experience implementing complete business workflows rather than isolated page components.

### Venue, Event, and Patron Management

Developed administrative user interfaces and supporting functionality for managing important ticketing entities.

These interfaces enabled venue and event personnel to configure and maintain operational information through structured workflows rather than manipulating underlying records directly.

### Order and Transaction-History Research

Designed and implemented interfaces and services that helped operational personnel research ticket orders and transaction history.

This functionality supported customer-service and box-office workflows in which personnel needed to understand the sequence of actions associated with an order or ticket transaction.

### Batched Bulk Ticket Returns

Developed functionality supporting batched returns of multiple tickets.

This work required translating a potentially repetitive and error-prone manual operation into a structured application workflow capable of handling groups of ticket records consistently.

### Reporting and Template Management

Contributed functionality for controlling access to reports and managing report templates.

Reporting was an important operational capability for venues and event organizations, and these features helped make platform information accessible through managed and reusable reporting configurations.

---

# How This Changed My Engineering Thinking

Tickets.com was where I gained confidence as a professional software engineer.

The scale and commercial significance of ProVenue showed me that I could contribute meaningfully to a substantial enterprise application rather than only small or short-lived projects.

The role taught me several foundational lessons:

### Understanding the Domain Is Part of Engineering

Ticketing involved much more operational complexity than was visible to customers purchasing seats. Building useful software required understanding how venue administrators, box-office personnel, customer-service representatives, and event organizers actually performed their work.

### Enterprise Applications Are Networks of Business Relationships

Venues, events, patrons, orders, tickets, transactions, and reports were not independent entities. A change in one area could influence workflows elsewhere. This taught me to think beyond individual screens and understand the wider business system.

### User Interfaces Encode Operational Processes

Administrative interfaces were not simply presentation layers. They shaped how users researched orders, maintained event data, returned tickets, and accessed reports. A good interface had to preserve business rules while making complex operations understandable.

### Long-Term Contribution Builds Engineering Confidence

Working on the same commercial platform for approximately five years allowed me to see features evolve, understand the effects of design decisions, maintain code written by others, and take increasing ownership of my work.

By the time I left Tickets.com, I no longer questioned whether I could succeed as a software engineer. I had contributed for several years to the development of a commercially significant platform used by major organizations.

---

# Technologies

Languages

- Core JAVA
- JavaScript
- HTML
- CSS

Frontend

- JavaScript
- AJAX
- Enterprise web applications

Backend Integration

- Spring MVC
- REST APIs
- Enterprise services

Development

- Agile development
- Source control
- Team collaboration

---

# How This Experience Influenced My Future Work

Looking back, Tickets.com gave me something far more valuable than technical skills.

It gave me confidence.

Confidence to pursue increasingly difficult engineering challenges.

Confidence to leave my comfort zone.

Confidence to transition from frontend development into distributed systems years later.

Confidence to join companies like Uber, Walmart, eBay, and Shrapnel, where I intentionally sought opportunities that would expand my understanding of software engineering.

Every stage of my career can be traced back to the belief I developed at Tickets.com—that with curiosity, discipline, and persistence, I could continue learning and solving increasingly complex problems.

In many ways, Tickets.com was not just where my software engineering career began. It was where I became a software engineer.