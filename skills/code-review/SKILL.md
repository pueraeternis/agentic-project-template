# Code Review

## Purpose

This skill reviews completed implementation before it becomes part of the project's engineering history.

The objective is to verify that the implementation:

* satisfies the approved implementation plan;
* follows the documented architecture;
* follows the approved engineering conventions;
* preserves repository consistency;
* introduces no unintended scope.

Code Review is the final quality gate before recording project progress.

---

# Lifecycle Stage

```text
Plan Implementation
        ↓
Code Review
        ↓
Progress Update
```

Code Review validates completed implementation.

It does not redesign the project.

---

# Role

Primary role:

**Review Agent**

---

# When to Use

Use this skill when:

* implementation has been completed;
* validation has been performed;
* documentation has been updated;
* implementation is ready for acceptance.

Perform Code Review before committing completed work to project history.

---

# Inputs

Required:

* approved implementation plan;
* implementation changes;
* `PROJECT.md`;
* `ROADMAP.md`;
* `ARCHITECTURE.md`;
* `ENGINEERING.md`.

Additional references:

* ADRs;
* completed plans;
* current repository state.

---

# Outputs

Produce one review outcome:

* **Approved**
* **Approved with Minor Suggestions**
* **Changes Requested**

Every requested change should include clear reasoning and evidence.

---

# Procedure

## Step 1 — Understand the Intent

Review:

* implementation plan;
* implementation scope;
* acceptance criteria;
* validation requirements.

Understand the approved engineering intent before reviewing code.

---

## Step 2 — Review the Implementation

Evaluate:

* correctness;
* completeness;
* maintainability;
* readability;
* consistency.

Look for unintended behavior and incomplete implementation.

---

## Step 3 — Verify Scope Compliance

Confirm that:

* only approved functionality has been implemented;
* no undocumented features have been introduced;
* no unrelated refactoring has occurred;
* implementation remains within approved scope.

Reject undocumented scope expansion.

---

## Step 4 — Verify Engineering Compliance

Verify consistency with:

* architecture;
* engineering conventions;
* repository standards;
* ADRs.

Confirm that implementation follows the engineering workflow defined in `ENGINEERING.md`.

---

## Step 5 — Review Validation

Confirm that:

* validation commands succeeded;
* tests passed;
* documentation was updated where required;
* repository remains internally consistent.

Review evidence rather than assumptions.

---

## Step 6 — Evaluate Findings

Classify findings as:

* Critical;
* Major;
* Minor;
* Suggestion.

Prioritize findings by engineering impact.

---

## Step 7 — Produce Review

Summarize:

* implementation quality;
* scope compliance;
* engineering compliance;
* validation results;
* review outcome.

Clearly state whether implementation is approved.

---

# Rules

Do:

* review against approved documentation;
* verify engineering compliance;
* verify traceability;
* provide objective, actionable feedback.

Do not:

* redesign the project;
* redefine architecture;
* introduce new engineering decisions;
* request unrelated improvements;
* block approval because of personal preferences.

Suggestions outside the approved scope should remain optional.

---

# Principles

A good review is:

* objective;
* evidence-based;
* proportional;
* actionable;
* traceable.

Review implementation against documented intent rather than hypothetical future improvements.

Correctness takes priority over optimization.

Scope compliance takes priority over feature requests.

---

# Success Criteria

The skill is complete when:

* implementation has been evaluated against the approved plan;
* engineering conventions have been verified;
* validation has been reviewed;
* significant issues have been documented;
* a review outcome has been produced;
* the human can confidently approve or reject the implementation.

---

# Handover

If the implementation is approved:

1. Update `PROGRESS.md`.
2. Move the implementation plan to `completed/`.
3. Begin the next implementation cycle with **Plan Creation**.
