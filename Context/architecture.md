---
title: Architectural Decisions
version: 0.1.0
status: Active
owner: Project
last_updated: 2026-07-15
related:
  - project.md
  - constraints.md
  - principles.md
  - roadmap.md
---

These are the architectural decisions we've made.

## AI
LLM abstraction layer.
Local models preferred.
Ollama selected as initial inference platform.
Future cloud providers supported.


## Knowledge Storage
Structured documents stored in Git.

Reason:
- version control
- review
- branching
- traceability

Git is the source of truth.

## Retrieval
Multiple storage engines.

Current architecture

Git
 │
 ▼
Document pipeline
 │
 ├── PostgreSQL
 ├── Qdrant
 └── Neo4j

Each database serves a different purpose.

PostgreSQL
Structured metadata

Examples:
- games
- cars
- manufacturers
- versions

Qdrant
Semantic search

Stores:
- embeddings
- chunks
- semantic similarity

Neo4j
Relationship graph

Stores
- manufacturer relationships
- shared engines
- platform lineage
- tuning dependencies
- knowledge graph

## Workflow
Markdown
↓
Validation
↓
Metadata extraction
↓
Chunking
↓
Embedding
↓
Database ingestion

Git remains authoritative.

Generated databases are disposable.
