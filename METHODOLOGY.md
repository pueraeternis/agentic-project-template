# Agentic Engineering Methodology

## Purpose

This document defines the engineering methodology for developing software with AI agents.

The methodology is independent of any programming language, framework, IDE, or AI model.

It describes how humans and AI agents collaborate through a repository that serves as the project's long-term memory.

---

# Core Philosophy

The repository is the permanent system of record.

Chat history is temporary.

Agent memory is unreliable.

Human memory is incomplete.

Project intent, engineering decisions, architecture, implementation plans, and project history belong in the repository.

Documentation is not an output of development.

Documentation is part of development.

---

# Project Lifecycle

Projects evolve through the following stages.

```text
Idea
        ↓
Project Discovery
        ↓
PROJECT.md

Roadmap Creation
        ↓
ROADMAP.md

Architecture Design
        ↓
ARCHITECTURE.md

Engineering Design
        ↓
ENGINEERING.md

Repository Initialization
        ↓
Initialized Repository

Plan Creation
        ↓
PLAN.md

Plan Review
        ↓

Plan Implementation
        ↓

Code Review
```

Each stage produces durable repository knowledge before implementation continues.

---

# Lifecycle Stages

## Project Discovery

Define the project vision.

Produce:

* project goals;
* scope;
* non-goals;
* success criteria.

Artifact:

`PROJECT.md`

---

## Roadmap Creation

Define how the project will evolve.

Produce:

* implementation phases;
* milestones;
* dependencies.

Artifact:

`ROADMAP.md`

---

## Architecture Design

Design the system structure.

Produce:

* components;
* responsibilities;
* boundaries;
* dependency flow.

Artifact:

`ARCHITECTURE.md`

---

## Engineering Design

Define implementation conventions.

Produce:

* technology stack;
* engineering standards;
* repository organization;
* development workflow;
* validation strategy.

Artifact:

`ENGINEERING.md`

---

## Repository Initialization

Transform approved documentation into an initialized repository.

Produce:

* project documentation;
* project-local AI rules;
* repository metadata;
* initialized project structure.

No production code is created during this stage.

---

## Implementation Lifecycle

After initialization:

* create plans;
* review plans;
* implement incrementally;
* review implementation;
* repeat.

---

# Engineering Principles

## Documentation Before Code

Implementation follows documented intent.

Do not implement undocumented behavior.

---

## Repository as Long-Term Memory

Important knowledge belongs in the repository.

Do not rely on conversations.

---

## Plans Authorize Change

Implementation should follow approved plans.

Avoid expanding scope without updating documentation.

---

## Humans Own Intent

Humans define:

* goals;
* priorities;
* architecture;
* scope.

Agents execute within documented boundaries.

---

## Prefer Simplicity

Choose the simplest solution that satisfies the documented requirements.

Avoid unnecessary abstractions.

Avoid premature architecture.

Introduce complexity only when it solves a demonstrated problem.

---

## Small Iterations

Deliver work in small, reviewable increments.

Each iteration should:

* have a clear scope;
* update documentation when necessary;
* remain independently understandable.

---

## Architecture Evolves Intentionally

Architectural changes require documentation.

Architecture should never exist only in source code.

---

## Knowledge Matures

Repository knowledge evolves:

```text
Conversation
        ↓
Project Documentation
        ↓
Template
        ↓
Skill
        ↓
Automation
```

Repeated practices should become permanent repository knowledge.

---

## Validation Completes Work

Implementation is incomplete until validation has been performed.

Validation requirements belong to the project.

---

## Tool Independence

The methodology is independent of:

* Cursor;
* Codex CLI;
* Claude Code;
* ChatGPT;
* future AI development tools.

Tool-specific configuration belongs in tool-specific directories.

---

# Definition of Done

A lifecycle stage is complete when:

* required artifacts have been created;
* repository knowledge is consistent;
* documentation has been updated;
* validation requirements have been satisfied;
* no important knowledge exists only in conversation.

---

# Summary

Agentic Engineering is a documentation-driven and lifecycle-oriented software engineering methodology.

Humans define intent.

Documentation preserves intent.

Repositories preserve knowledge.

Plans authorize implementation.

Agents execute within documented boundaries.

Validation protects quality.

The repository remains the single source of truth throughout the entire project lifecycle.
