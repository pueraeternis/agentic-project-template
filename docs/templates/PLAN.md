# PLAN.md

# Plan NNN — <Short Title>

**File:** `NNN-short-title.md` (e.g. `001-user-authentication.md`)

**Status:** Draft | Approved | In Progress | Completed | Superseded

**Created:** YYYY-MM-DD

**Approved:** YYYY-MM-DD (optional)

**Completed:** YYYY-MM-DD (optional)

---

# Objective

Describe the objective of this implementation increment.

The objective should explain what this plan accomplishes and why it is needed.

---

# Context

Describe the current project state that motivates this plan.

Reference:

* roadmap phase;
* previous implementation plans;
* architectural constraints;
* relevant ADRs.

The context should explain why this work is the logical next step.

---

# Scope

Describe exactly what is included in this implementation.

Be explicit.

The implementation agent should never need to guess what belongs to the plan.

---

# Out of Scope

Explicitly list what is **not** included.

This section prevents scope creep and clarifies implementation boundaries.

Examples:

* future improvements;
* unrelated refactoring;
* optimization work;
* additional features.

---

# Architectural Impact

Describe whether this plan changes the architecture.

If applicable, identify:

* affected components;
* dependency changes;
* integration changes;
* new architectural constraints.

If significant architectural changes are introduced, create or update an ADR.

---

# Risks

Identify implementation risks.

Examples:

* compatibility risks;
* migration risks;
* performance risks;
* operational risks;
* validation risks.

If no meaningful risks exist, explicitly state so.

---

# Acceptance Criteria

Acceptance criteria should be:

* objective;
* measurable;
* testable.

Examples:

* required functionality works;
* tests pass;
* documentation is updated;
* validation succeeds.

A reviewer should be able to determine whether the implementation satisfies the plan.

---

# Validation

Describe how the implementation will be validated.

Examples:

* unit tests;
* integration tests;
* manual verification;
* performance validation;
* documentation review.

---

# Implementation Checklist

* [ ] Task 1
* [ ] Task 2
* [ ] Task 3

The checklist should represent implementation progress.

Do not use it as a brainstorming list.

---

# Related Documents

Reference relevant project documentation.

Examples:

* PROJECT.md
* ROADMAP.md
* ARCHITECTURE.md
* ADRs
* previous plans

---

# Completion Notes

Complete this section only after implementation has finished.

Summarize:

* completed work;
* deviations from the original plan;
* follow-up work (if any).

Do not rewrite the plan.

Document only factual outcomes.

---

# Plan Lifecycle

## File Naming

Plans use a sequential three-digit prefix and a short kebab-case title:

```text
NNN-short-title.md
```

Examples:

* `001-user-authentication.md`
* `002-api-rate-limiting.md`

Assign the next available number when creating a plan. Do not reuse numbers.

## Status Lifecycle

A plan moves through the following statuses:

```text
Draft → Approved → In Progress → Completed
                              ↘ Superseded
```

| Status | Meaning |
| --- | --- |
| **Draft** | Plan is being written or revised. Does not authorize implementation. |
| **Approved** | Plan has been reviewed and accepted. Ready to move to `active/`. |
| **In Progress** | Implementation is underway. |
| **Completed** | Implementation finished and validated. |
| **Superseded** | Plan replaced by a newer plan. Preserved for history. |

Update the **Status** field and relevant dates when the plan transitions.

## Folder Lifecycle

Plan files move between folders as work progresses:

```text
docs/project/plans/backlog/  →  docs/project/plans/active/  →  docs/project/plans/completed/
```

| Folder | When to use |
| --- | --- |
| `backlog/` | Future work. Plan is a **Draft** or not yet scheduled. |
| `active/` | Authorized work. Plan is **Approved** or **In Progress**. |
| `completed/` | Finished or obsolete work. Plan is **Completed** or **Superseded**. |

Typical transitions:

1. Create the plan in `backlog/` with status **Draft**.
2. After review, set status to **Approved** and move the file to `active/`.
3. When implementation starts, set status to **In Progress**.
4. When implementation finishes, set status to **Completed** and move the file to `completed/`.
5. If a plan is replaced, set status to **Superseded** and move the file to `completed/`.

## Implementation Authorization

Only plans that are **both** in `active/` **and** have status **Approved** or **In Progress** authorize implementation.

Do not implement work described in:

* plans in `backlog/` or `completed/`;
* plans with status **Draft** or **Superseded**.

Every implementation increment should be authorized by exactly one active approved plan.

A completed plan becomes part of the project's engineering history.

It should not be rewritten after completion except to correct factual errors.

---

# Planning Principles

A good implementation plan is:

* focused;
* bounded;
* incremental;
* independently reviewable;
* directly traceable to the roadmap.

Prefer one small implementation increment over one large implementation effort.
