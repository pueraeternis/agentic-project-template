# Code Review Prompt

Review the completed implementation using the Agentic Engineering Methodology.

---

# Objective

Verify that the implementation:

* satisfies the approved implementation plan;
* preserves repository consistency;
* respects the documented architecture;
* follows documented engineering conventions;
* introduces no unintended scope.

The review should focus on correctness, consistency, maintainability, and traceability.

---

# Repository Context

Review the repository documentation in the following order:

1. `AGENTS.md`
2. `docs/project/PROJECT.md`
3. `docs/project/ROADMAP.md`
4. `docs/project/ARCHITECTURE.md`
5. `docs/project/ENGINEERING.md`
6. Relevant ADRs
7. Approved implementation plan

Then review the implementation changes.

---

# Review Checklist

Verify:

* implementation completeness;
* correctness;
* maintainability;
* readability;
* architectural consistency;
* engineering consistency;
* documentation updates;
* validation results.

Confirm that the implementation satisfies the documented acceptance criteria.

---

# Scope Compliance

Confirm that:

* only approved functionality has been implemented;
* no unrelated refactoring has been introduced;
* no hidden behavior has been added;
* architectural boundaries have been respected;
* engineering conventions have been followed.

Reject unnecessary scope expansion.

---

# Engineering Quality

Review:

* code organization;
* naming;
* type safety;
* error handling;
* logging;
* testing;
* documentation.

Use `ENGINEERING.md` as the source of truth for project-specific engineering conventions.

Prefer simple, maintainable implementations.

Avoid requesting improvements outside the approved scope.

---

# Findings

Classify findings by severity:

* Critical
* Major
* Minor
* Suggestion

Only Critical and Major findings should block approval.

---

# Review Outcome

Conclude with one of:

* **Approved**
* **Approved with Minor Suggestions**
* **Changes Requested**

Explain the reasoning for the outcome.

Suggestions outside the approved implementation scope should be clearly identified as optional.
