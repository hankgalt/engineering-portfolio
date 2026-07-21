# Walmart International

**Company:** Walmart International  
**Role:** Senior Software Engineer (Contract)  
**Duration:** September 2021 – September 2022

---

# Executive Summary

At Walmart International, I worked on migrating Walmart Mexico's content platform to a modern GraphQL-based architecture built on Apollo Federation.

Unlike many engineering projects where the implementation path is well understood, this project began with only a broad objective: migrate the existing functionality into the new platform. The technical requirements, migration strategy, dependencies, and implementation details were largely undefined.

The most significant challenge was not writing code—it was reducing ambiguity.

Success required understanding an unfamiliar system, identifying the missing requirements, working within Walmart's formal engineering processes, and gradually building a migration strategy that integrated cleanly into an existing large-scale distributed platform.

This project fundamentally changed how I approach engineering problems with incomplete information and reinforced the importance of architecture, communication, and systematic discovery before implementation.

---

# Business Context

Walmart International operates multiple regional e-commerce platforms, each with different business requirements, product catalogs, localization rules, and customer experiences.

As the organization modernized its platform architecture, Walmart Mexico began migrating content services toward a federated GraphQL platform.

The objectives included:

- Modernizing API architecture
- Standardizing service boundaries
- Supporting multiple regional marketplaces
- Improving frontend developer experience
- Simplifying data access
- Enabling independent evolution of backend services

Rather than exposing numerous REST endpoints, the new architecture aimed to present a unified GraphQL schema capable of composing data from multiple backend services.

---

# Engineering Problem

The migration itself was intentionally described at a very high level.

Rather than receiving detailed implementation specifications, I was given the overall business objective and expected to determine:

- What functionality existed in the legacy implementation
- Which services participated in the migration
- How data flowed through the existing system
- Which APIs needed to be preserved
- What new GraphQL schema should expose
- How to migrate functionality without disrupting existing consumers
- How to work within Walmart's established development, review, and release processes

The engineering challenge therefore became one of discovery rather than implementation.

Before writing code, I first needed to understand the problem.

---

# Architecture Overview

The migration centered around Apollo Federation, allowing multiple independently owned services to contribute to a unified GraphQL API.

```text
Frontend Applications
        │
        ▼
Apollo Gateway
        │
 ┌──────┼────────────┐
 │      │            │
Content Product Catalog Pricing
Service     Service      Service
        │
        ▼
Regional Data Sources
```

The Content Service acted as one of the federated GraphQL services responsible for exposing localized content consumed by Walmart Mexico.

The architecture emphasized:

- Independent service ownership
- Federated GraphQL schemas
- Strong service contracts
- Backward compatibility
- Incremental migration

---

# My Responsibilities

My responsibilities extended well beyond implementing assigned tasks.

They included:

- Understanding the legacy implementation
- Identifying migration requirements
- Designing migration approach
- Building GraphQL resolvers
- Migrating backend functionality
- Schema evolution
- API integration
- Performance optimization
- Observability improvements
- Cross-team collaboration
- Working within Walmart's engineering governance and release processes

A significant portion of the project involved investigation, architectural understanding, and requirement discovery before implementation began.

---

# Key Engineering Contributions

## Engineering Through Ambiguity

The defining characteristic of this project was ambiguity.

The migration objective was clear, but the implementation path was not.

Rather than immediately writing code, I spent considerable time understanding the existing platform, identifying dependencies, tracing data flows, and determining what the new architecture actually required.

This experience reinforced that successful engineering often begins with asking better questions rather than producing faster code.

---

## Apollo Federation Migration

The migration introduced me to GraphQL Federation at enterprise scale.

Instead of building isolated APIs, each service contributed a portion of the overall schema while remaining independently deployable.

This architectural style required careful consideration of:

- Schema ownership
- Entity resolution
- Cross-service contracts
- Backward compatibility
- Service composition

The experience broadened my understanding of distributed API design beyond traditional REST services.

---

## Incremental Migration

The migration was performed incrementally rather than through a large-scale replacement.

Existing functionality had to remain operational while new GraphQL services were introduced gradually.

This required balancing modernization with production stability.

The experience reinforced that successful migrations are usually evolutionary rather than revolutionary.

---

## Performance and Observability

As functionality moved into the new architecture, performance and visibility became increasingly important.

I worked on improving request latency while introducing observability that made it easier to understand service behavior during migration.

This highlighted the relationship between system visibility and engineering confidence.

Modern distributed systems cannot be effectively maintained without strong observability.

---

## Working Within Formal Engineering Processes

Walmart's engineering organization emphasized formal development practices including architecture reviews, code reviews, release processes, and structured collaboration across teams.

Initially this felt slower than smaller organizations.

Over time I realized that these processes existed to support coordination across hundreds of engineers working on interconnected systems.

The experience strengthened my appreciation for disciplined engineering practices at organizational scale.

---

# Collaboration

The migration required collaboration across multiple engineering teams responsible for different portions of the federated platform.

Much of the work involved:

- Clarifying requirements
- Understanding existing services
- Discussing schema ownership
- Coordinating integration points
- Aligning implementation with organizational standards

Rather than simply implementing assigned tickets, I frequently participated in discovering what the correct implementation should be.

---

# How This Changed My Engineering Thinking

## Ambiguity Is Part Of Engineering

One of the most valuable lessons from Walmart was that engineering problems rarely arrive fully defined.

Learning how to reduce ambiguity through investigation, communication, and experimentation became just as important as implementation itself.

---

## Architecture Exists To Enable Independent Teams

Apollo Federation demonstrated that architecture is ultimately about organizational scalability.

Well-defined service boundaries allow teams to evolve independently while maintaining a coherent platform.

---

## Migration Is Product Development

Successful migrations require as much engineering discipline as building entirely new systems.

Compatibility, incremental rollout, and operational safety become primary design constraints.

---

## Process Can Enable Scale

Before Walmart, I often viewed formal engineering processes primarily as overhead.

Working within a large engineering organization changed that perspective.

When hundreds of engineers contribute to the same platform, consistent engineering practices become essential for maintaining quality and stability.

---

## Observability Creates Confidence

The migration reinforced that metrics, tracing, and visibility are not operational afterthoughts.

They are essential tools that allow engineers to safely evolve distributed systems.

---

# Technologies

Languages

- Go
- TypeScript
- JavaScript

Backend

- GraphQL
- Apollo Federation
- gRPC
- REST

Cloud & Infrastructure

- Kubernetes
- Docker
- Google Cloud Platform

Observability

- OpenTelemetry
- Prometheus
- Grafana
- Jaeger

Development

- Git
- CI/CD

---

# How This Experience Influenced My Future Work

Looking back, Walmart fundamentally changed how I approach unfamiliar engineering problems.

Rather than immediately searching for technical solutions, I now spend considerably more time understanding the system, identifying constraints, and clarifying objectives before implementation begins.

This experience also deepened my appreciation for distributed APIs, observability, incremental migration strategies, and architecture that enables independent teams to evolve safely.

Many of these ideas later influenced my own open-source work, particularly around building reusable infrastructure, emphasizing observability, and designing systems that can evolve incrementally without disrupting existing users.