# KNOWLEDGE_MODEL.md

# Knowledge Model

## Purpose

This document defines the conceptual model of repository knowledge.

It explains how project knowledge is organized, why different types of documents exist, and how humans and AI agents should use the repository as a shared engineering workspace.

This document describes the structure of repository knowledge rather than project implementation.

---

# Core Concept

The repository is the shared working memory of humans and AI agents.

It is not merely a source code repository.

It is the place where project intent, architecture, implementation, decisions, plans, and historical context converge into a durable and discoverable system.

The repository should remain understandable without relying on:

- chat history;
- private notes;
- temporary IDE sessions;
- individual human memory;
- individual agent memory.

---

# Repository Layers

The repository is organized into several conceptual layers.

Each layer has a different purpose and evolves at a different pace.

---

## Layer 1 — Methodology

Purpose:

Define the engineering philosophy.

Typical artifacts:

- METHODOLOGY.md

Answers:

- What principles guide development?
- What do we believe?
- How should humans and AI agents collaborate?

Changes:

Very rarely.

---

## Layer 2 — Agent Rules

Purpose:

Define universal rules for AI agents working with the repository.

Typical artifacts:

- AGENTS.md

Answers:

- How should an agent approach the repository?
- Which documents should be read first?
- What execution rules should be followed?

Changes:

Rarely.

---

## Layer 3 — Skills

Purpose:

Provide reusable engineering workflows.

Typical artifacts include skills for:

- Project Discovery;
- Roadmap Creation;
- Architecture Design;
- Plan Creation;
- Plan Review;
- Plan Implementation;
- Code Review.

Answers:

- How is a specific engineering workflow executed?
- What inputs, outputs, and completion criteria apply?

Changes:

Occasionally.

---

## Layer 4 — Templates

Purpose:

Provide reusable document structures.

Typical artifacts include templates for:

- project definition;
- roadmap;
- architecture;
- implementation plans;
- decision records.

Templates define document structure rather than project knowledge.

Changes:

Occasionally.

---

## Layer 5 — Project Knowledge

Purpose:

Describe the actual project.

Typical artifacts may include:

- project definition;
- roadmap;
- architecture;
- decision records;
- operational procedures.

Answers:

- What is being built?
- Why is it being built?
- How is the system organized?

Changes:

Throughout the lifetime of the project.

---

## Layer 6 — Implementation

Purpose:

Capture work in progress.

Typical artifacts include:

- implementation plans;
- validation reports;
- review artifacts;
- implementation history.

Answers:

- What is currently being implemented?
- What has already been completed?

Changes:

Frequently.

Implementation plans authorize work after roadmap and architecture are defined in Layer 5.

---

## Layer 7 — Generated Knowledge

Purpose:

Store reproducible machine-generated artifacts.

Examples include:

- API inventories;
- schema documentation;
- generated reports;
- generated reference documentation.

Generated artifacts should not be edited manually.

They should be regenerated from their source.

---

# Knowledge Lifetime

Different knowledge has different expected lifetimes.

---

## Permanent Knowledge

Changes very rarely.

Examples:

- methodology;
- engineering principles;
- agent rules.

---

## Project Knowledge

Exists throughout the project.

Examples:

- project vision;
- goals;
- roadmap.

---

## Architectural Knowledge

Changes occasionally.

Examples:

- architecture;
- decision records;
- component responsibilities.

---

## Operational Knowledge

Changes frequently.

Examples:

- implementation plans;
- validation reports;
- review notes.

---

## Generated Knowledge

Can always be regenerated.

Examples:

- API documentation;
- schema inventories;
- generated reports.

---

## Ephemeral Knowledge

Exists only temporarily.

Examples:

- conversations;
- prompts;
- brainstorming sessions;
- temporary notes.

Ephemeral knowledge should not be relied upon for future development.

If it becomes important, it should be promoted into repository documentation.

---

# Repository Knowledge Flow

Knowledge should mature over time.

Typical progression:

```text
Conversation
        ↓
Decision
        ↓
Project Knowledge
        ↓
Template
        ↓
Skill
        ↓
Automation
```

Repeated work should become increasingly structured.

Project knowledge should mature into durable repository knowledge.

---

# Source of Truth

Repository artifacts are the authoritative source of project knowledge.

When conflicts exist, repository documentation has priority over conversational context.

Important project knowledge should never exist exclusively in conversations.

---

# What Does Not Belong in Repository Memory

Not every conversation should become documentation.

Avoid documenting:

- temporary brainstorming;
- speculative ideas;
- abandoned approaches;
- one-time implementation details;
- transient debugging notes.

Documentation should preserve durable knowledge rather than transient thinking.

---

# Evolution of the Repository

The repository should evolve intentionally.

New document types should be introduced only when they represent recurring and reusable knowledge.

Avoid creating documents for isolated situations.

A document should exist because it improves clarity, discoverability, or long-term maintainability.

---

# Repository Quality

A high-quality repository is:

- understandable by humans;
- understandable by AI agents;
- internally consistent;
- easy to navigate;
- explicit rather than implicit;
- resilient to changes in tools and technologies.

The repository should remain useful even as programming languages, frameworks, IDEs, and AI coding assistants evolve.

---

# Summary

The repository is more than a codebase.

It is the durable engineering memory of the project.

Source code is only one part of that memory.

Documentation, decisions, plans, generated artifacts, and engineering principles collectively define the project and enable effective collaboration between humans and AI agents over time.