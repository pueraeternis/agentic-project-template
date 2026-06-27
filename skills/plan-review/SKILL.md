# SKILL.md

# Plan Review

## Purpose

This skill reviews an implementation plan before any code is written.

Plan Review validates the engineering contract before implementation authorization.

The review ensures that:

- the implementation increment is well-defined;
- repository documentation is consistent;
- implementation can proceed without additional design work.

The review ensures that implementation begins from a high-quality engineering plan.

---

## Role

Review Agent

---

## When to Use

Use this skill when:

- a new implementation plan has been created;
- an existing plan has been significantly modified.

Always perform this review before implementation begins.

---

## Inputs

The skill requires:

- the implementation plan;
- `PROJECT.md`;
- `ROADMAP.md`;
- `ARCHITECTURE.md`;
- relevant ADRs;
- previous completed plans (when applicable).

**`PROJECT.md`** provides:

- project intent;
- Background;
- Core Idea;
- MVP.

**`ROADMAP.md`** provides:

- implementation strategy;
- current phase.

**`ARCHITECTURE.md`** provides:

- system boundaries;
- dependency rules.

**ADRs** provide:

- accepted architectural decisions.

The implementation plan is the proposed engineering contract.

---

## Outputs

The skill produces one of two outcomes:

- **Approved** — the plan is ready for implementation.
- **Changes Requested** — the plan requires revisions before implementation.

When changes are requested, provide clear, actionable feedback.

---

## Review Procedure

### Step 1 — Build Project Context

Explicitly review:

- `PROJECT.md`;
- `ROADMAP.md`;
- `ARCHITECTURE.md`;
- relevant ADRs;
- previous completed plans (when applicable).

The reviewer should understand why this implementation increment exists.

Understand where this plan fits within the project.

---

### Step 2 — Verify Scope

Confirm that:

- the scope is clearly defined;
- the implementation boundary is explicit;
- the plan does not exceed the current roadmap phase;
- no unrelated work has been introduced;
- every major implementation item can be traced to `PROJECT.md`, `ROADMAP.md`, `ARCHITECTURE.md`, or an accepted ADR.

Reject undocumented implementation work.

---

### Step 3 — Verify Completeness

Confirm that the plan contains:

- objective;
- scope;
- acceptance criteria;
- implementation approach;
- validation requirements;
- implementation checklist.

The implementation agent should not need to invent missing requirements.

---

### Step 4 — Verify Consistency

Check that the plan is consistent with:

- project goals;
- roadmap;
- existing architecture;
- previous engineering decisions.

Additionally verify that:

- the plan supports the documented MVP or current roadmap phase;
- no unresolved architectural decisions remain.

Plans should not depend on architecture that has not yet been defined.

Identify contradictions and ambiguities.

---

### Step 5 — Evaluate Risks

Review whether the plan introduces:

- unnecessary complexity;
- excessive implementation scope;
- architectural inconsistency;
- hidden assumptions;
- unnecessary future-proofing.

Encourage the simplest solution that satisfies the requirements.

---

### Step 6 — Produce the Review

### Traceability Assessment

Summarize:

- whether the implementation increment is fully justified by project documentation;
- whether undocumented scope exists;
- whether implementation can proceed without further architectural work.

Conclude with one of the following:

- **Approved**
- **Approved with Minor Suggestions**
- **Changes Requested**

Suggestions should be prioritized by importance.

---

## Rules

Do not redesign the project.

Do not introduce new roadmap phases.

Do not expand project scope.

Review the proposed plan, not an idealized future version of the project.

Feedback should remain within the current implementation increment.

---

## Review Principles

A good implementation plan is:

- clear;
- complete;
- bounded;
- consistent;
- implementable;
- reviewable.

Review documented intent before reviewing implementation details.

Every implementation increment should be traceable to documented project knowledge.

The review should improve clarity rather than increase complexity.

---

## Success Criteria

The skill is complete when:

- the implementation scope is validated;
- acceptance criteria are sufficient;
- implementation risks have been reviewed;
- the plan is either approved or returned for revision;
- the human understands the reasoning behind the review outcome.

---

## Next Skill

If approved, continue with:

**Plan Implementation**
