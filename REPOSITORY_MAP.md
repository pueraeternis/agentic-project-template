# REPOSITORY_MAP.md

# Repository Map

## Purpose

This document explains how knowledge is organized within the repository.

It serves as the primary navigation guide for both humans and AI agents.

When looking for information, start here.

---

# Repository Philosophy

The repository is organized around knowledge rather than code.

Each document has a single responsibility.

Knowledge should have one authoritative location.

Avoid duplicating information across documents.

---

# Repository Structure

```text
.
├── AGENTS.md
├── REPOSITORY_MAP.md
├── METHODOLOGY.md
├── KNOWLEDGE_MODEL.md
├── README.md
│
├── docs/
│   ├── project/
│   └── templates/
│
└── skills/
```

---

# Repository Entry Points

## README.md

Purpose:

Repository introduction.

Audience:

* humans

---

## AGENTS.md

Purpose:

Instructions for AI agents.

Defines:

* repository conventions;
* execution workflow;
* read-first order.

Audience:

* AI agents

---

## REPOSITORY_MAP.md

Purpose:

Repository navigation.

Explains where project knowledge lives.

Audience:

* humans;
* AI agents

---

## METHODOLOGY.md

Purpose:

Defines the engineering philosophy behind the repository.

Explains:

* development principles;
* engineering workflow;
* project lifecycle.

Audience:

* humans;
* AI agents

---

## KNOWLEDGE_MODEL.md

Purpose:

Defines how project knowledge is organized.

Explains:

* knowledge hierarchy;
* document responsibilities;
* relationships between project artifacts.

Audience:

* humans;
* AI agents

---

# Skills

Location:

```text
skills/
```

Purpose:

Reusable engineering procedures.

Each skill defines:

* purpose;
* role;
* inputs;
* outputs;
* execution procedure;
* completion criteria.

Current core skills:

* Project Discovery
* Roadmap Creation
* Architecture Design
* Plan Creation
* Plan Review
* Plan Implementation
* Code Review

Skills describe engineering processes.

They are reusable across projects.

---

# Project Documentation

Location:

```text
docs/project/
```

Purpose:

Contains all documentation specific to a single project.

Typical contents:

```text
PROJECT.md
ROADMAP.md
ARCHITECTURE.md
PROGRESS.md
adr/
plans/
```

Project documentation evolves throughout the project lifecycle.

---

## PROJECT.md

Defines:

* project vision;
* goals;
* scope;
* MVP;
* non-goals.

---

## ROADMAP.md

Defines:

* implementation phases;
* project evolution;
* delivery strategy.

---

## ARCHITECTURE.md

Defines:

* system architecture;
* component boundaries;
* dependency rules;
* architectural principles.

---

## PROGRESS.md

Records:

* completed implementation increments;
* engineering milestones;
* project history.

---

## adr/

Contains individual Architecture Decision Records (ADRs).

Each ADR documents:

* context;
* decision;
* rationale;
* consequences.

---

## plans/

Contains implementation plans that authorize and track implementation work.

Structure:

```text
plans/
├── backlog/
├── active/
└── completed/
```

### Naming Convention

Plan files use a sequential three-digit prefix and a short kebab-case title:

```text
NNN-short-title.md
```

Examples: `001-user-authentication.md`, `002-api-rate-limiting.md`.

See `docs/templates/PLAN.md` for the full plan template, status lifecycle, and folder transition rules.

### backlog/

Holds future implementation plans.

Plans here are **Draft** or not yet scheduled. They do not authorize implementation.

### active/

Holds approved work ready for or currently in implementation.

Only plans in this folder with status **Approved** or **In Progress** authorize implementation.

### completed/

Holds finished or superseded plans.

Plans here have status **Completed** or **Superseded**. They are preserved for traceability and must not authorize new implementation.

---

# Templates

Location:

```text
docs/templates/
```

Purpose:

Reusable document templates.

Templates are copied into `docs/project/` when initializing a new project.

Templates define document structure, not project content.

---

# Knowledge Flow

Knowledge evolves through the following lifecycle:

```text
Idea
    │
    ▼
PROJECT.md
    │
    ▼
ROADMAP.md
    │
    ▼
ARCHITECTURE.md
    │
    ▼
Implementation Plan
    │
    ▼
Plan Review
    │
    ▼
Implementation
    │
    ▼
PROGRESS.md
```

Significant architectural decisions are recorded as ADRs in `docs/project/adr/`.
Architecture may be updated when roadmap phases introduce new structural requirements.

---

# Read Order

When joining an existing project, read documents in the following order:

1. AGENTS.md
2. REPOSITORY_MAP.md
3. METHODOLOGY.md
4. KNOWLEDGE_MODEL.md
5. `docs/project/PROJECT.md`
6. `docs/project/ROADMAP.md`
7. `docs/project/ARCHITECTURE.md`
8. Active plans in `docs/project/plans/active/`
9. Relevant ADRs in `docs/project/adr/`
10. `docs/project/PROGRESS.md`

---

# Design Principles

The repository is organized around the following principles:

* one document, one responsibility;
* knowledge has a single source of truth;
* documentation drives implementation;
* implementation follows approved plans;
* architecture evolves intentionally;
* project history is preserved.

The repository should remain understandable to both humans and AI agents, regardless of project size.
