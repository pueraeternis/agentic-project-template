# METHODOLOGY.md

# Agentic Engineering Methodology

## Purpose

This document defines the core engineering principles for developing software projects with AI agents.

It is not tied to any specific tool, IDE, programming language, framework, or model.

The methodology is designed for projects where humans and AI agents collaborate through a shared repository.

---

## Core Idea

The repository is the shared working memory of humans and AI agents.

Chat history is temporary.

Agent memory is unreliable.

Human memory is incomplete.

The repository is the durable place where project knowledge, decisions, plans, architecture, implementation, and history must converge.

---

## What This Methodology Is Not

This methodology is not vibe coding.

It is not ad hoc prompting.

It is not unrestricted autonomous coding.

It is not a replacement for engineering judgment.

It is not a collection of tool-specific rules.

It is a structured approach for building software with AI agents while preserving clarity, control, traceability, and maintainability.

---

## Principle 1: Shared Understanding Precedes Implementation

Before code is written, the project must have a shared understanding of what is being built and why.

That understanding should be captured in repository artifacts.

Typical artifacts include:

* project definition;
* goals and non-goals;
* architecture;
* implementation plans;
* decision records;
* acceptance criteria.

Code should implement documented intent.

When intent is unclear, clarify it before implementation.

---

## Principle 2: The Repository Is Long-Term Memory

Important knowledge must live in the repository.

Do not rely on:

* chat history;
* private notes;
* IDE sessions;
* temporary agent context;
* memory of previous conversations.

If knowledge matters for future work, it should become a repository artifact.

Examples of repository artifacts:

* `AGENTS.md`;
* `PROJECT.md`;
* architecture documentation;
* decision records;
* implementation plans;
* completed plans;
* generated documentation;
* validation reports.

Knowledge outside the repository effectively does not exist for future agents.

---

## Principle 3: Documentation Drives Implementation

Documentation is not a follow-up task.

Documentation is part of the engineering process.

Implementation should follow documented project intent, architecture, decisions, and active plans.

When documentation and implementation disagree:

* update documentation if the implementation change is intentional;
* update implementation if documentation is authoritative.

Do not leave the repository in an inconsistent state.

---

## Principle 4: Plans Authorize Change

Significant implementation work should be authorized by an explicit plan.

A plan defines:

* objective;
* scope;
* acceptance criteria;
* implementation steps;
* risks;
* validation requirements.

Agents should not silently expand scope.

If new work is discovered during implementation, update the plan or create a new one.

The active plan defines the current implementation boundary.

---

## Principle 5: Humans Own Intent, Agents Execute Within Boundaries

Humans own:

* product direction;
* priorities;
* architectural trade-offs;
* scope decisions;
* final approval.

AI agents help with:

* exploration;
* analysis;
* implementation;
* refactoring;
* validation;
* documentation updates.

Agents should operate inside documented boundaries.

They may propose changes, but they should not silently redefine the project.

---

## Principle 6: AI Agents Are First-Class Contributors

Projects should be understandable not only to humans, but also to future AI agents.

This requires agent-legible structure:

* clear entry points;
* explicit documentation hierarchy;
* stable terminology;
* focused documents;
* documented architecture;
* documented decisions;
* small implementation plans;
* reproducible validation steps.

A future agent should be able to enter the repository, read the documented context, and perform useful work without relying on hidden conversation history.

---

## Principle 7: Small Iterations Preserve Quality

Prefer small, bounded increments.

A good iteration has:

* clear scope;
* limited architectural impact;
* explicit acceptance criteria;
* validation;
* documentation updates.

Small iterations are easier to:

* review;
* test;
* debug;
* revert;
* hand off to another agent.

Large speculative changes reduce control and increase the risk of incoherent code.

---

## Principle 8: Architecture Evolves Intentionally

Architecture should not change accidentally.

Any meaningful architectural change should be documented.

Architecture documentation should describe:

* components;
* responsibilities;
* boundaries;
* dependency flow;
* integration points;
* ownership rules.

Decision records should capture:

* context;
* decision;
* rationale;
* consequences;
* rejected alternatives when useful.

Architecture should be visible in documentation, not only in source code.

---

## Principle 9: Knowledge Must Mature

Repeated knowledge should move from temporary instructions into durable artifacts.

Typical maturation path:

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

A one-time instruction may stay in a prompt.

A repeated rule should become project knowledge and durable repository knowledge.

A repeated document structure should become a template.

A repeated workflow should become a skill.

A repeated scheduled or trigger-based workflow may become automation.

The system should learn from repeated work.

---

## Principle 10: Validation Is Part of the Work

Work is incomplete until it has been validated according to project standards.

Validation may include:

* tests;
* static analysis;
* type checking;
* formatting checks;
* manual review;
* documentation review;
* acceptance criteria verification.

Validation requirements are project-specific and should be documented in the repository.

Agents should not assume that code generation is the final step.

---

## Principle 11: Traceability Matters

Future contributors should be able to understand why the project looks the way it does.

Traceability means connecting:

* goals to requirements;
* requirements to architecture;
* architecture to decisions;
* decisions to plans;
* plans to implementation;
* implementation to validation.

Traceability reduces dependency on memory and makes future agent work safer.

---

## Principle 12: The Process Should Stay Tool-Agnostic

The methodology must not depend on a specific AI tool.

It should work with:

* Codex CLI;
* Cursor;
* Claude Code;
* other AI coding agents;
* human-only development.

Tool-specific configuration belongs in tool-specific files.

Core project knowledge belongs in repository documentation.

---

## Practical Workflow

A typical project follows this flow:

```text
Idea
↓
Discussion
↓
PROJECT.md
↓
ROADMAP.md
↓
ARCHITECTURE.md
↓
Implementation Plan
↓
Plan Review
↓
Implementation
↓
Validation
↓
Documentation Update
↓
Completed Plan
```

The exact document set may vary by project.

The key rule is that knowledge should become explicit before it becomes code.

---

## Definition of Done

Work is complete when:

* the requested scope has been implemented;
* acceptance criteria are satisfied;
* validation has been performed;
* documentation has been updated when needed;
* decisions have been recorded when needed;
* the repository remains internally consistent.

Code alone does not complete a task.

---

## Summary

Agentic engineering is disciplined software engineering adapted for AI-assisted development.

The goal is not to let agents code freely.

The goal is to create a repository where humans and AI agents can collaborate safely, incrementally, and predictably.

The repository is the shared working memory.

Documentation preserves intent.

Plans control change.

Architecture guides implementation.

Validation protects quality.

Agents execute within boundaries.
