# Repository Audit Prompt

Perform a read-only engineering audit of the repository.

Do not modify any files.

---

# Objectives

Evaluate the repository with respect to:

* documentation quality;
* engineering consistency;
* architectural consistency;
* implementation quality;
* repository organization;
* engineering process.

The objective is to identify issues, not to fix them.

---

# Repository Context

Review the repository in the following order:

1. `AGENTS.md`
2. `docs/project/PROJECT.md`
3. `docs/project/ROADMAP.md`
4. `docs/project/ARCHITECTURE.md`
5. `docs/project/ENGINEERING.md`
6. Relevant ADRs
7. Active implementation plans
8. `docs/project/PROGRESS.md`

Then inspect the implementation.

---

# Audit Checklist

Evaluate:

* documentation completeness;
* project consistency;
* engineering consistency;
* architectural consistency;
* dependency boundaries;
* implementation quality;
* repository organization;
* testing strategy;
* validation workflow.

---

# Documentation Audit

Verify that:

* repository documentation is internally consistent;
* project documentation is complete;
* architecture matches the implementation;
* engineering decisions match the implementation;
* completed work is reflected in `PROGRESS.md`;
* active plans match the current implementation;
* significant engineering decisions are documented.

---

# Engineering Audit

Verify that the implementation follows the documented engineering decisions.

Examples include:

* language and runtime versions;
* repository layout;
* dependency management;
* configuration strategy;
* testing strategy;
* validation workflow;
* coding conventions.

Do not infer undocumented engineering conventions.

---

# Architecture Audit

Review:

* component organization;
* dependency direction;
* architectural boundaries;
* ownership rules;
* integration points.

Recommend architectural changes only when supported by repository evidence.

Avoid speculative redesign.

---

# Implementation Audit

Review:

* code quality;
* maintainability;
* unnecessary complexity;
* technical debt;
* testing quality;
* documentation updates.

Focus on observable repository evidence.

---

# Findings

Classify findings as:

* Critical
* Major
* Minor
* Suggestion

Support every finding with repository evidence.

Avoid subjective preferences.

---

# Deliverable

Produce:

1. Executive Summary
2. Repository Strengths
3. Findings by Severity
4. Recommended Next Actions

Recommendations should remain within the documented project scope.

Future ideas should be clearly identified as recommendations rather than required changes.

Do not modify the repository.
