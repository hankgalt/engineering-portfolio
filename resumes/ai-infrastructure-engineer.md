# Vishal Talwar

Seattle, WA | vtalwar.w@gmail.com | 949.202.6399 | [LinkedIn](https://www.linkedin.com/in/hankgalt/) | [GitHub](https://github.com/hankgalt) | [Portfolio](https://github.com/hankgalt/engineering-portfolio/)

## Senior Software Engineer | AI Infrastructure & Distributed Systems

## Professional Summary

Senior software engineer with 18+ years building distributed systems and developer platforms, with direct open-source work in local transformer inference, embeddings, semantic search, and vector search. Implementations include a Go embedding library built on ONNX Runtime and Hugging Face tokenization, plus ONNX embeddings and Elasticsearch vector search in Comfforts. Professional work includes Go and gRPC services, Temporal and Cadence workflows, recoverable migrations across millions of records, Kubernetes, and observability.

## Core Expertise

- **AI Infrastructure & Semantic Search:** ONNX Runtime, transformer inference, Hugging Face tokenizers, mean pooling, vector embeddings, semantic search, Elasticsearch vector search
- **Languages & Services:** Go, Python, TypeScript, gRPC, REST, Protocol Buffers
- **Workflow & Distributed Systems:** Temporal, Cadence, batch orchestration, microservices, retries, idempotency, checkpointing, failure recovery
- **Data Systems:** MongoDB, Redis, MySQL, Elasticsearch
- **Platform & Observability:** Docker, Kubernetes, Helm, OpenTelemetry, Prometheus, Grafana, Jaeger

## Selected AI & Platform Work

### [Embeddings](https://github.com/hankgalt/embeddings)

Open-source Go library created as a learning exercise and reusable interface for local transformer inference that generates sentence embeddings without a hosted AI API dependency.

- Implements ONNX Runtime execution, Hugging Face tokenization, and mean pooling to generate vector embeddings locally.
- Exposes a shared embedding interface across multiple transformer models, keeping semantic-search applications independent of model-specific implementations.

### [Comfforts Platform](https://github.com/comfforts) — Founder & Software Architect

2024–Present | Active open-source development

- Builds semantic address search from normalized addresses, ONNX embeddings, and Elasticsearch vectors, with Redis caching and MongoDB persistence.
- Defines gRPC and Protocol Buffer contracts with reusable Go and TypeScript clients across independently deployable domain services.
- Runs durable onboarding in dedicated Temporal workflow and worker components and packages local infrastructure with Kubernetes, OpenTelemetry, Prometheus, Grafana, Jaeger, and Loki.

### [Batch Orchestra](https://github.com/hankgalt/batch-orchestra)

Reusable Go and Temporal framework for resilient, domain-independent batch processing.

- Keeps batch orchestration independent of storage through generic source and sink interfaces for MongoDB, CSV, SQL, cloud storage, or custom adapters.
- Encapsulates Continue-As-New, checkpointing, retries, progress reporting, parallel execution, idempotency, and recovery for long-running workflows.

## Professional Experience

### Shrapnel — Senior Software Engineer

Consultant → Full-Time | 2024–2025

- Designed Temporal migrations for millions of user, wallet, collection, and digital-asset records with batch execution, activity retries, heartbeat recovery, workflow resumption, failure isolation, and single-record recovery.
- Evolved customer-facing APIs from Protocol Buffer contracts and generated clients through Go gRPC services, the Hermes REST layer, a Next.js portal, and automated tests.
- Connected Redis Pub/Sub, Server-Sent Events, Go webhook services, and portal UI so developers could observe webhook delivery and testing without relying on log inspection.
- Built generated mocks, reusable test infrastructure, and workflow diagnostics to improve confidence in long-running operations and external integrations.

### eBay — Senior Software Engineer

Consultant | 2023–2024

- Extended an Ontology Change Management platform governing taxonomy and knowledge-graph metadata that supported search, recommendations, analytics, and machine-learning models across the marketplace.
- Implemented metadata-driven, version-aware proposal, approval, validation, scheduling, and release workflows with taxonomy, knowledge-graph, platform, and release specialists.

### Walmart Global Tech — Senior Software Engineer

Consultant | 2021–2022

- Led discovery for Walmart Mexico's localization migration by tracing legacy data flows and dependencies, then defining an incremental path to Apollo Federation.
- Designed and implemented federated GraphQL schemas and resolvers with explicit schema ownership, entity resolution, cross-service contracts, and backward compatibility.
- Reduced request latency through service redesign and added OpenTelemetry tracing to expose service behavior during the migration.

### Uber — Senior Software Engineer

Consultant | 2018–2019, 2020–2021

- Built Python and Flask services and REST APIs for an internal recruiting platform coordinating calendars, video conferencing, and recruiting systems.
- Implemented Cadence-backed capabilities for long-running processes, making coordination, retries, and recovery explicit.
- Investigated failures across distributed integrations and worked with product, recruiting, infrastructure, and service-owning teams to resolve cross-system issues.

### Restoration Hardware — Senior Software Engineer

Consultant | 2019

- Contributed to a React and Node.js proof of concept that modeled warehouse capacity constraints and operational workflows.

### ViaPath Technologies (formerly Telmate) — Senior Software Engineer

Full-Time | 2014–2018

- Helped build and evolve Command Center, a unified administration platform that became the primary customer portal after Telmate's acquisition.

### Williams-Sonoma — Software Engineer

Full-Time | 2012–2014

- Built reusable JavaScript components and shared infrastructure for a frontend framework used across Williams-Sonoma's retail brands.

### Tickets.com — Software Engineer

Consultant → Full-Time | 2007–2012

- Built Java and Spring MVC services and JavaScript interfaces for enterprise ticketing workflows spanning venues, events, patrons, orders, returns, and reporting.

### Prounlimited — Software Engineer

Consultant | 2006–2007

- Developed Java, EJB, and Hibernate backend functionality for enterprise workforce-management software.

## Patent

**Method and Apparatus for Improving Fluid Mixing in Micro-Environments Using Magnets** — [US20090227044](https://patents.google.com/patent/US20090227044)

## Education

**Master of Science, Mechanical Engineering** — University of California, Davis

**Bachelor of Engineering, Mechanical Engineering** — Punjab Technical University

**Diploma, Software Engineering**
