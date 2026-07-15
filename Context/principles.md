---
title: Principles
version: 0.1.0
status: Active
owner: Project
last_updated: 2026-07-15
related:
  - project.md
  - architecture.md
  - constraints.md
  - principles.md
  - decisions.md
  - roadmap.md
  - glossary.md
---

# Project Principles
Explain before recommending. Every tuning recommendation should include the reasoning behind it.
Separate theory from implementation. Vehicle dynamics are documented independently from game-specific behavior.
Preserve provenance. Every important fact should be traceable to its source or clearly marked as experiential knowledge.
Treat Git as the canonical knowledge base. Databases, embeddings, and indexes are generated artifacts that can be rebuilt at any time.
Design for modularity. Components such as the LLM, vector database, graph database, or workflow engine should be replaceable with minimal impact on the rest of the system.
Optimise for the casual user first. Interfaces and explanations should be approachable by default, with advanced or expert functionality layered on rather than replacing the beginner experience.
Prefer open standards and open-source software. Choose proprietary solutions only when they offer a compelling, well-documented advantage.
Make decisions explicit. Record architectural and design decisions, including rejected alternatives and the reasoning behind the choice.
Favour deterministic pipelines. Knowledge ingestion, validation, metadata extraction, and indexing should be automated and reproducible.
Accept uncertainty. When evidence is incomplete or conflicting, the system should communicate confidence levels instead of presenting speculation as fact.

# Trusted references worth aligning with
Rather than building the context file from one article, I'd anchor it to established practices that have stood the test of time:
- Architecture Decision Records (ADRs), especially Michael Nygard's ADR format. This provides a lightweight, industry-standard way to document technical decisions and their rationale.
- The Twelve-Factor App principles, where applicable, for configuration management, portability, and separation of concerns.
- Diátaxis Documentation Framework, which separates tutorials, how-to guides, explanations, and reference material. This maps particularly well to an AI knowledge base because it distinguishes conceptual knowledge from procedural instructions.
- Knowledge Graph concepts for modelling relationships between vehicles, platforms, engines, tuning principles, and game implementations.
- Retrieval-Augmented Generation (RAG) best practices, particularly maintaining a clear separation between the canonical source documents and derived indexes such as vector databases or graph databases.
