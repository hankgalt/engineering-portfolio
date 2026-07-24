# ViaPath Technologies (formerly Telmate)

**Company:** Telmate (acquired by ViaPath Technologies)  
**Role:** Software Engineer / Senior Software Engineer  
**Duration:** 2014 – 2018

---

# Career Context

ViaPath (formerly Telmate) was the longest engagement of my early career and the period during which I matured from a developer focused on implementing features into an engineer focused on building products that could evolve over many years.

Unlike my previous roles, where I primarily contributed to individual applications, I had the opportunity to help build and continuously evolve a single platform—Command Center. Over four years, I experienced nearly every stage of a product's lifecycle, from introducing new capabilities and refining user experiences to maintaining, extending, and adapting the platform as business needs evolved.

One of the most rewarding aspects of this experience came after Telmate was acquired by ViaPath Technologies. The Command Center platform that our team had built became the primary customer administration portal for the combined organization, replacing or consolidating solutions from multiple acquired companies. Seeing software that I had helped build become part of the company's strategic value—and continue serving customers after the acquisition—fundamentally changed how I viewed the role of software engineering within a business.

This experience also reinforced the importance of long-term thinking. Building software that remains valuable for years requires more than delivering features; it requires creating maintainable architectures, reusable components, and consistent user experiences that can grow alongside the business. Those principles became a cornerstone of my engineering philosophy and influenced every role that followed.

---

# Executive Summary

My time at Telmate was one of the most formative periods of my engineering career.

When I joined, Telmate was an independent company focused on communication and technology solutions for correctional facilities. During my tenure, I helped build a modern web-based customer administration platform known as **Command Center**, which became the primary interface used by customers to manage facilities, inmate services, communication products, and operational workflows.

As Telmate continued to grow, the quality and capabilities of the Command Center became one of the factors that differentiated the company within the correctional technology market.

When Telmate was later acquired by ViaPath Technologies, the platform we had built became the primary customer administration portal for the combined organization, replacing or consolidating portals from multiple acquired companies.

Looking back, this was the first time I experienced software becoming more than a product feature—it became a strategic business asset.

---

# Business Context

Correctional facilities rely on a wide range of technology services to manage inmate communications and operational processes.

These services include:

- Video visitation
- Messaging
- Phone services
- Payments
- Trust accounts
- Facility administration
- Customer support
- Reporting
- Account management

Historically, many of these capabilities existed as separate applications with inconsistent user experiences.

As Telmate expanded its product offerings, there was a growing need for a unified administrative platform that could provide facility administrators and customer support teams with a single interface for managing the entire ecosystem.

Command Center was built to become that platform.

---

# Engineering Problem

The challenge extended far beyond building another web application.

The platform needed to:

- Bring together multiple independent business domains
- Replace fragmented administrative tools
- Support rapidly evolving business requirements
- Remain usable despite increasing complexity
- Scale as new products were introduced
- Provide a consistent experience across diverse workflows

As the company continued to grow through both product expansion and acquisition, maintaining consistency became just as important as delivering new functionality.

---

# Architecture Overview

The platform was built as a modern single-page application that interacted with multiple backend services.

```text
Facility Administrators
Customer Support
Operations Teams
          │
          ▼
React / AngularJS Customer Portal
(Command Center)
          │
          ▼
REST APIs
          │
 ┌────────┼────────┐
 │        │        │
Messaging Payments Video Services
 │
 ▼
Correctional Facility Systems
```

The architecture emphasized:

- Modular frontend development
- Reusable UI components
- Shared authentication
- Consistent user experience
- Integration across multiple backend systems

As additional services were introduced, the portal evolved into the central operational interface for customers.

---

# My Responsibilities

Over the course of four years, my responsibilities expanded significantly.

They included:

- Frontend architecture
- Building reusable UI components
- Designing complex administrative workflows
- Authentication and authorization
- Payment-related interfaces
- API integration
- Performance optimization
- Customer-facing features
- Internal administration tools
- Mentoring engineers
- Collaborating with product managers and designers

Working on the same platform over multiple years also gave me the opportunity to experience how software evolves long after its initial release.

---

# Key Engineering Contributions

## Building Command Center

The most significant project during my time at Telmate was the development of Command Center.

Rather than creating isolated pages for individual products, we built a unified platform that provided administrators with a single place to manage multiple operational workflows.

As the platform matured, it became the primary interface through which customers interacted with Telmate's services.

Following the acquisition by ViaPath, Command Center continued to serve as the primary administration portal for the combined organization, demonstrating the long-term value of investing in a well-designed platform.

---

## Creating Reusable Frontend Architecture

As the application expanded, maintaining consistency became increasingly important.

Rather than implementing each feature independently, I focused on building reusable components and shared interaction patterns that could support future functionality.

This reduced duplication, improved maintainability, and allowed the application to grow without becoming fragmented.

This experience marked the beginning of my appreciation for platform thinking and reusable abstractions.

---

## Supporting Rapid Business Growth

The business evolved continuously throughout my time at Telmate.

New products, operational requirements, and customer needs required the application to adapt without disrupting existing workflows.

Working within this environment taught me how to design software that remains flexible as business priorities change.

---

## Long-Term Product Ownership

Unlike shorter consulting engagements, I had the opportunity to work on the same platform over several years.

This exposed me to the complete lifecycle of software development:

- Initial architecture
- Feature expansion
- Refactoring
- Performance improvements
- Customer feedback
- Operational support
- Continuous evolution

Experiencing this full lifecycle fundamentally shaped my understanding of sustainable software engineering.

---

# Collaboration

Building Command Center required close collaboration across engineering, product management, design, customer support, and operations.

Because the platform served multiple business functions, engineering decisions frequently involved balancing technical considerations with usability and operational efficiency.

Working closely with customer-facing teams also provided valuable insight into how software decisions directly affect day-to-day business operations.

---

# How This Changed My Engineering Thinking

## Software Can Become A Business Asset

Before Telmate, I primarily viewed software as the implementation of product requirements.

Watching Command Center become one of the defining strengths of the company—and later the primary administration portal after acquisition—changed that perspective.

Well-designed software can become a strategic asset that directly influences business value.

---

## Platforms Outlast Features

Individual features have relatively short lifecycles.

Platforms continue to evolve for years.

Working on Command Center taught me to think beyond immediate feature requests and instead design foundations capable of supporting future growth.

---

## Consistency Creates Scale

As applications grow, consistency becomes increasingly valuable.

Reusable components, shared interaction patterns, and coherent user experiences reduce both engineering complexity and user cognitive load.

This principle has continued to influence nearly every system I have built since.

---

## Business Understanding Improves Engineering

Some of the most effective engineering decisions came from understanding how correctional facilities, customer support teams, and operations actually used the platform.

Technology became significantly more effective when grounded in real business workflows.

---

## Long-Term Ownership Changes Design Decisions

Maintaining the same system for multiple years changed how I approached engineering.

When you know you will live with your design decisions, maintainability, readability, and extensibility become much more important than delivering features as quickly as possible.

---

# Technologies

Languages

- JavaScript
- Ruby

Frontend

- AngularJS
- React
- Redux

Backend Integration

- Ruby on Rails
- REST APIs
- OAuth2 Authentication

Business Domains

- Payments
- Messaging
- Video visitation
- Facility administration
- Customer management

Development

- Git
- Agile development

---

# How This Experience Influenced My Future Work

Looking back, my years at Telmate laid the foundation for much of my later engineering philosophy.

This was where I first developed an appreciation for:

- Building platforms rather than isolated features
- Investing in reusable abstractions
- Designing software for long-term evolution
- Aligning engineering decisions with business outcomes
- Thinking about user experience as part of system architecture

Many of these principles continued to shape my work throughout the rest of my career.

Although I would later move into distributed systems, workflow orchestration, and platform engineering, the underlying mindset remained the same: build systems that continue creating value long after the initial implementation is complete.

The fact that Command Center remained the primary customer portal after Telmate's acquisition by ViaPath remains one of the accomplishments I value most, not because of the acquisition itself, but because it demonstrated that thoughtful engineering can create software with lasting strategic value.