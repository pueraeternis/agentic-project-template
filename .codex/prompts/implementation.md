# Implementation Prompt

Implement the requested changes using the Agentic Engineering Methodology.

---

# Objective

Implement the approved engineering contract.

The implementation should:

* remain within the approved scope;
* preserve repository consistency;
* respect the documented architecture;
* follow the documented engineering conventions;
* produce production-ready code.

---

# Repository Context

Before implementation, review the repository in the following order:

1. `AGENTS.md`
2. `docs/project/PROJECT.md`
3. `docs/project/ROADMAP.md`
4. `docs/project/ARCHITECTURE.md`
5. `docs/project/ENGINEERING.md`
6. Relevant ADRs
7. Active implementation plan
8. `docs/project/PROGRESS.md`

Confirm that implementation is authorized by an active approved plan.

---

# Implementation Rules

Implement only the approved scope.

Respect:

* architectural boundaries;
* engineering conventions;
* repository organization;
* project validation requirements.

Do not:

* redesign the architecture;
* modify project goals;
* introduce unrelated refactoring;
* implement future roadmap phases;
* add speculative abstractions;
* silently expand scope.

Prefer the simplest implementation that satisfies the documented requirements.

---

# Documentation

If implementation changes:

* architecture;
* engineering decisions;
* repository workflow;
* permanent project knowledge;

update the appropriate documentation as part of the same change.

Do not leave the repository in an inconsistent state.

---

# Validation

Before considering the implementation complete:

* verify the acceptance criteria;
* execute the validation workflow defined in `ENGINEERING.md`;
* ensure documentation is consistent;
* confirm no unrelated changes remain.

---

# Deliverable

Provide:

1. Implementation Summary
2. Files Changed
3. Validation Performed
4. Documentation Updated
5. Follow-up Work Requiring a New Implementation Plan

Do not propose additional features unless explicitly requested.
