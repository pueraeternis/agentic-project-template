# AGENTS.md

# AI Agent Guide

## Purpose

This document defines the universal rules for AI agents working with this repository.

It is intended for any AI coding assistant, including Codex CLI, Cursor, Claude Code, and future agent-based development tools.

This document contains only repository-independent development principles.

Project-specific requirements belong in the project documentation.

---

# Core Principles

* Documentation is the primary source of truth.
* Chat history is temporary context and must not be treated as persistent knowledge.
* Repository documentation has higher priority than conversational context.
* Keep the repository internally consistent.
* Implement only the requested scope.
* Prefer simple, maintainable solutions over unnecessary complexity.

---

# Read-First Order

Before making implementation changes, read the repository documentation in the following order when available:

1. AGENTS.md
2. `docs/project/PROJECT.md`
3. `docs/project/ARCHITECTURE.md`
4. Relevant ADRs in `docs/project/adr/`
5. Active plans in `docs/project/plans/active/`
6. `docs/project/PROGRESS.md`

If a document does not exist, continue with the next available document.

This is the implementation read order. For repository onboarding, see the read order in `REPOSITORY_MAP.md`.

---

# Documentation Precedence

When information conflicts, use the following priority:

1. `docs/project/PROJECT.md`
2. `docs/project/ARCHITECTURE.md`
3. Relevant ADRs in `docs/project/adr/`
4. Active plans in `docs/project/plans/active/`
5. `docs/project/PROGRESS.md`
6. Chat context

Repository documentation always overrides conversational context.

---

# Development Workflow

For every implementation task:

1. Understand the project documentation.
2. Identify the requested scope.
3. Implement only the required changes.
4. Update documentation if the repository knowledge has changed.
5. Verify that the repository remains consistent.

---

# Documentation Rules

Documentation should evolve together with the project.

Update documentation whenever:

* architecture changes;
* design decisions change;
* implementation workflow changes;
* repository structure changes;
* new permanent project knowledge appears.

Do not store permanent project knowledge only in chat conversations.

---

# Modification Rules

Do not:

* introduce undocumented architectural changes;
* modify unrelated parts of the project;
* make assumptions that contradict repository documentation;
* perform destructive operations without explicit user approval.

When requirements are ambiguous, ask for clarification instead of guessing.

---

# Completion Criteria

A task is complete when:

* the requested scope has been implemented;
* documentation has been updated if necessary;
* the repository remains internally consistent;
* all project-specific validation requirements have been satisfied.
