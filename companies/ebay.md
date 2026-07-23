# eBay

**Company:** eBay  
**Role:** Senior Software Engineer (Contract)  
**Duration:** 2023 – 2024

---

# Career Context

By the time I joined eBay, I had spent several years broadening my engineering expertise—from frontend development to distributed systems and backend services. I was looking for opportunities that would deepen my understanding of how large organizations manage complexity, particularly in systems where correctness and consistency are as important as functionality.

Working on eBay's Ontology Change Management platform provided that opportunity.

Unlike traditional application development, the platform governed changes to the product taxonomy and metadata that influenced millions of listings across the marketplace. Every modification had the potential to affect numerous downstream systems, making change management itself an engineering problem.

This role expanded my perspective beyond building software to governing how software and data evolve over time. I gained a deeper appreciation for metadata-driven systems, versioning, workflow-driven approvals, and the operational processes required to safely introduce change in a large-scale organization.

Looking back, eBay reinforced that engineering at scale is not simply about handling more traffic or larger systems—it is about creating processes, tools, and architectures that allow complex systems to evolve predictably and safely. Those lessons became invaluable in my subsequent work on distributed platforms and workflow orchestration.

---

# Executive Summary

At eBay, I worked on the Ontology Change Management platform, an internal system responsible for governing how changes to eBay's product taxonomy and knowledge graph were introduced into production.

Unlike customer-facing applications, the platform existed to help engineers, product managers, and domain experts safely evolve one of eBay's most critical assets—its product ontology—without disrupting millions of sellers, listings, APIs, or downstream systems.

The work was less about building new features and more about building confidence in change. Every modification to categories, item aspects, validation rules, or metadata required structured workflows, approvals, versioning, dependency tracking, and release coordination.

Working on this platform fundamentally changed how I think about metadata-driven systems, schema evolution, and engineering at organizational scale.

---

# Business Context

eBay's marketplace depends on structured product data.

Every listing belongs to a product category, and every category defines structured metadata such as:

- Brand
- Size
- Color
- Material
- Compatibility
- Technical specifications
- Required and optional item aspects

These structured attributes power:

- Search relevance
- Product recommendations
- Catalog matching
- Listing quality
- Buyer filtering
- Advertising
- Analytics
- Machine learning models

Because millions of active listings depend on this ontology, seemingly small metadata changes can have organization-wide consequences.

Adding a new required attribute, renaming an aspect, changing validation rules, or reorganizing category hierarchies can affect sellers, APIs, search quality, recommendation systems, and numerous downstream services.

The challenge was therefore not creating taxonomy changes—it was governing them safely.

---

# Engineering Problem

Ontology evolution is fundamentally a change-management problem.

The platform needed to coordinate:

- Proposed ontology changes
- Review workflows
- Multi-stage approvals
- Release planning
- Version tracking
- Dependency management
- Data quality validation
- Delivery timelines

The objective was to ensure that every ontology modification could be reviewed, tracked, approved, and released without introducing inconsistencies into the broader marketplace ecosystem.

Unlike traditional CRUD applications, this system modeled the lifecycle of change itself.

---

# Architecture Overview

The application consisted of a React/Redux frontend backed by GraphQL and internal services.

```text
React + Redux
        │
        ▼
GraphQL
        │
        ▼
Node.js Services
        │
        ▼
Ontology Management Services
        │
        ▼
Knowledge Graph
```

One particularly interesting aspect of the platform was its use of React Flow to visualize ontology change workflows.

Rather than representing data as static forms, the application displayed change requests as interactive workflow graphs that captured state transitions, dependencies, approvals, and release progress.

This provided users with a much clearer understanding of where a change existed within the overall release lifecycle.

---

# My Responsibilities

My work focused on extending and improving the Ontology Change Management platform.

Responsibilities included:

- React and Redux application development
- GraphQL integration
- Workflow visualization
- State management
- Dynamic form development
- Approval workflow enhancements
- Version-aware UI behavior
- Internal developer tooling
- CI/CD improvements
- Authentication and SSO integration

Throughout the project I collaborated closely with engineers, product managers, and domain specialists responsible for maintaining eBay's product taxonomy.

---

# Key Engineering Contributions

## Workflow-Centric User Experience

Unlike conventional business applications that primarily edit records, the platform centered around managing change.

The application modeled:

- Proposal
- Review
- Approval
- Validation
- Scheduling
- Release

Each stage represented a meaningful state transition rather than simply updating database records.

This experience reinforced that many enterprise systems exist primarily to coordinate people and processes rather than manipulate data.

---

## Metadata-Driven Interfaces

The ontology itself determined much of the application's behavior.

Forms, validation rules, approval states, and available actions were driven by metadata rather than hard-coded business logic.

Working within this architecture demonstrated the long-term advantages of configuration-driven systems.

Rather than requiring code changes for every new ontology rule, much of the application's behavior could evolve alongside the metadata itself.

---

## Managing Complexity Through Visualization

Representing workflow state visually proved significantly more effective than presenting users with traditional forms.

Using React Flow, complex approval chains, dependencies, and release progress became understandable at a glance.

This reinforced an important engineering lesson:

Good visualization is often as valuable as good backend architecture.

---

## Building Internal Platforms

Although the application was not customer-facing, its users were responsible for evolving one of eBay's foundational datasets.

Small usability improvements produced disproportionately large organizational benefits because they reduced friction in workflows that affected numerous downstream teams.

This shifted my thinking about internal engineering platforms.

Developer productivity and operational tooling are products in their own right.

---

# Collaboration

The project required close collaboration across multiple disciplines.

Engineering decisions frequently involved:

- Product managers
- Taxonomy specialists
- Knowledge graph engineers
- Platform engineers
- Release managers

Technical implementation was only one part of the problem.

Many discussions centered around release planning, governance, operational safety, and minimizing disruption to downstream systems.

Working within this environment strengthened my appreciation for engineering as an organizational discipline rather than purely a technical one.

---

# How This Changed My Engineering Thinking

## Metadata Is Software

Before eBay, I tended to think primarily in terms of application code.

Working on ontology management taught me that metadata often becomes the true source of system behavior.

Well-designed metadata systems can evolve significantly without requiring equivalent application changes.

---

## Schema Evolution Is Continuous

Large organizations never "finish" designing their data models.

Schemas evolve continuously.

Successful platforms are designed with controlled evolution in mind rather than assuming stable data models.

---

## Internal Platforms Create Enormous Leverage

Improving internal developer workflows can have greater long-term impact than shipping isolated customer-facing features.

Every improvement to ontology management reduced friction for future taxonomy releases across the organization.

---

## Visualization Improves Decision Making

Engineering often focuses heavily on backend architecture.

This project demonstrated that presenting system state clearly can dramatically improve user understanding and operational efficiency.

Visualization became another engineering tool—not simply a UI concern.

---

## Governance Is An Engineering Problem

I came to appreciate that governance, approvals, versioning, auditing, and release management are not bureaucratic overhead.

They are engineering mechanisms that allow large organizations to evolve safely.

---

# Technologies

Frontend

- React
- Redux
- TypeScript
- React Flow

Backend

- Node.js
- GraphQL
- gRPC

Infrastructure

- Docker
- Kubernetes
- GitHub Actions
- CI/CD

---

# How This Experience Influenced My Future Work

Working on ontology management significantly influenced how I think about reusable software architecture.

It reinforced several ideas that continued to appear in my later work:

- Configuration over hard-coded logic
- Generic workflow engines instead of feature-specific implementations
- Strong versioning and compatibility boundaries
- Metadata-driven application behavior
- Internal platforms as force multipliers
- Building reusable abstractions rather than isolated features

Looking back, I can see many of these same principles reflected in my later open-source projects, particularly around workflow orchestration, platform engineering, and reusable infrastructure.