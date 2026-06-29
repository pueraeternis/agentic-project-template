# AGENTS.md

# AI Agent Guide

## Purpose

This document defines the universal rules for AI agents working with this repository.

It is intended for any AI coding assistant, including Codex CLI, Cursor, Claude Code, ChatGPT, and future agent-based development tools.

This document contains only repository-independent principles.

Project-specific knowledge belongs in the project documentation.

---

# Repository Philosophy

The repository is the permanent system of record.

Documentation defines:

* project intent;
* implementation strategy;
* architecture;
* engineering decisions;
* implementation plans.

Source code implements documented decisions.

Repository documentation always has higher priority than conversational context.

---

# Framework Overview

This repository provides an AI-first development framework based on a documentation-driven workflow.

The project lifecycle is:

```text
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

Additional framework documentation:

* `METHODOLOGY.md` — development methodology and lifecycle
* `KNOWLEDGE_MODEL.md` — repository knowledge model
* `REPOSITORY_MAP.md` — repository organization

---

# Read-First Order

Before performing work, read repository documentation in the following order when available:

1. `AGENTS.md`
2. `docs/project/PROJECT.md`
3. `docs/project/ROADMAP.md`
4. `docs/project/ARCHITECTURE.md`
5. `docs/project/ENGINEERING.md`
6. Relevant ADRs in `docs/project/adr/`
7. Active plans in `docs/project/plans/active/`
8. `docs/project/PROGRESS.md`

If a document does not exist, continue with the next available document.

For repository onboarding, see `REPOSITORY_MAP.md`.

---

# Documentation Precedence

When information conflicts, use the following priority:

1. `docs/project/PROJECT.md`
2. `docs/project/ROADMAP.md`
3. `docs/project/ARCHITECTURE.md`
4. `docs/project/ENGINEERING.md`
5. Relevant ADRs
6. Active plans
7. `docs/project/PROGRESS.md`
8. Chat context

Repository documentation always overrides conversational context.

---

# Working Principles

* Documentation is the primary source of truth.
* Chat history is temporary context.
* Implement only the requested scope.
* Keep the repository internally consistent.
* Prefer simple, maintainable solutions.
* Avoid unnecessary complexity.
* Do not invent undocumented project decisions.

---

# Development Workflow

For every task:

1. Read the relevant project documentation.
2. Determine the current lifecycle stage.
3. Perform only the responsibilities of that stage.
4. Update repository documentation when required.
5. Verify repository consistency before considering the task complete.

---

# Documentation Rules

Documentation evolves together with the project.

Update documentation whenever:

* project goals change;
* architecture changes;
* engineering decisions change;
* implementation workflow changes;
* repository structure changes;
* permanent project knowledge is introduced.

Do not allow important project knowledge to exist only in chat conversations.

---

# Modification Rules

Do not:

* introduce undocumented architectural changes;
* redesign approved project goals;
* modify unrelated parts of the repository;
* contradict approved documentation;
* perform destructive operations without explicit approval.

When requirements are ambiguous, ask for clarification instead of guessing.

---

# Completion Criteria

A task is complete when:

* the requested lifecycle stage has been completed;
* required repository artifacts have been created or updated;
* repository documentation is internally consistent;
* project-specific validation requirements have been satisfied;
* no permanent project knowledge exists only in conversational context.
