# Shrapnel

**Company:** Shrapnel  
**Role:** Senior Software Engineer  
**Duration:** 2024 – 2025

---

# Career Context

Shrapnel represented the culmination of many of the engineering principles I had developed throughout my career.

By this point, I had gained experience building customer-facing applications, reusable platforms, distributed systems, and metadata-driven workflows. I was looking for an opportunity where I could apply those experiences to architecting systems from the ground up while working across the entire technology stack.

At Shrapnel, I had the opportunity to design and build platform capabilities that emphasized reliability, scalability, and operational simplicity. The work extended well beyond implementing individual services—it involved designing workflows, defining service boundaries, building reusable infrastructure, and improving the developer experience for the engineering organization.

This role brought together many of the lessons I had accumulated over the years. The disciplined engineering practices I learned at Williams-Sonoma, the long-term platform thinking I developed at ViaPath, the distributed systems knowledge I gained at Uber, and the governance-oriented mindset I acquired at eBay all influenced the architectural decisions I made at Shrapnel.

Looking back, Shrapnel was less about learning an entirely new discipline and more about integrating everything I had learned into a cohesive approach to software architecture. It strengthened my belief that the highest-value engineering comes from building resilient, reusable systems that enable both applications and engineering teams to evolve with confidence.

---

# Executive Summary

Shrapnel was my first opportunity to work extensively on a modern cloud-native platform built around distributed systems, durable workflows, and event-driven architecture. The platform served as the backend infrastructure for managing blockchain assets, wallets, collections, marketplace integrations, customer APIs, and developer tooling.

Unlike many of my previous projects, where I primarily focused on building business features, Shrapnel exposed me to the engineering challenges involved in evolving a large polyglot platform composed of independently deployable services written in Go, TypeScript, C#, and React.

My work focused on extending platform capabilities while preserving architectural boundaries, improving operational tooling, and building reusable infrastructure that future features could build upon.

This experience significantly influenced how I think about distributed systems, long-running workflows, API contracts, and platform engineering.

---

# Business Context

Mercury was designed as the customer-facing platform for developers building blockchain-enabled applications.

The platform provided APIs and tooling for:

- User and wallet management
- Digital asset collections
- Marketplace integrations
- Smart contract interactions
- Customer webhooks
- Administrative portal
- Migration from legacy Neon platform

One of the major operational challenges was migrating customer data from the legacy Neon platform into Mercury while maintaining data integrity and minimizing operational risk.

This migration involved millions of records across users, wallets, collections, and digital assets, requiring a durable and observable workflow rather than traditional migration scripts.

---

# Architecture Overview

The platform followed a service-oriented architecture with clearly defined service boundaries.

```text
Customer Portal (Next.js)
        │
        ▼
Hermes REST API
        │
        ▼
Go gRPC Services
        │
 ┌──────┼──────────┐
 │      │          │
Temporal MongoDB  Redis
 │                 │
 ▼                 ▼
Migration      Webhook Streaming
```

Major architectural characteristics included:

- REST APIs for public consumption
- gRPC for internal service communication
- MongoDB as the primary persistence layer
- Redis Pub/Sub for asynchronous event distribution
- Server-Sent Events (SSE) for live portal updates
- Temporal for durable operational workflows
- Polyglot implementation across Go, TypeScript, React, and .NET

---

# My Responsibilities

My work primarily focused on extending the platform while preserving its existing architectural patterns.

Areas of responsibility included:

- Temporal-based migration workflows
- Go backend services
- gRPC API evolution
- REST integration through Hermes
- Customer webhook infrastructure
- Frontend portal functionality
- Shared frontend components
- Filtering, pagination, and reusable UI infrastructure
- Operational tooling
- Testing and developer tooling

Rather than working in isolation, I collaborated closely with engineers across multiple services and technology stacks, ensuring new functionality integrated cleanly into the existing platform architecture.

---

# Key Engineering Contributions

## Durable Data Migration

One of my primary areas of work involved designing and extending durable migration workflows using Temporal.

Instead of treating migrations as one-off scripts, the platform modeled migrations as long-running workflows capable of surviving worker failures, infrastructure restarts, and transient errors.

The migration system supported:

- Batch processing
- Activity retries
- Heartbeat recovery
- Workflow resumption
- Failure isolation
- Operational visibility
- Single-record recovery workflows

This significantly improved migration reliability while reducing operational overhead during large customer migrations.

---

## API Evolution Across Multiple Service Boundaries

A seemingly simple API change required coordinated updates across multiple independently deployed services.

Typical implementation involved:

```text
protobuf
    ↓
Generated Clients
    ↓
Go Services
    ↓
Hermes REST Layer
    ↓
Customer Portal
    ↓
Tests
```

Working within this architecture reinforced the importance of maintaining stable service contracts and carefully evolving APIs without breaking downstream consumers.

---

## Event-Driven Webhook Platform

I contributed to improving the developer experience around webhook integrations.

The implementation combined:

- Redis Pub/Sub
- Server-Sent Events
- Go webhook services
- Portal UI

to provide live visibility into webhook delivery and testing.

Instead of relying on log inspection, developers could immediately observe webhook activity through the portal, significantly shortening the feedback loop during integration debugging.

---

## Reusable Frontend Infrastructure

Rather than implementing isolated UI features, I contributed reusable frontend infrastructure including:

- Shared React components
- Generic table filtering
- Pagination framework
- Redux Toolkit state management
- Storybook documentation
- Reusable modal patterns

These abstractions reduced duplication and simplified future feature development.

---

## Operational Reliability

Much of the engineering effort focused on designing for failure rather than the happy path.

Examples included:

- Retry policies
- Heartbeat recovery
- Error classification
- Partial failure handling
- Idempotent operations
- Generated mocks
- Improved testing infrastructure

These improvements increased confidence in long-running operational workflows and external integrations.

---

# Collaboration

Shrapnel reinforced that successful platform engineering is highly collaborative.

The system already consisted of multiple independently evolving services owned by different engineers and teams.

My responsibility was not to redesign the platform, but to understand existing architectural principles, extend them consistently, and collaborate across service boundaries while maintaining long-term maintainability.

This experience strengthened my appreciation for:

- Interface-first development
- Respecting architectural boundaries
- Incremental evolution of production systems
- Cross-team communication
- Designing for maintainability rather than short-term delivery

---

# What I Learned

## Durable Workflows Are Different From Background Jobs

Temporal fundamentally changed how I think about operational work.

Long-running operations should be treated as durable workflows with explicit state, retries, recovery, and observability—not simply asynchronous background tasks.

---

## Stable Contracts Enable Independent Evolution

Maintaining protobuf contracts across Go services, REST adapters, generated clients, and frontend applications demonstrated how stable interfaces allow independently deployed systems to evolve safely.

---

## Operational Tooling Is A Product Feature

Developer productivity improves dramatically when operational tooling is treated as a first-class feature.

Webhook visualization, migration monitoring, and reusable diagnostics often provide as much value as customer-facing functionality.

---

## Platform Engineering Compounds

Reusable abstractions provide significantly more long-term value than isolated feature implementations.

Well-designed filtering frameworks, shared UI components, workflow abstractions, and testing infrastructure reduce implementation effort across the entire platform.

---

## Reliability Must Be Designed

Reliability is not something added after implementation.

Retry behavior, idempotency, heartbeat recovery, observability, and failure handling should influence architectural decisions from the beginning.

---

# Technologies

Languages

- Go
- TypeScript
- React
- Next.js
- C#

Backend

- gRPC
- REST
- Protocol Buffers
- MongoDB
- Redis
- Temporal

Frontend

- Redux Toolkit
- Storybook

Infrastructure

- Docker
- Kubernetes
- Helm

---

# Looking Back

Shrapnel significantly changed the way I think about software engineering.

Prior to this role, I primarily viewed software as collections of services and business logic.

After working on Mercury, I increasingly began thinking in terms of:

- systems rather than services
- workflows rather than jobs
- contracts rather than endpoints
- platforms rather than features
- operational tooling rather than debugging
- reusable abstractions rather than isolated implementations

Many of the ideas explored later in my open-source projects—including generic workflow orchestration, reusable service frameworks, and platform-oriented design—can be traced back to lessons I learned while working on Mercury.