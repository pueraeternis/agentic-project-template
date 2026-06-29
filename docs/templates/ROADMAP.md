# Roadmap

## Purpose

This document defines the long-term evolution of the project.

It translates the project vision into a sequence of implementation phases.

The roadmap answers the question:

> **How will the project evolve over time?**

The roadmap describes capabilities rather than implementation tasks.

Implementation details belong in implementation plans.

---

# Relationship to the Project Lifecycle

The roadmap is created after `PROJECT.md` and before architectural design.

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
Implementation Plans
```

The roadmap defines the overall direction for all subsequent work.

---

# Roadmap Principles

A roadmap should:

* describe project evolution;
* deliver value incrementally;
* remain relatively stable;
* define capabilities rather than implementation tasks;
* minimize unnecessary dependencies between phases.

The roadmap is not a backlog.

The roadmap is not a task tracker.

---

# Current Status

Current phase:

**Phase N — <Name>**

Overall status:

* Planned
* In Progress
* Completed

---

# Phase Template

## Phase N — <Phase Name>

### Goal

Describe the purpose of the phase.

### Expected Outcome

Describe what the project will be capable of after completing this phase.

### Major Capabilities

List the primary capabilities introduced.

### Dependencies

List prerequisite phases, if any.

### Risks

Describe significant risks associated with this phase.

### Exit Criteria

Describe how to determine that the phase is complete and the project is ready for the next phase.

Repeat this structure for each roadmap phase.

---

# Future Direction

Describe future phases at a high level.

Avoid unnecessary implementation detail.

Future phases are expected to evolve as the project matures.

---

# Relationship to Plans

Each roadmap phase is implemented through one or more implementation plans.

Typical structure:

```text
Roadmap Phase
        │
        ├── Plan 001
        ├── Plan 002
        ├── Plan 003
        └── ...
```

The roadmap defines **what capabilities are delivered**.

Implementation plans define **how each capability is implemented**.

---

# Repository Relationships

This document should be read together with:

| Document          | Purpose                             |
| ----------------- | ----------------------------------- |
| `PROJECT.md`      | Defines why the project exists      |
| `ARCHITECTURE.md` | Defines the target system structure |
| `ENGINEERING.md`  | Defines implementation conventions  |
| Plans             | Deliver roadmap phases              |
| `PROGRESS.md`     | Records completed phases            |

---

# Roadmap Evolution

Update this document only when project direction changes.

Examples:

* new major capability;
* significant reprioritization;
* project scope changes;
* architectural strategy changes.

Routine implementation work should not modify the roadmap.

---

# Success Criteria

A roadmap is successful when:

* project direction is clear;
* implementation phases are logically ordered;
* each phase delivers meaningful value;
* implementation plans can be derived naturally from roadmap phases;
* project evolution remains understandable throughout its lifecycle.

---

# Summary

The roadmap connects project vision to implementation.

It answers:

* What major capabilities will be delivered?
* In what order will they be delivered?
* How does the project evolve over time?
* Which phase is currently active?

The roadmap should remain stable while implementation plans evolve beneath it.
