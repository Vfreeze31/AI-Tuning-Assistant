---
title: Decisions Register
version: 0.1.0
status: Active
owner: Project
last_updated: 2026-07-15
related:
  - project.md
  - architecture.md
  - constraints.md
  - principles.md
  - roadmap.md
---

# ADR-001
## Decision
Git is the source of truth.

## Reason
human readable
version control
branching
collaboration
AI friendly

## Alternatives
PostgreSQL
Neo4j
Notion

## Outcome
*Accepted

# ADR-002
## Decision
Use multiple databases.

## Reason
No single database excels at:
- semantic search
- graph traversal
- structured querying

## Outcome
Accepted

# ADR-003
## Decision
Target casual users first.

## Reason
Largest audience.
Simpler UX.
Allows expert mode later.

# ADR-004
## Decision
Game knowledge and tuning theory remain separate.

## Reason
Vehicle dynamics rarely change.
Games do.

# ADR-005
## Decision
Support multiple LLMs.

## Reason
Prevent vendor lock-in.

# ADR-006
## Decision
Open-source first.

## Reason
Long-term maintainability.

Self-hosting.

Community ecosystem.
