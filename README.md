# Agentic Project Template

A reusable AI-first development framework for building software with AI agents.

The repository is the shared working memory where project intent, architecture, engineering decisions, implementation plans, and project history live together—not just source code.

---

# What This Is

This repository provides a **documentation-driven engineering framework** for human–AI collaboration.

It defines how projects move from an initial idea to production implementation through a structured lifecycle.

The framework separates:

* project design;
* repository initialization;
* implementation.

It is intentionally tool-agnostic and can be used with Cursor, Codex CLI, Claude Code, ChatGPT, or future AI development tools.

This repository is a **template**, not a finished application.

---

# Who This Is For

* Engineering leads designing AI-assisted development workflows
* Software architects who want traceable engineering decisions
* Developers starting new projects with AI assistance
* Teams using multiple AI coding tools
* Anyone who wants repository knowledge instead of chat-dependent development

---

# Core Philosophy

Chat history is temporary.

Agent memory is unreliable.

Human memory is incomplete.

**The repository is the permanent system of record.**

Documentation drives implementation.

Engineering decisions are documented before code exists.

Implementation follows approved plans.

Validation is part of the development process.

---

# Project Lifecycle

Projects built with this framework follow the lifecycle below.

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

---

# Repository Structure

```text
.
├── README.md
├── AGENTS.md
├── METHODOLOGY.md
├── KNOWLEDGE_MODEL.md
├── REPOSITORY_MAP.md
├── VERSION.md
│
├── docs/
│   ├── project/
│   │   ├── adr/
│   │   └── plans/
│   └── templates/
│
├── skills/
│
├── .agents/
│
├── .cursor/
│
└── .codex/
```

| Location          | Purpose                                |
| ----------------- | -------------------------------------- |
| Root documents    | Framework documentation                |
| `docs/templates/` | Templates used during project creation |
| `docs/project/`   | Project-specific documentation         |
| `skills/`         | Reusable engineering procedures        |
| `.agents/`        | Specialized AI agent definitions       |
| `.cursor/`        | Cursor configuration                   |
| `.codex/`         | Codex configuration                    |

---

# Repository Workflow

A typical project evolves as follows:

1. Define the project vision (`PROJECT.md`)
2. Create the delivery roadmap (`ROADMAP.md`)
3. Design the architecture (`ARCHITECTURE.md`)
4. Define engineering standards (`ENGINEERING.md`)
5. Initialize the repository
6. Create implementation plans
7. Implement incrementally
8. Review implementation
9. Record completed work

Architectural decisions are recorded as ADRs throughout the project.

---

# Getting Started

## Creating a New Project

1. Complete Project Discovery.
2. Create:

   * `PROJECT.md`
   * `ROADMAP.md`
   * `ARCHITECTURE.md`
   * `ENGINEERING.md`
3. Run Repository Initialization.
4. Create the first implementation plan.
5. Begin implementation.

---

## Joining an Existing Project

Read in the following order:

1. `AGENTS.md`
2. `REPOSITORY_MAP.md`
3. `METHODOLOGY.md`
4. `KNOWLEDGE_MODEL.md`
5. `docs/project/PROJECT.md`
6. `docs/project/ROADMAP.md`
7. `docs/project/ARCHITECTURE.md`
8. `docs/project/ENGINEERING.md`
9. Active implementation plans

---

## For AI Agents

Always begin with `AGENTS.md`.

Follow the documentation read order defined there before making repository changes.

---

# Framework Documentation

| Document             | Purpose                          |
| -------------------- | -------------------------------- |
| `AGENTS.md`          | Universal rules for AI agents    |
| `METHODOLOGY.md`     | Complete development methodology |
| `KNOWLEDGE_MODEL.md` | Repository knowledge model       |
| `REPOSITORY_MAP.md`  | Repository navigation            |
| `VERSION.md`         | Framework version history        |
