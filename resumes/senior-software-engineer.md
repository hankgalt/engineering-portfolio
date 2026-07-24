# Vishal Talwar

Seattle, WA | vtalwar.w@gmail.com | 949.202.6399 | [LinkedIn](https://www.linkedin.com/in/hankgalt/) | [GitHub](https://github.com/hankgalt) | [Portfolio](https://github.com/hankgalt/engineering-portfolio/)

## Senior Software Engineer | Distributed Systems & Platform Architecture

## Professional Summary

Senior software engineer with 18+ years of experience building distributed platforms, workflow systems, and enterprise applications. Recent work includes recoverable Temporal migrations across millions of records at Shrapnel, Walmart Mexico's Apollo Federation migration, and ontology-governance workflows at eBay. Work has ranged from defining service boundaries and API contracts to planning incremental migrations, designing failure recovery, instrumenting services, and building developer tooling in Go, Python, and TypeScript.

## Core Expertise

- **Architecture & APIs:** Distributed systems, service boundaries, API contracts, gRPC, REST, Apollo Federation, metadata-driven systems
- **Workflow & Reliability:** Temporal, Cadence, batch orchestration, retries, idempotency, checkpointing, recovery
- **Platform & Observability:** Developer platforms, AWS, GCP, Docker, Kubernetes, Helm, OpenTelemetry, Prometheus, Grafana, Jaeger
- **Languages & Data:** Go, Python, Ruby, TypeScript, React, MongoDB, Redis, MySQL, Elasticsearch

## Professional Experience

### Shrapnel — Senior Software Engineer

Consultant → Full-Time | 2024–2025

- Made migrations across millions of user, wallet, collection, and digital-asset records recoverable by designing Temporal workflows with batching, retries, heartbeat recovery, resumability, failure isolation, and single-record recovery.
- Evolved customer-facing APIs end to end—from Protocol Buffers and generated clients through Go gRPC services, the Hermes REST layer, and the Next.js portal—while maintaining consistent contracts across independently deployed components.
- Added live webhook delivery and testing visibility by connecting Redis Pub/Sub, Server-Sent Events, Go webhook services, and the portal, shortening the feedback loop for integration debugging.
- Created shared filtering, pagination, UI components, generated mocks, and workflow diagnostics to reduce duplication and support future platform work.

### eBay — Senior Software Engineer

Consultant | 2023–2024

- Extended the Ontology Change Management platform that governed taxonomy and knowledge-graph changes affecting millions of marketplace listings and multiple downstream systems.
- Implemented metadata-driven, version-aware forms and actions for proposals, validation, approvals, scheduling, and releases so application behavior could evolve with ontology rules instead of hard-coded UI logic.
- Visualized approval chains, dependencies, state transitions, and release progress with React Flow, giving platform users a clearer view of complex change workflows.
- Translated governance requirements from product, taxonomy, knowledge-graph, platform, and release stakeholders into workflows that balanced usability with operational safety.

### Walmart Global Tech — Senior Software Engineer

Consultant | 2021–2022

- Led discovery for Walmart Mexico's localization migration by tracing legacy data flows, dependencies, and consumer requirements, then defining an incremental path to Apollo Federation.
- Designed and implemented federated GraphQL schemas and resolvers with explicit schema ownership, entity resolution, cross-service contracts, and backward compatibility.
- Preserved existing functionality while federated services were introduced, treating backward compatibility and rollout safety as architecture constraints.
- Reduced request latency through service redesign and added OpenTelemetry tracing to expose service behavior during the migration.

### Uber — Senior Software Engineer

Consultant | 2018–2019, 2020–2021

- Built Python and Flask services, REST APIs, and React features for an internal recruiting platform coordinating calendars, video conferencing, and recruiting systems.
- Implemented Cadence-backed capabilities for long-running recruiting workflows, making coordination, retries, and recovery explicit.
- Investigated failures across distributed integrations and worked with product, recruiting, infrastructure, and service-owning teams to resolve issues across system boundaries.

### Restoration Hardware — Senior Software Engineer

Consultant | 2019

- Contributed React interfaces and Node.js services to a warehouse capacity-planning proof of concept, becoming productive quickly in an unfamiliar distributed architecture.

### ViaPath Technologies (formerly Telmate) — Senior Software Engineer

Full-Time | 2014–2018

- Helped build and evolve Command Center, a unified administration platform spanning facility operations, communications, payments, customer management, and reporting; it became the primary customer portal after Telmate's acquisition.
- Shaped frontend architecture and reusable components across React, Redux, and AngularJS, enabling the platform to absorb new products and business workflows without fragmenting the user experience.
- Mentored engineers and worked with product, design, support, and operations to evolve the same platform through four years of feature growth, refactoring, performance work, and production support.

### Williams-Sonoma — Software Engineer

Full-Time | 2012–2014

- Built reusable components and shared application infrastructure for a modular frontend framework used across Williams-Sonoma's retail brands, reducing duplicate implementation and giving product teams consistent integration patterns.

### Tickets.com — Software Engineer

Consultant → Full-Time | 2007–2012

- Built Java, Spring MVC, and JavaScript workflows for ProVenue covering venue and event administration, order-history research, batched ticket returns, and report-template access.

### Prounlimited — Software Engineer

Consultant | 2006–2007

- Developed and maintained enterprise workforce-management software.

## Selected Open-Source & Platform Work

### [Comfforts Platform](https://github.com/comfforts) — Founder & Software Architect

2024–Present | Active open-source development

- Architected Comfforts as independently deployable services with explicit ownership for identity, geospatial intelligence, workflow orchestration, email delivery, gateway, web, and infrastructure concerns.
- Defined gRPC and Protocol Buffer contracts with reusable Go and TypeScript clients, and separated long-running onboarding from domain services through dedicated Temporal workflow and worker components.
- Made local development and deployment reproducible with Kubernetes, Helm, Kustomize, and integrated observability through OpenTelemetry, Prometheus, Grafana, Jaeger, and Loki.

### [Batch Orchestra](https://github.com/hankgalt/batch-orchestra)

Reusable Go and Temporal framework for resilient, domain-independent batch processing.

- Created generic source and sink interfaces that keep orchestration independent of MongoDB, CSV, SQL, cloud storage, or custom adapters.
- Encapsulated Continue-As-New, checkpointing, retries, progress reporting, parallel execution, idempotency, and recovery for long-running workflows.

### [Workflow Scheduler](https://github.com/hankgalt/workflow-scheduler)

Distributed workflow-scheduling project focused on secure communication, observability, and operational simplicity.

- Designed Go scheduling services around gRPC and mutual TLS, with OpenTelemetry, Prometheus, Grafana, and Jaeger embedded in the architecture.

## Patent

**Method and Apparatus for Improving Fluid Mixing in Micro-Environments Using Magnets** — US20090227044

## Education

**Master of Science, Mechanical Engineering** — University of California, Davis

**Bachelor of Engineering, Mechanical Engineering** — Punjab Technical University

**Diploma, Software Engineering**
