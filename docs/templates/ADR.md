# ADR-NNN — <Short Title>

**Status:** Proposed | Accepted | Deprecated | Superseded

**Date:** YYYY-MM-DD

**Superseded by:** ADR-NNN (optional)

---

# Purpose

This Architecture Decision Record documents a significant engineering or architectural decision.

ADRs explain **why** the system looks the way it does.

They complement `ARCHITECTURE.md`, which describes **what** the current architecture is.

---

# When to Create

Create an ADR when a decision:

* changes system architecture;
* introduces a new architectural pattern;
* changes component ownership or boundaries;
* establishes a long-term engineering convention;
* resolves a significant trade-off;
* is expensive to reverse.

Do **not** create ADRs for:

* local implementation details;
* temporary experiments;
* trivial refactorings;
* easily reversible decisions.

ADRs are typically created during:

* Architecture Design;
* Engineering Design;
* Plan Implementation (when architectural changes emerge).

---

# Context

Describe the situation that requires a decision.

Include:

* the problem or opportunity;
* relevant constraints;
* current project state;
* competing forces;
* assumptions that influenced the decision.

Provide enough background so that future contributors can understand the decision without relying on chat history.

---

# Decision

State the decision clearly and concisely.

Use active voice.

Example:

> We will use PostgreSQL as the primary relational database.

The decision should guide future implementation.

---

# Rationale

Explain why this decision was made.

Describe:

* how it addresses the context;
* which project goals it supports;
* why it was preferred over alternatives;
* why it is appropriate at this stage of the project.

Focus on engineering reasoning rather than implementation details.

---

# Alternatives Considered

List realistic alternatives that were evaluated.

| Alternative | Reason Not Chosen |
| ----------- | ----------------- |
| Option A    | ...               |
| Option B    | ...               |

If no meaningful alternatives were considered, explain why.

---

# Consequences

Describe the expected impact of the decision.

## Positive

* benefits introduced;
* problems solved;
* simplifications gained.

## Negative

* trade-offs accepted;
* new constraints;
* operational costs;
* maintenance implications.

## Follow-up

* additional work required;
* documentation updates;
* implementation considerations;
* future review points.

---

# Related Documents

Reference repository artifacts related to this decision.

Typical references:

* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`
* `ENGINEERING.md`
* relevant implementation plans
* related ADRs

---

# ADR Lifecycle

Typical lifecycle:

```text
Proposed
        ↓
Accepted
        ↓
Deprecated
        ↓
Superseded
```

Only **Accepted** ADRs represent the authoritative architecture.

Deprecated and Superseded ADRs remain in the repository for historical traceability.

---

# Repository Relationships

`ARCHITECTURE.md`

: describes the current system architecture.

`ENGINEERING.md`

: describes engineering conventions that may result from this decision.

Implementation Plans

: implement the decision.

`PROGRESS.md`

: records when the decision was delivered.

---

# Writing Guidelines

Use concise, factual language.

Describe:

* why the decision exists;
* what alternatives were considered;
* what trade-offs were accepted.

Avoid:

* implementation details;
* speculative discussion;
* temporary design ideas;
* conversational history.

An ADR should remain understandable years after it was written.
