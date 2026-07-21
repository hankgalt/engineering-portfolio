# Workflow Scheduler

**Repository:** github.com/hankgalt/workflow-scheduler

---

# Context

While working with distributed systems, I repeatedly encountered the same operational challenge:

How do you reliably schedule workflows across multiple services while maintaining security, observability, and operational simplicity?

Existing schedulers often focused only on execution.

I wanted to explore what a modern workflow scheduling platform would look like if reliability and developer experience were treated as first-class concerns.

---

# Executive Summary

Workflow Scheduler is a distributed scheduling service built around gRPC, mutual TLS, observability, and durable execution.

Rather than being a simple cron replacement, the project explores how enterprise workflow scheduling systems should be designed.

---

# Engineering Focus

The project explores:

- secure service communication
- workflow scheduling
- service discovery
- observability
- distributed architecture
- operational tooling

---

# Notable Design Decisions

- gRPC instead of REST
- Unix Domain Sockets for local communication
- mTLS between services
- OpenTelemetry throughout
- Prometheus metrics
- Grafana dashboards
- Jaeger tracing

Rather than viewing observability as something added after implementation, the project treats telemetry as part of the architecture itself.

---

# Technologies

- Go
- gRPC
- MySQL
- MongoDB
- Docker
- Kubernetes
- OpenTelemetry
- Prometheus
- Grafana
- Jaeger

---

# Why I Built It

Workflow Scheduler reflects my growing interest in platform engineering.

Rather than focusing on application features, the project investigates how engineering teams can build reliable infrastructure that other services depend upon.

Many architectural ideas explored here continue to influence how I think about distributed systems.