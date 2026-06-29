# Architecture

## Purpose

This document defines the long-term architecture of the project.

It describes:

* system structure;
* major components;
* responsibilities;
* dependency rules;
* integration boundaries;
* architectural constraints.

It does **not** describe implementation details or engineering conventions.

Technology choices belong in `ENGINEERING.md`.

Implementation details belong in implementation plans.

---

# Architecture Overview

Provide a concise description of the overall system.

Describe:

* the architectural style;
* the primary responsibilities of the system;
* major architectural building blocks;
* important architectural constraints.

This section should explain the system in a few paragraphs.

---

# Architecture Goals

Describe the qualities the architecture should provide.

Examples:

* simplicity;
* maintainability;
* scalability;
* observability;
* reliability;
* security;
* extensibility;
* deterministic behavior.

Only include goals that matter for this project.

---

# High-Level Architecture

Provide a simple diagram.

Example:

```text id="7l8n2m"
User
        ↓
Application
        ↓
API
        ↓
Core Services
        ↓
Storage
```

The diagram should communicate the overall structure in seconds.

---

# Core Components

Document each major component.

For every component include:

## Component

### Purpose

### Responsibilities

### Inputs

### Outputs

### Dependencies

### Constraints

Constraints are often more important than responsibilities.

Repeat for every architectural component.

---

# Integration Boundaries

Describe communication with external systems.

Typical examples:

* databases;
* LLM providers;
* external APIs;
* MCP servers;
* message brokers;
* authentication systems.

For each integration describe:

* ownership;
* communication model;
* trust boundary.

---

# Data Flow

Describe how data moves through the system.

Focus on:

* ownership;
* major execution paths;
* state transitions;
* validation boundaries.

Avoid implementation details.

---

# Control Flow

Describe how work moves through the architecture.

Examples:

* request processing;
* workflow execution;
* asynchronous processing;
* approval workflows;
* background execution.

Explain responsibilities rather than implementation.

---

# Dependency Rules

Document allowed dependency directions.

Example:

```text id="qej0co"
Presentation
        ↓
Application
        ↓
Domain
        ↓
Infrastructure
```

Document prohibited dependencies as well.

Examples:

```text id="c6rk4v"
Infrastructure → Presentation
Domain → Infrastructure
```

Architectural boundaries should remain explicit.

---

# Architectural Constraints

Document rules that must always be respected.

Examples:

* ownership boundaries;
* communication rules;
* dependency restrictions;
* state ownership;
* security boundaries.

These constraints should remain stable throughout the project.

---

# Deferred Decisions

List architectural topics intentionally postponed.

For each topic describe:

* what is deferred;
* why;
* when it should be revisited.

Avoid solving speculative problems.

---

# Architecture Evolution

Update this document only when the architecture changes.

Examples:

* components added or removed;
* dependency rules changed;
* ownership boundaries changed;
* integration patterns changed.

Do not update this document for ordinary implementation work.

---

# Repository Relationships

This document should be read together with:

| Document         | Purpose                                       |
| ---------------- | --------------------------------------------- |
| `PROJECT.md`     | Defines project goals                         |
| `ROADMAP.md`     | Defines project evolution                     |
| `ENGINEERING.md` | Defines implementation conventions            |
| ADRs             | Explain why architectural decisions were made |
| Plans            | Implement architectural changes               |

Together these documents describe both the architecture and its evolution.

---

# Summary

This document describes the stable architecture of the project.

It should answer questions such as:

* How is the system organized?
* What are the major components?
* Where are the architectural boundaries?
* How do components interact?
* Which architectural rules must always be respected?

The document should evolve only when the architecture itself evolves.
