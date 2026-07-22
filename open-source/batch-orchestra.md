# Batch Orchestra

**Repository:** [github.com/hankgalt/batch-orchestra](https://github.com/hankgalt/batch-orchestra)

---

# Context

Throughout my career, I worked on numerous systems that needed to process millions of records reliably.

Although every project differed in business domain, they all shared remarkably similar engineering concerns:

- batching
- retries
- checkpointing
- resumability
- progress reporting
- parallelism
- failure recovery

I repeatedly found myself rebuilding similar orchestration logic.

Batch Orchestra was created to extract those recurring patterns into a reusable framework built on Temporal.

---

# Executive Summary

Batch Orchestra is a generic workflow engine for large-scale batch processing.

Rather than implementing batch execution logic independently for every project, Batch Orchestra provides reusable orchestration primitives that allow engineers to focus solely on reading and writing data.

The framework handles the operational complexity of large batch jobs while remaining independent of any specific business domain.

---

# Engineering Problem

Large batch processing introduces numerous operational challenges.

- Processing millions of records
- Activity retries
- Partial failures
- Workflow continuation
- Progress tracking
- Parallel execution
- Snapshot recovery
- Idempotency

Most implementations solve these problems repeatedly.

Batch Orchestra solves them once.

---

# Architecture

```
Source
   │
Read Batch Activity
   │
Workflow
   │
Process Batch Activity
   │
Snapshot
   │
Sink
```

The workflow itself owns orchestration while individual activities remain responsible only for business logic.

---

# Key Design Decisions

## Generic Interfaces

Rather than coupling orchestration to a particular storage technology, the framework uses generic interfaces for sources and sinks.

This allows the same workflow to support MongoDB, CSV files, SQL databases, cloud storage, or custom implementations.

---

## Separation of Concerns

Business logic remains isolated inside activities.

Workflow logic focuses exclusively on coordination, retries, scheduling, checkpointing, and recovery.

---

## Continue-As-New

Large workflows eventually accumulate execution history.

Batch Orchestra automatically supports Continue-As-New, allowing workflows processing millions of records to execute indefinitely while maintaining predictable workflow histories.

---

## Operational Visibility

The framework exposes progress information and workflow state to simplify monitoring and recovery.

Observability was considered a first-class engineering requirement rather than an afterthought.

---

# Technologies

- Go
- Temporal
- Generics
- MongoDB
- CSV
- Docker

---

# Why I Built It

Batch Orchestra represents a philosophy that has become central to my engineering approach:

Recurring engineering problems should become reusable frameworks rather than repeatedly copied implementations.

It is the direct result of lessons accumulated throughout my work at Uber, Walmart, eBay, and Shrapnel.