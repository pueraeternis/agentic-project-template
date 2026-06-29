# Repository Audit Prompt

Perform a read-only engineering audit of the repository.

Do not modify any files.

## Objectives

Evaluate the current state of the repository with respect to:

* documentation;
* architecture;
* implementation;
* engineering process;
* repository consistency.

The purpose is to identify issues, not to fix them.

---

## Audit Context

Review the repository documentation in the following order:

1. `AGENTS.md`
2. `PROJECT.md`
3. `ROADMAP.md`
4. `ARCHITECTURE.md`
5. Relevant ADRs
6. Active implementation plans
7. `PROGRESS.md`

Then inspect the implementation.

---

## Audit Checklist

Evaluate:

* documentation completeness;
* architectural consistency;
* dependency boundaries;
* implementation quality;
* project structure;
* repository organization;
* testing coverage;
* validation workflow.

---

## Documentation Audit

Verify that:

* documentation is internally consistent;
* architecture matches the implementation;
* completed work is recorded in `PROGRESS.md`;
* active plans reflect current implementation;
* important engineering decisions are documented.

---

## Implementation Audit

Review:

* component organization;
* dependency direction;
* code quality;
* maintainability;
* unnecessary complexity;
* technical debt;
* opportunities to simplify the implementation.

Do not recommend speculative redesign.

---

## Findings

Classify findings by severity:

* Critical
* Major
* Minor
* Suggestion

Support every finding with evidence from the repository.

Avoid subjective preferences.

---

## Deliverable

Produce:

1. Executive summary.
2. Repository strengths.
3. Findings by severity.
4. Recommended next actions.

Do not modify the repository.

Do not propose work outside the documented project scope unless clearly identified as a future recommendation.
