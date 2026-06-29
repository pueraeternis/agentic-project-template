# Plan Creation

## Purpose

This skill transforms the current project state into a single implementation increment.

Each implementation plan defines one bounded, reviewable, and executable unit of work.

The resulting plan becomes the engineering contract between planning, implementation, and review.

---

# Lifecycle Stage

```text
Repository Initialization
        ↓
Plan Creation
        ↓
Plan Review
```

Plan Creation defines **what will be implemented next**.

It does not perform implementation.

---

# Role

Primary role:

**Planning Agent**

---

# When to Use

Use this skill when:

* project initialization has been completed;
* the next implementation increment must be defined;
* a previous implementation plan has been completed;
* implementation priorities need to be adjusted.

Do not use this skill for:

* project discovery;
* architecture design;
* engineering design;
* production code;
* code review.

---

# Inputs

Required:

* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`
* `ENGINEERING.md`

Additional context:

* ADRs;
* completed plans;
* current repository state.

Planning should reconcile documentation with the actual implementation before producing a new plan.

---

# Outputs

Produce one implementation plan.

The plan should define:

* objective;
* scope;
* out-of-scope items;
* acceptance criteria;
* validation strategy;
* implementation checklist;
* risks.

The plan becomes the authoritative specification for the next implementation increment.

---

# Procedure

## Step 1 — Build Context

Review:

* project definition;
* roadmap;
* architecture;
* engineering design;
* ADRs;
* completed plans;
* current implementation.

Understand both project intent and repository state.

---

## Step 2 — Select the Next Increment

Choose the smallest meaningful implementation increment.

The increment should:

* deliver measurable value;
* support the current roadmap phase;
* respect architecture;
* follow engineering conventions;
* remain independently reviewable.

Avoid large implementation batches.

---

## Step 3 — Define Scope

Clearly define:

* included work;
* excluded work;
* dependencies;
* assumptions.

Implementation should never require guessing the intended scope.

---

## Step 4 — Define Validation

Document:

* acceptance criteria;
* validation commands;
* required testing;
* documentation updates.

Validation should follow `ENGINEERING.md`.

---

## Step 5 — Evaluate Risks

Consider:

* implementation risks;
* compatibility;
* migration;
* validation complexity;
* architectural impact.

Record only meaningful risks.

---

## Step 6 — Verify Traceability

Verify that every major implementation item is traceable to one or more of:

* `PROJECT.md`;
* `ROADMAP.md`;
* `ARCHITECTURE.md`;
* `ENGINEERING.md`;
* ADRs.

The plan must not introduce undocumented project scope.

---

## Step 7 — Produce Documentation

Complete the implementation plan.

The document should allow an Implementation Agent to begin work without additional project design.

---

# Rules

Do:

* create one implementation increment;
* keep scope explicit;
* follow approved architecture;
* follow engineering conventions;
* preserve traceability.

Do not:

* redesign the project;
* modify the roadmap;
* redefine engineering decisions;
* expand scope;
* combine unrelated work.

Planning authorizes implementation.

It does not perform implementation.

---

# Principles

A good implementation plan is:

* focused;
* incremental;
* independently reviewable;
* architecture-compliant;
* engineering-compliant;
* fully traceable.

Prefer multiple small plans over one large plan.

---

# Success Criteria

The skill is complete when:

* one implementation increment has been defined;
* scope is explicit;
* acceptance criteria are measurable;
* validation requirements are documented;
* engineering conventions are respected;
* traceability has been verified;
* the human approves the plan.

---

# Handover

After Plan Creation is approved, continue with:

**Plan Review**

The Review Agent validates that the proposed implementation is complete, consistent, and aligned with the approved project documentation before implementation begins.
