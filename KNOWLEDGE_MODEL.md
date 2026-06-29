# Knowledge Model

## Purpose

This document defines the conceptual model of repository knowledge.

It explains how knowledge is organized, how it evolves throughout a project, and how humans and AI agents use the repository as a shared engineering workspace.

The repository stores engineering knowledge, not merely source code.

---

# Core Concept

The repository is the permanent engineering memory of the project.

It contains:

* project intent;
* implementation strategy;
* architecture;
* engineering decisions;
* implementation plans;
* project history.

Knowledge should be explicit, discoverable, and independent of temporary conversations.

---

# Knowledge Layers

Repository knowledge is organized into layers.

Higher layers change less frequently and guide lower layers.

---

## Layer 1 — Methodology

Purpose:

Define the engineering methodology.

Typical artifacts:

* `METHODOLOGY.md`

Answers:

* How do projects evolve?
* What engineering principles guide development?

Changes:

Very rarely.

---

## Layer 2 — Framework Rules

Purpose:

Define repository-wide rules.

Typical artifacts:

* `AGENTS.md`

Answers:

* How should humans and AI agents work with the repository?
* Which documents define project intent?

Changes:

Rarely.

---

## Layer 3 — Skills

Purpose:

Define reusable engineering workflows.

Typical skills include:

* Project Discovery
* Roadmap Creation
* Architecture Design
* Engineering Design
* Repository Initialization
* Plan Creation
* Plan Review
* Plan Implementation
* Code Review

Answers:

* How is a lifecycle stage performed?
* What are its inputs and outputs?

Changes:

Occasionally.

---

## Layer 4 — Templates

Purpose:

Define reusable document structures.

Typical templates:

* PROJECT
* ROADMAP
* ARCHITECTURE
* ENGINEERING
* PLAN
* ADR
* RUNBOOK
* PROGRESS

Templates define document structure rather than project knowledge.

---

## Layer 5 — Project Design

Purpose:

Describe what is being built.

Artifacts:

* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`
* `ENGINEERING.md`

These documents are produced before implementation begins.

They define the project.

---

## Layer 6 — Project Execution

Purpose:

Capture implementation work.

Artifacts:

* implementation plans;
* completed plans;
* ADRs;
* progress logs;
* review artifacts.

These documents evolve throughout development.

---

## Layer 7 — Generated Knowledge

Purpose:

Store reproducible generated artifacts.

Examples:

* API documentation;
* inventories;
* generated reports;
* generated reference documentation.

Generated artifacts should never become the primary source of truth.

They should always be reproducible.

---

# Knowledge Lifetime

Different repository knowledge has different expected lifetimes.

## Permanent Knowledge

Examples:

* methodology;
* framework rules;
* reusable skills.

Changes very rarely.

---

## Project Design Knowledge

Examples:

* project vision;
* roadmap;
* architecture;
* engineering decisions.

Changes occasionally.

---

## Operational Knowledge

Examples:

* implementation plans;
* ADRs;
* progress records.

Changes frequently.

---

## Generated Knowledge

Examples:

* inventories;
* generated documentation;
* reports.

Always reproducible.

---

## Ephemeral Knowledge

Examples:

* conversations;
* brainstorming;
* temporary prompts;
* exploratory notes.

Ephemeral knowledge should never become the only place where important information exists.

---

# Knowledge Evolution

Knowledge matures over time.

```text id="iqnpur"
Conversation
        ↓
Project Documentation
        ↓
Framework Template
        ↓
Skill
        ↓
Automation
```

Repeated knowledge should become increasingly reusable.

---

# Knowledge Flow

Project knowledge follows the lifecycle.

```text id="8mv83n"
PROJECT
        ↓
ROADMAP
        ↓
ARCHITECTURE
        ↓
ENGINEERING
        ↓
Repository Initialization
        ↓
Implementation Plans
        ↓
Implementation
        ↓
Progress
```

Each stage consumes knowledge from the previous stage and produces knowledge for the next.

---

# Source of Truth

Repository documentation is authoritative.

When conflicts exist:

Repository documentation overrides conversations.

Project documentation overrides assumptions.

Implementation should remain consistent with documented project knowledge.

---

# Repository Quality

A high-quality repository is:

* understandable by humans;
* understandable by AI agents;
* internally consistent;
* lifecycle-oriented;
* documentation-driven;
* easy to navigate;
* resilient to changes in tools and technologies.

---

# Summary

The repository is the long-term engineering memory of the project.

Knowledge evolves from conversation into durable documentation.

Documentation defines the project.

Plans authorize implementation.

Implementation produces new repository knowledge.

The repository remains the single source of truth throughout the entire project lifecycle.
