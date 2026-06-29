# Plan NNN — <Short Title>

**File:** `NNN-short-title.md`

**Status:** Draft | Approved | In Progress | Completed | Superseded

**Created:** YYYY-MM-DD

**Approved:** YYYY-MM-DD (optional)

**Completed:** YYYY-MM-DD (optional)

---

# Purpose

This document authorizes one bounded implementation increment.

A plan defines:

* what will be implemented;
* why it is needed;
* what is intentionally excluded;
* how completion will be verified.

Implementation should never extend beyond the approved plan.

---

# Relationship to the Project Lifecycle

Implementation plans are created after the project design is complete.

Typical lifecycle:

```text
PROJECT
        ↓
ROADMAP
        ↓
ARCHITECTURE
        ↓
ENGINEERING
        ↓
PLAN
        ↓
IMPLEMENTATION
```

Plans translate long-term project design into small implementation increments.

---

# Objective

Describe the objective of this implementation increment.

Explain both:

* what will be delivered;
* why this work is needed now.

---

# Context

Describe the current project state.

Reference, when applicable:

* roadmap phase;
* architecture;
* engineering decisions;
* ADRs;
* previous implementation plans.

The context should explain why this is the logical next step.

---

# Scope

Describe exactly what belongs to this plan.

The implementation agent should never need to guess.

---

# Out of Scope

Explicitly list work that is excluded.

Typical examples:

* future improvements;
* unrelated refactoring;
* optimizations;
* additional features.

Clear boundaries prevent scope creep.

---

# Architectural Impact

Describe whether this implementation changes the architecture.

If applicable describe:

* affected components;
* dependency changes;
* integration changes;
* ownership changes.

Significant architectural changes should result in an ADR.

---

# Risks

Describe implementation risks.

Examples:

* compatibility;
* migration;
* performance;
* operational;
* validation.

If no meaningful risks exist, state so explicitly.

---

# Acceptance Criteria

Acceptance criteria should be:

* objective;
* measurable;
* testable.

Examples:

* required functionality implemented;
* tests pass;
* documentation updated;
* validation successful.

A reviewer should be able to determine whether the plan has been completed.

---

# Validation

Describe how completion will be verified.

Examples:

* unit tests;
* integration tests;
* manual verification;
* documentation review;
* performance validation.

---

# Implementation Checklist

* [ ] Task 1
* [ ] Task 2
* [ ] Task 3

The checklist tracks implementation progress.

It is not a brainstorming list.

---

# Related Documents

Typical references:

* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`
* `ENGINEERING.md`
* ADRs
* previous plans

---

# Completion Notes

Complete this section only after implementation.

Record:

* completed work;
* deviations from the plan;
* follow-up work.

Do not rewrite historical sections.

---

# Plan Lifecycle

## File Naming

Plans use:

```text
NNN-short-title.md
```

Examples:

```text
001-project-bootstrap.md
002-agent-routing.md
```

Plan numbers are sequential and never reused.

---

## Status Lifecycle

```text
Draft
        ↓
Approved
        ↓
In Progress
        ↓
Completed
        ↘
     Superseded
```

Only Approved and In Progress plans authorize implementation.

---

## Folder Lifecycle

```text
backlog
        ↓
active
        ↓
completed
```

Typical transitions:

1. Create in `backlog/` as Draft.
2. Review and approve.
3. Move to `active/`.
4. Implement.
5. Move to `completed/`.

---

# Repository Relationships

Planning uses:

* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`
* `ENGINEERING.md`

Implementation follows the plan.

Review verifies completion.

`PROGRESS.md` records delivered work.

---

# Planning Principles

A good implementation plan is:

* small;
* focused;
* independently reviewable;
* directly traceable to the roadmap;
* independently deliverable.

Prefer multiple small plans over one large implementation effort.

---

# Definition of Done

A plan is complete when:

* implementation is finished;
* acceptance criteria are satisfied;
* validation has passed;
* documentation has been updated when required;
* completion notes have been written;
* the plan has been moved to `completed/`.

Completed plans become part of the project's permanent engineering history.
