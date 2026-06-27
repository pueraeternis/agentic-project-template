# SKILL.md

# Code Review

## Purpose

This skill reviews an implementation after development has been completed.

The goal is to verify that the implementation satisfies the approved plan, maintains project quality, and does not introduce unintended changes.

The review focuses on correctness, consistency, maintainability, and compliance with the documented engineering process.

---

## Role

Review Agent

---

## When to Use

Use this skill when:

- implementation has been completed;
- validation has been performed;
- the implementation is ready for review.

The review should occur before merging or committing the changes.

---

## Inputs

The skill requires:

- the approved implementation plan;
- the implementation diff;
- PROJECT.md;
- ROADMAP.md;
- architecture documentation (if available);
- relevant decision records (if available).

---

## Outputs

The skill produces one of the following outcomes:

- Approved
- Approved with Minor Suggestions
- Changes Requested

The review should include clear reasoning for every requested change.

---

## Review Procedure

### Step 1 — Understand the Intent

Understand not only what was implemented, but why.

Review:

- the implementation plan;
- acceptance criteria;
- implementation scope.

Verify that the implementation can be traced back to the approved plan.

The reviewer should understand the approved engineering intent before evaluating the changes.

---

### Step 2 — Review the Changes

Inspect the implementation.

Verify:

- correctness;
- completeness;
- readability;
- maintainability;
- consistency with existing code.

Look for unintended behavior.

---

### Step 3 — Verify Scope Compliance

Confirm that:

- only approved functionality has been implemented;
- no unrelated changes have been introduced;
- no hidden refactoring has been performed;
- project boundaries have been respected;
- every significant implementation change can be traced to an approved plan item or documented architectural decision.

Reject unnecessary scope expansion.

Reject undocumented functionality, even if technically correct.

---

### Step 4 — Verify Engineering Quality

Review:

- code organization;
- naming;
- error handling;
- testing;
- documentation updates;
- architectural consistency;
- consistency with documented architecture;
- consistency with relevant ADRs (when applicable).

Ensure the implementation follows repository conventions.

Ensure the implementation remains aligned with documented project knowledge.

---

### Step 5 — Evaluate Risks

Identify:

- bugs;
- regressions;
- missing validation;
- architectural violations;
- maintainability concerns.

Prioritize findings according to their impact.

---

### Step 6 — Produce the Review

Summarize the review.

Classify findings by severity:

- Critical
- Major
- Minor
- Suggestion

### Traceability Assessment

Summarize:

- whether the implementation fully matches the approved plan;
- whether undocumented functionality was introduced;
- whether documentation updates appear sufficient.

This is not another approval decision.

It is a short assessment of engineering traceability.

Conclude with one of:

- Approved
- Approved with Minor Suggestions
- Changes Requested

---

## Rules

Review the implementation against:

- the approved plan;
- the documented architecture;
- repository conventions.

Do not:

- redesign the project;
- introduce unrelated improvements;
- request changes outside the approved scope;
- recommend speculative refactoring.

Suggestions outside the approved scope may be recorded separately, but should not block approval.

---

## Review Principles

The purpose of review is to improve implementation quality.

Not to redesign the project.

Not to rewrite the implementation.

Not to enforce personal coding preferences.

A good review is:

- objective;
- actionable;
- evidence-based;
- proportional to the impact of the issue.

Review documented intent before reviewing implementation details.

The reviewer should verify that the implementation solves the approved problem before evaluating coding style or optimization opportunities.

Focus on correctness before optimization.

Focus on scope before future improvements.

---

## Success Criteria

The skill is complete when:

- the implementation has been evaluated against the approved plan;
- all significant issues have been documented;
- the review outcome is clearly communicated;
- the human can confidently decide whether to approve the implementation.

---

## Next Skill

After the implementation is approved:

- commit the changes;
- update project progress if required;
- continue with **Plan Creation** for the next implementation increment.