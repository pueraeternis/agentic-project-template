# Plan Review Prompt

Review the proposed implementation plan before any code is written.

## Objectives

Determine whether the plan is ready for implementation.

The review should verify that the plan is:

* complete;
* coherent;
* appropriately scoped;
* aligned with the project documentation.

---

## Review Context

Review the following repository documentation:

1. `AGENTS.md`
2. `PROJECT.md`
3. `ROADMAP.md`
4. `ARCHITECTURE.md`
5. Relevant ADRs
6. The implementation plan

Evaluate the plan against the documented project intent.

---

## Review Checklist

Verify that the plan:

* defines one implementation increment;
* has explicit scope;
* identifies out-of-scope work;
* contains measurable acceptance criteria;
* includes validation requirements;
* respects the documented architecture;
* follows the roadmap;
* does not introduce unnecessary complexity.

---

## Scope Review

Confirm that:

* the implementation boundary is clear;
* no unrelated work has been introduced;
* future roadmap phases are not included;
* assumptions are documented.

Reject hidden scope expansion.

---

## Engineering Review

Evaluate:

* clarity;
* completeness;
* consistency;
* implementation feasibility;
* maintainability.

Prefer the simplest plan that satisfies the project goals.

---

## Findings

Classify findings as:

* Major
* Minor
* Suggestion

Only Major findings should block implementation.

Avoid requesting unrelated improvements.

---

## Review Outcome

Conclude with one of:

* **Approved**
* **Approved with Minor Suggestions**
* **Changes Requested**

Explain the reasoning for the outcome.

Focus on improving the implementation plan rather than redesigning the project.
