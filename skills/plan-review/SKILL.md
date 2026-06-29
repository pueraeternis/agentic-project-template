# Plan Review

## Purpose

This skill validates an implementation plan before implementation begins.

The review confirms that the plan is complete, consistent, traceable, and ready for execution.

Plan Review is the final quality gate before implementation authorization.

---

# Lifecycle Stage

```text
Plan Creation
        ↓
Plan Review
        ↓
Plan Implementation
```

Plan Review determines whether implementation can safely begin.

---

# Role

Primary role:

**Review Agent**

---

# When to Use

Use this skill when:

* a new implementation plan has been created;
* an implementation plan has been significantly revised;
* implementation authorization is required.

Always perform this review before implementation begins.

---

# Inputs

Required:

* implementation plan;
* `PROJECT.md`;
* `ROADMAP.md`;
* `ARCHITECTURE.md`;
* `ENGINEERING.md`.

Additional references:

* ADRs;
* completed plans;
* current repository state (when relevant).

The implementation plan is the proposed engineering contract.

---

# Outputs

Produce one review outcome:

* **Approved**
* **Approved with Minor Suggestions**
* **Changes Requested**

When revisions are required, provide clear, prioritized, and actionable feedback.

---

# Procedure

## Step 1 — Build Context

Review:

* project definition;
* roadmap;
* architecture;
* engineering design;
* ADRs;
* completed plans.

Understand why this implementation increment exists.

---

## Step 2 — Verify Scope

Confirm that:

* scope is explicit;
* implementation boundaries are clear;
* work fits the current roadmap phase;
* engineering conventions are respected;
* undocumented work has not been introduced.

Every major implementation item should be traceable to approved project documentation.

---

## Step 3 — Verify Completeness

Confirm the plan contains:

* objective;
* scope;
* out-of-scope items;
* acceptance criteria;
* validation strategy;
* implementation checklist;
* identified risks.

Implementation should not require inventing missing requirements.

---

## Step 4 — Verify Consistency

Verify consistency with:

* project goals;
* roadmap;
* architecture;
* engineering design;
* ADRs.

Confirm that:

* no unresolved architectural issues remain;
* no engineering decisions are contradicted;
* implementation can begin without additional design work.

---

## Step 5 — Evaluate Risks

Review for:

* excessive scope;
* unnecessary complexity;
* hidden assumptions;
* compatibility concerns;
* unnecessary future-proofing.

Prefer the simplest implementation that satisfies the approved documentation.

---

## Step 6 — Verify Traceability

Confirm that implementation items are justified by:

* `PROJECT.md`;
* `ROADMAP.md`;
* `ARCHITECTURE.md`;
* `ENGINEERING.md`;
* ADRs.

Reject undocumented scope expansion.

---

## Step 7 — Produce Review

Summarize:

* strengths;
* issues;
* required changes (if any);
* review outcome.

The review should clearly explain whether implementation may proceed.

---

# Rules

Do:

* review the proposed implementation increment;
* verify consistency;
* verify traceability;
* verify engineering compliance;
* provide actionable feedback.

Do not:

* redesign the project;
* redefine architecture;
* rewrite engineering decisions;
* expand implementation scope;
* review hypothetical future work.

Review the submitted plan, not the ideal project.

---

# Principles

A good implementation plan is:

* complete;
* focused;
* traceable;
* architecture-compliant;
* engineering-compliant;
* immediately implementable.

The review should improve clarity without introducing unnecessary complexity.

---

# Success Criteria

The skill is complete when:

* implementation scope has been validated;
* engineering conventions have been verified;
* acceptance criteria are sufficient;
* validation requirements are complete;
* implementation risks have been reviewed;
* a review outcome has been produced;
* the human understands the review decision.

---

# Handover

If the plan is approved, continue with:

**Plan Implementation**

The Implementation Agent may now execute the approved implementation plan while remaining within the documented project, architecture, and engineering boundaries.
