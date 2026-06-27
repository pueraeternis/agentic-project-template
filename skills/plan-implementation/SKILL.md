# SKILL.md

# Plan Implementation

## Purpose

This skill implements an approved implementation plan.

Implementation is the execution of an approved engineering contract.

The implementation agent realizes documented project intent rather than making design decisions.

The implementation agent translates the approved engineering plan into production-ready code while preserving architecture and repository consistency.

The implementation should satisfy the acceptance criteria without introducing unrelated changes.

---

## Role

Implementation Agent

---

## When to Use

Use this skill when:

- an implementation plan has been approved;
- all required project documentation is available;
- implementation is authorized.

Do not use this skill before the implementation plan has been reviewed and approved.

---

## Inputs

The skill requires:

- the approved implementation plan — the authoritative engineering contract;
- `PROJECT.md` — project intent, Background, Core Idea, and MVP;
- `ROADMAP.md` — current delivery strategy and implementation priorities;
- `ARCHITECTURE.md` — component boundaries and dependency rules;
- relevant ADRs — architectural decisions that must be respected;
- the current repository state — the current implementation baseline.

---

## Outputs

The skill produces:

- production-ready implementation;
- tests where appropriate;
- documentation updates when required;
- completed implementation checklist;
- implementation ready for code review.

---

## Procedure

### Step 1 — Understand the Engineering Contract

Read the implementation plan completely.

Explicitly verify:

- objective;
- scope;
- acceptance criteria;
- implementation constraints;
- validation requirements;
- architectural assumptions.

Implementation must not begin until the approved contract is fully understood.

---

### Step 2 — Review Project Knowledge

Review the repository documentation necessary for the current work.

Explicitly review:

- `PROJECT.md`;
- `ROADMAP.md`;
- `ARCHITECTURE.md`;
- relevant ADRs;
- current repository state.

The objective is to understand why the implementation exists before changing code.

Understand:

- existing architecture;
- component ownership;
- previous implementation decisions;
- coding conventions.

Avoid making assumptions.

---

### Step 3 — Implement the Approved Scope

Implement only the approved scope.

Before implementing a significant change, verify that it can be traced to:

- the approved implementation plan;
- the documented architecture;
- an accepted ADR (when applicable).

Do not introduce undocumented functionality.

Respect:

- architectural boundaries;
- component ownership;
- project conventions.

Keep the implementation as simple as possible.

---

### Step 4 — Validate the Implementation

Verify that:

- acceptance criteria are satisfied;
- tests pass;
- validation requirements are met;
- no regressions have been introduced.

Resolve issues before considering the implementation complete.

---

### Step 5 — Update Documentation

Update project documentation whenever implementation changes repository knowledge.

Examples include:

- architecture changes;
- ADR implementation;
- completed checklist;
- generated documentation.

Documentation should remain synchronized with implementation.

Documentation updates should be part of the same change.

---

### Step 6 — Prepare for Review

Before handing the work to the Review Agent, verify:

- implementation is complete;
- validation has been performed;
- documentation is consistent;
- no unrelated changes remain;
- implementation remains within approved scope;
- repository documentation is internally consistent;
- no undocumented architectural changes have been introduced.

The implementation should be ready for review without additional cleanup.

---

## Rules

Implement only the approved plan.

Do not:

- expand project scope;
- redesign the architecture;
- introduce unrelated refactoring;
- implement future roadmap phases;
- silently change requirements.

If additional work is discovered:

- stop implementation;
- document the finding;
- recommend creating or updating a plan.

Do not continue outside the approved scope.

---

## Implementation Principles

Prefer:

- simple solutions;
- explicit logic;
- maintainable code;
- small commits;
- minimal complexity;
- implement documented intent before introducing optimization;
- preserve engineering traceability;
- prefer explicit implementation over implicit behavior.

Avoid:

- speculative engineering;
- premature optimization;
- unnecessary abstractions;
- hidden behavior;
- scope creep.

The simplest correct implementation is usually the best implementation.

---

## Success Criteria

The skill is complete when:

- the approved scope has been fully implemented;
- acceptance criteria are satisfied;
- validation has been completed;
- documentation has been updated when necessary;
- the implementation is ready for independent review.

---

## Next Skill

After implementation is complete, continue with:

**Code Review**
