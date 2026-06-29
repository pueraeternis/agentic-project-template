# Code Review Prompt

Review the completed implementation using the Agentic Engineering Methodology.

## Objectives

Verify that the implementation:

* satisfies the approved implementation plan;
* preserves repository consistency;
* respects the documented architecture;
* introduces no unintended changes.

The review should focus on correctness rather than redesign.

---

## Review Context

Review the following documentation:

1. `AGENTS.md`
2. `PROJECT.md`
3. `ROADMAP.md`
4. `ARCHITECTURE.md`
5. Relevant ADRs
6. Approved implementation plan

Then review the implementation itself.

---

## Review Checklist

Verify:

* implementation completeness;
* correctness;
* maintainability;
* readability;
* architectural consistency;
* documentation updates;
* validation results.

Confirm that the implementation satisfies the documented acceptance criteria.

---

## Scope Compliance

Confirm that:

* only approved functionality has been implemented;
* no unrelated refactoring has been introduced;
* no hidden behavior has been added;
* project boundaries have been respected.

Reject unnecessary scope expansion.

---

## Engineering Quality

Review:

* code organization;
* naming;
* type safety;
* error handling;
* logging;
* testing;
* documentation.

Prefer simple, maintainable implementations.

Avoid requesting improvements outside the approved scope.

---

## Findings

Classify findings by severity:

* Critical
* Major
* Minor
* Suggestion

Only Critical and Major findings should block approval.

---

## Review Outcome

Conclude with one of:

* **Approved**
* **Approved with Minor Suggestions**
* **Changes Requested**

Explain the reasoning for the outcome.

Suggestions outside the approved implementation scope should be clearly identified as optional.
