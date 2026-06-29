# Plan Implementation

## Purpose

This skill implements one approved implementation plan.

Implementation is the execution of an approved engineering contract.

The objective is to translate documented project intent into production-ready implementation while preserving architecture, engineering conventions, and repository consistency.

Implementation should satisfy the approved plan without introducing unrelated work.

---

# Lifecycle Stage

```text
Plan Review
        ↓
Plan Implementation
        ↓
Code Review
```

Plan Implementation realizes the approved implementation increment.

It does not redesign the project.

---

# Role

Primary role:

**Implementation Agent**

---

# When to Use

Use this skill when:

* an implementation plan has been approved;
* implementation has been authorized;
* required project documentation exists.

Do not begin implementation before Plan Review has approved the plan.

---

# Inputs

Required:

* approved implementation plan;
* `PROJECT.md`;
* `ROADMAP.md`;
* `ARCHITECTURE.md`;
* `ENGINEERING.md`.

Additional references:

* ADRs;
* completed plans;
* current repository state.

The approved implementation plan is the authoritative engineering contract.

---

# Outputs

Produce:

* production-ready implementation;
* tests where appropriate;
* updated documentation when required;
* completed implementation checklist;
* implementation ready for Code Review.

---

# Procedure

## Step 1 — Understand the Engineering Contract

Review the implementation plan.

Verify:

* objective;
* scope;
* out-of-scope items;
* acceptance criteria;
* validation requirements;
* implementation constraints.

Implementation must not begin until the contract is fully understood.

---

## Step 2 — Build Project Context

Review:

* project definition;
* roadmap;
* architecture;
* engineering design;
* ADRs;
* current implementation.

Understand:

* why the implementation exists;
* architectural boundaries;
* engineering conventions;
* existing repository structure.

Avoid assumptions.

---

## Step 3 — Implement the Approved Scope

Implement only the approved work.

Respect:

* project intent;
* roadmap;
* architecture;
* engineering conventions;
* implementation plan.

Keep the implementation as simple as possible.

If additional work is discovered, stop and recommend a new or updated implementation plan.

---

## Step 4 — Validate the Implementation

Verify that:

* acceptance criteria are satisfied;
* validation commands succeed;
* tests pass;
* repository standards are satisfied;
* no regressions have been introduced.

Validation should follow the engineering workflow defined in `ENGINEERING.md`.

---

## Step 5 — Update Documentation

Update repository documentation whenever implementation changes repository knowledge.

Typical updates include:

* completed implementation checklist;
* architecture (when approved changes were implemented);
* ADR references;
* generated documentation.

Documentation and implementation should remain synchronized.

---

## Step 6 — Prepare for Review

Before handover verify:

* implementation is complete;
* validation has been performed;
* documentation is consistent;
* no unrelated changes remain;
* implementation remains within approved scope;
* engineering conventions have been followed.

The repository should be ready for independent review.

---

# Rules

Do:

* implement the approved plan;
* preserve repository consistency;
* follow engineering conventions;
* update documentation when necessary;
* keep implementation simple.

Do not:

* redesign the project;
* redefine architecture;
* modify engineering decisions;
* expand scope;
* introduce speculative improvements;
* implement future roadmap phases.

Implementation follows the approved engineering contract.

---

# Principles

Implementation should be:

* simple;
* maintainable;
* explicit;
* traceable;
* architecture-compliant;
* engineering-compliant.

Prefer the simplest implementation that satisfies the documented requirements.

Avoid unnecessary abstractions and premature optimization.

---

# Success Criteria

The skill is complete when:

* the approved implementation has been completed;
* acceptance criteria are satisfied;
* validation has passed;
* documentation has been updated where required;
* engineering conventions have been followed;
* the implementation is ready for independent Code Review.

---

# Handover

After implementation is complete, continue with:

**Code Review**

The Review Agent validates that the implementation satisfies the approved plan, preserves repository consistency, and is ready to become part of the project's engineering history.
