# ADR-NNN — <Short Title>

**Status:** Proposed | Accepted | Deprecated | Superseded

**Date:** YYYY-MM-DD

**Superseded by:** ADR-NNN (optional, when status is Superseded)

---

# Context

Describe the situation that requires a decision.

Include:

* the problem or opportunity;
* relevant constraints;
* current project state;
* forces that influence the decision.

Provide enough background so a future reader can understand why the decision was needed without relying on chat history or prior conversations.

---

# Decision

State the decision clearly and concisely.

Use active voice.

Example:

> We will use PostgreSQL as the primary data store for the application.

The decision should be specific enough to guide implementation and future architectural work.

---

# Rationale

Explain why this decision was made.

Describe:

* how the decision addresses the context;
* which goals or constraints it satisfies;
* why this approach is appropriate for the project at this time.

Focus on reasoning, not implementation details.

---

# Alternatives Considered

List other options that were evaluated.

For each alternative, briefly describe:

* what it is;
* why it was not chosen.

Example:

| Alternative | Reason Rejected |
|-------------|-----------------|
| SQLite | Insufficient concurrency for expected load |
| MongoDB | Team lacks operational experience; relational model fits domain |

If no serious alternatives were considered, state that explicitly and explain why.

---

# Consequences

Describe the expected impact of this decision.

Include:

**Positive:**

* benefits gained;
* problems solved;
* simplifications introduced.

**Negative:**

* trade-offs accepted;
* new constraints introduced;
* operational or maintenance costs.

**Neutral:**

* follow-up work required;
* areas that need monitoring or future review.

Be honest about trade-offs. Consequences help future contributors evaluate whether the decision still holds.

---

# Related Documents

Reference project artifacts connected to this decision.

Examples:

* ARCHITECTURE.md
* Plan XXX
* ADR-NNN
* ROADMAP.md (phase reference)

Link to documents that this decision affects or that motivated it.

---

# ADR Guidelines

## When to Write an ADR

Create an ADR when a decision:

* affects system architecture or component boundaries;
* is difficult or costly to reverse;
* establishes a pattern that future work will follow;
* resolves a significant trade-off;
* needs to be understood by future contributors or agents.

Do not create ADRs for trivial or easily reversible choices.

## Title Format

Use the format:

```text
ADR-NNN — <Short Title>
```

Where:

* `NNN` is a zero-padded sequential number (e.g. `001`, `002`);
* `<Short Title>` is a brief, descriptive name for the decision.

## Status Values

| Status | Meaning |
|--------|---------|
| Proposed | Under discussion; not yet authoritative |
| Accepted | Approved and in effect |
| Deprecated | No longer recommended; retained for history |
| Superseded | Replaced by a newer ADR |

## File Location

Store project ADRs in:

```text
docs/project/adr/
```

Use a filename that matches the title, for example:

```text
docs/project/adr/ADR-001-database-selection.md
```

## Relationship to Other Documents

* **ARCHITECTURE.md** describes the current system structure; ADRs explain why it looks that way.
* **Implementation plans** may reference ADRs when work depends on a recorded decision.
* **PROGRESS.md** may reference ADRs when recording completed work that enacted a decision.

When a decision changes architecture, update ARCHITECTURE.md after the ADR is accepted.
