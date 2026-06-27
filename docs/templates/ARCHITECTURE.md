# ARCHITECTURE.md

# Architecture

## Purpose

This document describes the long-term architecture of the project.

It defines the major system components, their responsibilities, architectural boundaries, dependency rules, and interactions.

This document describes **how the system is organized**, not **how individual features are implemented**.

Implementation details belong in implementation plans.

---

# Overview

Provide a short description of the overall system.

Describe:

* the architectural style;
* the primary purpose of the system;
* the major building blocks;
* important design constraints.

---

# Architecture Goals

Describe the qualities the architecture should provide.

Examples:

* simplicity;
* maintainability;
* scalability;
* observability;
* extensibility;
* reliability;
* security;
* deterministic behavior.

Only include goals that are relevant to the project.

---

# High-Level Architecture

Provide a high-level diagram of the system.

Example:

```text
User
    │
    ▼
Client
    │
    ▼
Application
    │
    ├────────────► External Service A
    ├────────────► External Service B
    └────────────► Storage
```

The diagram should help readers understand the overall system structure in a few seconds.

---

# Core Components

Describe every major architectural component.

Each component should include:

## Component Name

### Purpose

What the component is responsible for.

### Responsibilities

Examples:

* orchestration;
* business logic;
* persistence;
* communication;
* validation.

### Inputs

What the component receives.

### Outputs

What the component produces.

### Dependencies

Which components it is allowed to communicate with.

### Constraints

What the component must **not** do.

Clearly defining constraints is often more important than listing responsibilities.

Repeat this structure for every major component.

---

# External Systems

Describe external dependencies.

Examples:

* databases;
* APIs;
* LLM providers;
* MCP servers;
* message brokers;
* object storage;
* authentication providers.

For each external system describe:

* purpose;
* interaction model;
* ownership boundary.

---

# Data Flow

Describe how data moves through the system.

Focus on:

* primary execution paths;
* state transitions;
* data ownership;
* validation points.

Avoid implementation details.

---

# Control Flow

Describe how execution flows through the system.

Examples:

* request processing;
* workflow execution;
* asynchronous processing;
* approval workflows;
* background execution.

The objective is to explain how work moves through the architecture.

---

# Source Layout

Describe the intended repository structure.

Example:

```text
src/
├── application/
├── domain/
├── infrastructure/
├── interfaces/
└── shared/
```

Briefly explain the responsibility of each major directory.

Avoid documenting every file.

---

# Dependency Rules

Document allowed dependency directions.

Example:

```text
Presentation
        ↓
Application
        ↓
Domain
        ↓
Infrastructure
```

Also document prohibited dependencies.

Examples:

```text
Infrastructure → Presentation
Domain → Infrastructure
Adapters → Business Logic
```

Clear dependency rules prevent architectural erosion.

---

# Validation and Safety

Describe architectural validation points.

Examples:

* approval workflows;
* validation before execution;
* permission checks;
* policy enforcement;
* safety boundaries.

Identify which operations require explicit validation before execution.

---

# Observability

Describe how the system should be observed.

Examples:

* logs;
* metrics;
* traces;
* execution history;
* audit events.

Include only long-term observability requirements.

Implementation details belong elsewhere.

---

# Architectural Principles

Document the architectural principles that guide the project.

Examples:

* simplicity over unnecessary complexity;
* explicit boundaries;
* composition over coupling;
* deterministic workflows before autonomous workflows;
* validation before execution;
* documentation as the system of record.

These principles should remain stable throughout the project.

---

# Deferred Decisions

Document architectural questions that are intentionally postponed.

For each deferred decision include:

* the topic;
* why it is deferred;
* when it should be revisited.

Avoid solving problems before they become relevant.

---

# Change Management

Update this document whenever:

* major components are added or removed;
* architectural boundaries change;
* dependency rules change;
* integration patterns change;
* core system responsibilities change.

Do not update this document for ordinary implementation changes.

Those belong in implementation plans.

---

# Relationship to Other Documents

This document should be read together with:

* `PROJECT.md` — defines what is being built.
* `ROADMAP.md` — defines the implementation strategy.
* Implementation plans — define individual implementation increments.
* Decision records — explain why significant architectural decisions were made.

Together these documents provide a complete understanding of the system.

---

# Summary

The purpose of this document is to describe the stable architecture of the project.

It should answer questions such as:

* How is the system organized?
* What are the major components?
* Where are the architectural boundaries?
* How do components interact?
* What architectural rules must always be respected?

The document should remain stable and evolve only when the architecture itself evolves.
