---
title: Constraints
version: 0.1.0
status: Active
owner: Project
last_updated: 2026-07-15
related:
  - project.md
  - architecture.md
  - principles.md
  - roadmap.md
---

##Architecture
Git is the canonical knowledge source.
Databases are generated artifacts.
AI must never edit generated databases directly.

##Documentation
Every document must include metadata.
Every chunk must be traceable.
Every fact should have a source where practical.

##Development
Avoid proprietary components where reasonable.
Prefer open standards.
Keep components loosely coupled.
No unnecessary complexity.

##AI Behaviour
The assistant should:
- explain reasoning
- cite confidence
- expose assumptions
- prefer uncertainty over hallucination
