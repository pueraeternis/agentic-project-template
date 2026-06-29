# Plan Creation Prompt

Create the next implementation plan using the Agentic Engineering Methodology.

## Objectives

Produce one bounded implementation plan that:

* advances the roadmap;
* has explicit scope;
* is independently reviewable;
* authorizes exactly one implementation increment.

---

## Before Planning

Review:

1. `AGENTS.md`
2. `PROJECT.md`
3. `ROADMAP.md`
4. `ARCHITECTURE.md`
5. Relevant ADRs
6. Completed implementation plans
7. `PROGRESS.md`

Understand the current project state before proposing new work.

---

## Planning Rules

Create exactly one implementation plan.

The plan should:

* implement one logical increment;
* have explicit boundaries;
* define measurable acceptance criteria;
* identify risks;
* describe validation.

Do not:

* redesign the architecture;
* combine multiple roadmap phases;
* introduce speculative work;
* silently expand project scope.

---

## Scope

Clearly define:

* what is included;
* what is excluded;
* dependencies;
* assumptions.

The implementation agent should not need to guess the intended scope.

---

## Acceptance Criteria

Acceptance criteria must be:

* objective;
* testable;
* observable;
* unambiguous.

A reviewer should be able to determine whether the implementation satisfies the plan.

---

## Validation

Specify how the implementation will be validated.

Examples include:

* unit tests;
* integration tests;
* manual verification;
* documentation review;
* quality commands.

---

## Deliverable

Produce a completed implementation plan using the repository plan template.

The plan should be ready for review without requiring additional design work.
