---
title: Project Context
version: 0.1.0
status: Active
owner: Project
last_updated: 2026-07-15
related:
  - architecture.md
  - constraints.md
  - principles.md
  - roadmap.md
---

# Project Context

## Purpose

This document defines the vision, objectives and scope of the AI Car Tuning Assistant project. It serves as the canonical description of the project and should be consulted before making architectural or design decisions.

## Vision
Build an open knowledge platform for racing game vehicle tuning.
Support multiple racing games rather than being tied to one franchise.
Initial focus:
- Forza Horizon
- Forza Motorsport
- Assetto Corsa Evo
Future expansion to additional simulation and arcade racing games.
AI should assist beginners through experts.
Casual gamer experience is the primary design target.
Expert tuning mode may be added later as an optional capability.
Local-first architecture.
Open-source wherever practical.
Modular components to allow replacement without redesign.

## Goals
Explain tuning decisions rather than only giving values.
Build reusable automotive knowledge.
Separate game-specific knowledge from vehicle dynamics.
Support RAG over structured documentation.
Preserve references back to original sources.
Minimise hallucination.
Allow offline operation.
Scale from single user to community contributions.

## Non-goals
Cloud-first SaaS.
Closed proprietary knowledge.
Vendor lock-in.
Hardcoding game logic into prompts.
Dependence on a single LLM.
