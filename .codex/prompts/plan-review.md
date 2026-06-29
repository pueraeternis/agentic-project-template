# Plan Review Prompt

Review the proposed implementation plan before any code is written.

---

# Objective

Determine whether the plan is ready for implementation.

The review should verify that the plan is:

* complete;
* coherent;
* appropriately scoped;
* traceable;
* aligned with project documentation;
* consistent with engineering decisions.

---

# Repository Context

Review the repository documentation in the following order:

1. `AGENTS.md`
2. `docs/project/PROJECT.md`
3. `docs/project/ROADMAP.md`
4. `docs/project/ARCHITECTURE.md`
5. `docs/project/ENGINEERING.md`
6. Relevant ADRs
7. The implementation plan

Evaluate the plan against the documented project intent, architecture, and engineering conventions.

---

# Review Checklist

Verify that the plan:

* defines exactly one implementation increment;
* has explicit scope;
* identifies out-of-scope work;
* contains measurable acceptance criteria;
* includes validation requirements;
* respects the documented architecture;
* follows the documented engineering conventions;
* supports the current roadmap phase;
* does not introduce unnecessary complexity.

---

# Scope Review

Confirm that:

* the implementation boundary is clear;
* no unrelated work has been introduced;
* future roadmap phases are not included;
* assumptions are documented;
* engineering constraints are explicit.

Reject hidden scope expansion.

---

# Engineering Review

Evaluate:

* clarity;
* completeness;
* consistency;
* implementation feasibility;
* maintainability;
* validation strategy.

Use `ENGINEERING.md` as the source of truth for project-specific engineering conventions.

Prefer the simplest plan that satisfies the documented requirements.

---

# Findings

Classify findings as:

* Major
* Minor
* Suggestion

Only Major findings should block implementation.

Avoid requesting unrelated improvements.

---

# Review Outcome

Conclude with one of:

* **Approved**
* **Approved with Minor Suggestions**
* **Changes Requested**

Explain the reasoning for the outcome.

Focus on improving the implementation plan rather than redesigning the project.
