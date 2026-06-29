# Progress

## Purpose

This document is the chronological engineering journal of the project.

It records completed implementation increments and significant engineering milestones.

It documents **what has been delivered**, not **what is planned**.

Future work belongs in:

* `ROADMAP.md`
* implementation plans

---

# Relationship to the Project Lifecycle

Progress is the final stage of the implementation lifecycle.

Typical flow:

```text
PLAN
        ↓
IMPLEMENTATION
        ↓
REVIEW
        ↓
PROGRESS
```

Each completed implementation plan should result in one progress entry.

---

# Progress Principles

Each entry should be:

* factual;
* chronological;
* concise;
* implementation-oriented;
* traceable to a completed plan.

Record outcomes.

Do not record intentions.

---

# Entry Template

## YYYY-MM-DD

### Plan NNN — <Title>

**Status**

Completed

---

### Summary

Briefly describe what was delivered.

Examples:

* implemented feature X;
* completed roadmap phase;
* introduced component Y;
* established engineering workflow.

---

### Artifacts

List important repository artifacts produced or updated.

Examples:

* source modules;
* documentation;
* ADRs;
* templates;
* skills;
* configuration.

---

### Validation

Describe how completion was verified.

Examples:

* unit tests passed;
* integration tests passed;
* manual verification completed;
* documentation reviewed;
* code review completed.

Record validation evidence rather than implementation details.

---

### Related Documents

Typical references:

* implementation plan;
* ADRs;
* `ARCHITECTURE.md`;
* `ENGINEERING.md`.

---

### Notes

Optional observations that may help future contributors understand the project history.

Avoid repeating implementation details already documented elsewhere.

---

# Repository Relationships

`PROJECT.md`

: defines project intent.

`ROADMAP.md`

: defines long-term direction.

Implementation Plans

: authorize work.

ADRs

: explain significant engineering decisions.

`PROGRESS.md`

: records completed implementation history.

Together these documents provide a complete history of project evolution.

---

# Change Rules

Update this document only after meaningful implementation milestones.

Typical examples:

* completed implementation plan;
* completed roadmap phase;
* completed architectural milestone;
* completed repository initialization.

Do not update this document for:

* work in progress;
* draft plans;
* temporary experiments;
* intermediate implementation states.

---

# Progress Principles

Do:

* record completed work;
* reference implementation plans;
* reference important repository artifacts;
* preserve chronological order.

Do not:

* record future work;
* maintain TODO lists;
* rewrite previous entries;
* duplicate implementation details.

Previous entries should only be modified to correct factual errors.

---

# Success Criteria

A progress journal is successful when:

* every completed implementation plan is recorded;
* project history is easy to follow;
* engineering milestones are traceable;
* important repository artifacts are discoverable;
* repository evolution can be understood without reading commit history.

---

# Summary

`PROGRESS.md` is the permanent engineering history of the project.

It answers questions such as:

* What has already been delivered?
* When was it delivered?
* Which plan introduced it?
* How was it validated?

The document should provide a concise chronological history of project evolution throughout its lifetime.
