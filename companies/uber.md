# Uber

**Company:** Uber  
**Role:** Senior Software Engineer (Contract)  
**Duration:** 2018–2019, 2020–2021

---

# Career Context

Uber marked the most significant turning point in my engineering career.

After spending several years building customer-facing web applications, I realized that although I had become a capable frontend engineer, I had only a limited understanding of the distributed systems and backend architectures that powered modern software platforms. I wanted to become a more well-rounded software engineer, but my existing role offered few opportunities to gain that experience.

With that goal in mind, I made the difficult decision to leave a stable full-time position at ViaPath and pursue consulting opportunities where learning would take priority over familiarity. My objective was not simply to work for a well-known company, but to immerse myself in large-scale distributed systems and learn from engineers solving problems I had not previously encountered.

Uber became that opportunity.

Working on Uber's Recruiting Engineering platform exposed me to service-oriented architecture, backend development, asynchronous workflows, external system integrations, and engineering at a scale that fundamentally expanded my perspective. It was also my first introduction to Cadence, Uber's workflow orchestration platform, which reshaped how I thought about long-running business processes, reliability, and system coordination.

Looking back, this role represents the point where I consciously transitioned from primarily building applications to understanding and building the systems that power them. Many of the ideas that later influenced my work at Walmart, eBay, Shrapnel, and eventually my own open-source projects can be traced back to the foundation I built during my time at Uber.

---

# Executive Summary

Joining Uber marked a deliberate turning point in my career.

Until then, I had spent most of my professional life building front-end applications. While I enjoyed creating user interfaces and improving user experiences, I increasingly felt that my understanding of software engineering was incomplete. I had limited exposure to distributed systems, backend architecture, and the operational challenges involved in running software at large scale.

Recognizing that growth would require a fundamentally different environment, I made the difficult decision to leave a stable full-time position and pursue consulting opportunities. My objective was not simply to change employers, but to accelerate my learning by working on technically demanding systems.

Uber became that opportunity.

Working on Uber's internal recruiting platform exposed me to distributed services, asynchronous workflows, service integrations, event-driven systems, and engineering at a scale I had not previously experienced. It was also my first introduction to Cadence, Uber's workflow orchestration platform, which fundamentally changed how I thought about long-running business processes.

Looking back, this role transformed me from primarily a front-end engineer into a software engineer who began thinking in terms of systems rather than applications.

---

# Business Context

Hiring is one of Uber's most critical internal business functions.

Every candidate moves through a complex lifecycle involving recruiters, hiring managers, interviewers, calendars, video conferencing, approvals, and multiple internal systems.

The Recruiting Engineering team was responsible for building the internal tools that coordinated these workflows, allowing recruiters and hiring managers to move candidates efficiently through the hiring process.

Rather than building customer-facing features, the team built internal platforms that improved the productivity of thousands of Uber employees responsible for recruiting.

Every improvement to these systems reduced operational overhead and enabled faster, more reliable hiring.

---

# Engineering Problem

Recruiting workflows appear straightforward from the outside, but coordinating them at Uber's scale presents significant engineering challenges.

Scheduling interviews requires synchronizing multiple independent systems while respecting business rules, availability constraints, and organizational processes.

The platform integrated with services such as:

- Calendar providers
- Video conferencing platforms
- Internal recruiting systems
- Candidate management workflows
- Notification services

Failures were rarely isolated.

A missed calendar update, delayed synchronization, or failed external integration could disrupt an entire interview loop.

The engineering challenge was therefore not simply building user interfaces, but coordinating reliable workflows across distributed systems.

---

# Architecture Overview

The recruiting platform followed a service-oriented architecture where multiple independent services collaborated to execute hiring workflows.

```text
Recruiting Portal (React)
            │
            ▼
Python / Flask Services
            │
 ┌──────────┼──────────┐
 │          │          │
Calendars  Zoom   Recruiting Services
            │
            ▼
Workflow Coordination
      (Cadence)
```

The architecture emphasized:

- Independent services
- API-driven communication
- External system integrations
- Asynchronous workflow execution
- Reliable coordination across long-running business processes

---

# My Responsibilities

My responsibilities evolved over the course of the engagement and included:

- Building frontend features for recruiting applications
- Developing backend services using Python and Flask
- Designing and implementing APIs
- Integrating external services such as calendars and video conferencing
- Improving recruiting workflows
- Debugging distributed production issues
- Collaborating across multiple engineering teams
- Learning and applying workflow orchestration concepts using Cadence

This role represented my first opportunity to contribute meaningfully across both frontend and backend systems within a large distributed architecture.

---

# Key Engineering Contributions

## Expanding Beyond Frontend Development

Although I initially joined with a strong frontend background, Uber provided opportunities to contribute across the entire application stack.

Working on backend services exposed me to distributed communication, service ownership, API design, and operational debugging.

Rather than viewing software primarily through the lens of user interfaces, I began understanding how frontend applications depended on reliable backend systems and service interactions.

This shift permanently broadened my perspective as an engineer.

---

## Workflow-Oriented Thinking

One of the most influential technologies I encountered at Uber was Cadence.

Rather than modeling recruiting activities as isolated API calls, Cadence treated long-running business processes as durable workflows.

Scheduling interviews, coordinating approvals, and handling retries became explicit workflow concerns rather than scattered application logic.

Although I would not fully appreciate its significance until years later, this experience planted the foundation for my later interest in workflow orchestration and resilient distributed systems.

---

## Building Internal Platforms

The recruiting platform was not intended for external customers.

Its users were Uber employees responsible for hiring.

This changed how I thought about software value.

Internal engineering platforms can create enormous organizational leverage by improving the efficiency of thousands of employees every day.

Developer experience, operational tooling, and workflow automation became just as important as traditional customer-facing features.

---

## Integrating Distributed Systems

A significant portion of the work involved integrating multiple independent services into cohesive business workflows.

These integrations required careful handling of failures, retries, consistency, and synchronization between systems that evolved independently.

The experience highlighted that successful distributed systems are defined as much by their interactions as by the services themselves.

---

# Collaboration

Uber's engineering organization exposed me to a level of collaboration that differed significantly from my previous experience.

Engineers regularly worked across service boundaries, coordinated with product managers, recruiters, infrastructure teams, and other platform owners.

Engineering discussions often focused on system interactions, operational considerations, and long-term maintainability rather than isolated feature implementation.

This environment reinforced that building software at scale is fundamentally a collaborative effort.

---

# How This Changed My Engineering Thinking

## Software Is More Than User Interfaces

Before Uber, I primarily thought about software through the lens of frontend applications. Uber shifted my focus toward services, APIs, workflows, and distributed architectures. Applications became only one layer within much larger systems.

---

## Long-Running Business Processes Deserve First-Class Models

Cadence introduced me to the idea that workflows should be modeled explicitly rather than embedded across numerous services.

This concept fundamentally changed how I think about reliability, orchestration, retries, and operational resilience.

---

## Internal Platforms Create Organizational Leverage

Helping employees become more productive can generate organizational impact equal to—or greater than—building customer-facing features.

This appreciation for internal platforms continues to influence the kinds of problems I enjoy solving.

---

## Distributed Systems Require New Ways of Thinking

Building distributed systems involves more than learning new technologies.

It requires thinking about communication, consistency, failures, retries, observability, and coordination between independently evolving services.

Uber was my introduction to this way of thinking.

---

## Continuous Learning Is A Career Strategy

Perhaps the most important lesson from Uber was personal rather than technical.

Choosing opportunities based on learning potential rather than familiarity accelerated my growth far more than remaining within my existing comfort zone.

That decision continues to shape how I evaluate engineering opportunities today.

---

# Technologies

Languages

- Python
- JavaScript
- TypeScript

Frontend

- React

Backend

- Flask
- REST APIs

Distributed Systems

- Cadence
- Microservices
- Asynchronous workflows

Integrations

- Calendar systems
- Zoom
- Internal recruiting platforms

---

# How This Experience Influenced My Future Work

Uber fundamentally redirected my engineering career.

It transformed my interests from building applications to understanding the systems that power them.

The concepts I first encountered here—workflow orchestration, service communication, distributed coordination, and internal platforms—continued to appear throughout my later work at Walmart, eBay, and Shrapnel.

Years later, when designing open-source projects such as `batch-orchestra` and `workflow-scheduler`, I found myself returning to many of the same ideas that I had first encountered through Cadence at Uber.

Looking back, Uber was not simply another consulting engagement. It was the point at which I consciously transitioned from being primarily a front-end developer into an engineer focused on building resilient, scalable systems.