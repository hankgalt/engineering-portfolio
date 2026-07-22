# Embeddings

**Repository:** [github.com/hankgalt/embeddings](https://github.com/hankgalt/embeddings)

---

# Context

As large language models and semantic search became increasingly important, I wanted to better understand how modern embedding systems operate beneath the API layer.

Rather than relying exclusively on hosted AI services, I explored how high-quality sentence embeddings could be generated locally using ONNX Runtime and open-source transformer models.

This project was created both as a learning exercise and as a reusable library for applications requiring semantic understanding without depending on external APIs.

---

# Executive Summary

Embeddings is a Go library for generating sentence embeddings locally using ONNX Runtime.

The library supports multiple transformer models while exposing a consistent API for downstream applications.

Its primary goal is to make semantic search and vector-based applications easier to build in Go.

---

# Engineering Focus

The project explores several areas of modern AI infrastructure:

- ONNX Runtime integration
- Transformer inference
- Tokenization
- Mean pooling
- Model abstraction
- Efficient embedding generation

By separating model-specific implementation details from the public API, the library provides a consistent interface while remaining flexible enough to support multiple embedding models.

---

# Notable Design Decisions

- Local inference instead of cloud dependency
- Support for multiple transformer architectures
- Shared embedding interface across models
- Efficient pooling implementation
- Minimal external dependencies

These decisions allow applications to experiment with different embedding models without requiring significant code changes.

---

# Technologies

- Go
- ONNX Runtime
- Hugging Face Tokenizers
- Transformer Models
- Vector Embeddings

---

# Why I Built It

This project reflects my curiosity about the engineering foundations of modern AI systems.

Rather than treating embeddings as a black-box API, I wanted to understand how transformer models are executed, how embeddings are generated, and how semantic search systems can be built using open-source tooling.

It also aligns with a broader engineering principle that has guided much of my work: understanding the underlying mechanisms of a technology leads to better architectural decisions when incorporating it into larger systems.