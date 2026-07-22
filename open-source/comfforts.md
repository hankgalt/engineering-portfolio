# Comfforts Platform

## Overview

Comfforts is an open-source platform that I have been designing and developing to support individuals, local communities, businesses, service providers, and community organizers.

Rather than approaching the platform as a single monolithic application, I chose to build it as a collection of independently deployable services, each responsible for a well-defined business capability. This architecture allows individual components to evolve independently while maintaining clear service boundaries through typed APIs and workflow orchestration.

Although the platform is still under active development, it has become my primary vehicle for exploring modern distributed system design, workflow orchestration, developer infrastructure, geospatial intelligence, identity management, and operational tooling.

More importantly, it allows me to apply the architectural lessons I have accumulated throughout my career while experimenting with new ideas outside the constraints of commercial software.

---

# Platform Goals

The long-term vision for Comfforts is to provide infrastructure that enables local communities and organizations to collaborate more effectively.

The platform is being designed around several foundational capabilities:

- Identity and profile management
- Organization and role management
- Location intelligence
- Workflow orchestration
- Service discovery
- Communication
- Operational infrastructure
- Developer productivity

Each capability is implemented as an independent service with clearly defined ownership and interfaces.

---

# Platform Architecture

Comfforts currently consists of several collaborating services.

| Service | Responsibility |
|---------|----------------|
| **comff-profiles** | Profile, organization, onboarding, capability, and role management |
| **comff-geo** | Geocoding, routing, semantic address search, caching, and geospatial services |
| **comff-scheduler** | Workflow lifecycle management and Temporal integration |
| **comff-workflows** | Long-running business workflow orchestration |
| **comff-workers** | Temporal worker processes |
| **comff-emailer** | Email sender management and transactional email delivery |
| **comff-REST** | REST gateway over internal gRPC services |
| **comfforts-next** | Web application and backend-for-frontend |
| **comff-infra** | Kubernetes, observability, deployment, and platform infrastructure |

Together these services form a modular platform that separates business domains from orchestration, infrastructure, transport, and presentation concerns.

---

# Engineering Principles

Several architectural principles have consistently guided the development of the platform.

## Clear Domain Ownership

Each service owns a specific business capability and its corresponding data.

Rather than allowing multiple services to manipulate the same domain concepts, ownership is centralized behind well-defined APIs.

---

## Workflow-Oriented Architecture

Business processes that span multiple services are implemented as durable workflows instead of tightly coupled synchronous calls.

Temporal provides workflow durability while dedicated worker processes execute workflow logic independently from API services.

This keeps domain services focused on business capabilities while workflow services coordinate long-running operations.

---

## Strongly Typed Service Contracts

Internal communication uses gRPC and Protocol Buffers to provide strongly typed contracts between services.

Language-specific client libraries allow both Go and TypeScript applications to consume platform services consistently.

---

## Infrastructure as Code

Local development and deployment environments are treated as first-class engineering concerns.

The platform includes Kubernetes manifests, Kustomize overlays, Helm integrations, certificate management, centralized observability, and local developer automation to ensure that services can be developed and operated consistently.

---

## Observability by Design

Operational visibility is considered part of the platform architecture rather than an afterthought.

Services expose metrics and tracing, while the infrastructure integrates Prometheus, Grafana, OpenTelemetry, Jaeger, Loki, Elasticsearch, and related operational tooling.

---

# Technologies

The platform brings together a broad range of technologies, including:

- Go
- TypeScript
- Next.js
- gRPC
- Protocol Buffers
- Temporal
- MongoDB
- Redis
- Elasticsearch
- ONNX Runtime
- libpostal
- Kubernetes
- Helm
- Docker
- OpenTelemetry
- Prometheus
- Grafana
- Jaeger
- Loki

---

# What This Project Represents

Comfforts represents my continued growth as a software engineer beyond my professional work.

It is where I explore architectural ideas, validate design patterns, and build reusable platform capabilities that can evolve into production-quality systems.

More than any individual repository, Comfforts reflects how I approach software architecture: decomposing complex systems into well-defined services, keeping business capabilities independent from orchestration and infrastructure, and designing platforms that remain maintainable as they grow.

While the platform is still evolving, it demonstrates my approach to distributed systems, platform engineering, workflow orchestration, and long-term software design.