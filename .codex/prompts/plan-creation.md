# Plan Creation Prompt

Create the next implementation plan using the Agentic Engineering Methodology.

---

# Objective

Produce one bounded implementation plan that:

* advances the current roadmap phase;
* remains consistent with the documented architecture;
* follows the documented engineering conventions;
* authorizes exactly one implementation increment.

---

# Repository Context

Review the repository in the following order:

1. `AGENTS.md`
2. `docs/project/PROJECT.md`
3. `docs/project/ROADMAP.md`
4. `docs/project/ARCHITECTURE.md`
5. `docs/project/ENGINEERING.md`
6. Relevant ADRs
7. Completed implementation plans
8. `docs/project/PROGRESS.md`

Understand the current repository state before proposing new work.

---

# Planning Rules

Create exactly one implementation plan.

The plan should:

* implement one logical engineering increment;
* have explicit implementation boundaries;
* define measurable acceptance criteria;
* identify implementation risks;
* define validation requirements;
* remain consistent with the engineering decisions documented in `ENGINEERING.md`.

Do not:

* redesign the project;
* redesign the architecture;
* combine multiple roadmap phases;
* introduce speculative work;
* silently expand project scope.

---

# Scope

Clearly define:

* included work;
* excluded work;
* dependencies;
* assumptions;
* engineering constraints.

The implementation agent should not need to infer the intended scope.

---

# Acceptance Criteria

Acceptance criteria should be:

* objective;
* measurable;
* testable;
* observable;
* unambiguous.

A reviewer should be able to determine whether the implementation satisfies the plan.

---

# Validation

Define how the implementation will be validated.

Use the validation strategy documented in `ENGINEERING.md`.

Examples include:

* unit tests;
* integration tests;
* manual verification;
* documentation review;
* project validation commands.

---

# Deliverable

Produce a complete implementation plan using the repository plan template.

The resulting plan should be ready for review without requiring additional engineering or architectural design.
