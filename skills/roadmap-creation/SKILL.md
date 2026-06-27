# SKILL.md

# Roadmap Creation

## Purpose

This skill transforms shared project understanding into a long-term implementation strategy.

It takes an approved `PROJECT.md` and produces a high-level roadmap that describes how the project evolves from the MVP toward the complete vision.

The roadmap defines the major phases of project evolution and provides the foundation for future implementation plans.

The roadmap bridges project vision and engineering execution while remaining implementation-independent.

---

## Role

Reasoning Agent

---

## When to Use

Use this skill when:

- a new `PROJECT.md` has been approved;
- the overall implementation strategy needs to be defined;
- the project scope changes significantly.

Do not use this skill for implementation planning or technical design.

---

## Inputs

The skill requires:

- an approved `PROJECT.md`.

`PROJECT.md` provides the conceptual artifacts from which the roadmap is derived:

- Background;
- Core Idea;
- Vision;
- Goals;
- MVP;
- Constraints.

The project vision should already be stable before roadmap creation begins.

---

## Outputs

The skill produces:

- a completed `ROADMAP.md`;
- a sequence of implementation phases;
- a high-level implementation strategy;
- phase dependencies;
- an incremental delivery path from MVP to project completion.

The roadmap should provide enough structure to begin writing implementation plans.

---

## Procedure

### Step 1 — Build Project Context

Review the project definition and explicitly examine:

- Background;
- Core Idea;
- Vision;
- Goals;
- MVP;
- Constraints.

The objective is to understand the intended evolution of the project before defining implementation phases.

The roadmap should remain aligned with the approved project vision.

---

### Step 2 — Identify Major Milestones

Break the project into a small number of meaningful phases.

Each phase should represent a significant step in the evolution of the product.

Verify that:

- every phase delivers meaningful new capability;
- the MVP appears as an explicit early phase;
- later phases build naturally upon earlier phases.

Avoid implementation details.

The roadmap should describe capability evolution rather than implementation activities.

Think in terms of capabilities rather than code.

---

### Step 3 — Define Dependencies

Arrange the phases in a logical implementation order.

Earlier phases should enable later ones.

Introduce dependencies only when they simplify implementation or reflect genuine capability prerequisites.

Avoid creating artificial phase dependencies.

Minimize unnecessary dependencies.

The roadmap should support incremental development.

---

### Step 4 — Validate the Roadmap

Review the roadmap for:

- logical progression;
- realistic scope;
- independent milestones;
- clear MVP delivery path;
- every phase supports the documented project vision;
- every phase can be traced back to documented project goals;
- no phase exists solely because of implementation convenience.

Every phase should move the project meaningfully forward.

The roadmap should remain product-driven rather than implementation-driven.

---

### Step 5 — Produce ROADMAP.md

Populate the roadmap template.

Describe each phase clearly enough that future implementation plans can be created without redefining project strategy.

---

## Rules

During Roadmap Creation:

- focus on project evolution rather than implementation;
- describe capabilities, not code;
- avoid frameworks, libraries, and technologies;
- avoid implementation tasks;
- avoid architectural details;
- avoid file-level planning.

The roadmap defines *what* should be built first, not *how* it will be implemented.

---

## Roadmap Principles

A roadmap should be:

- incremental;
- easy to understand;
- stable;
- implementation-independent;
- focused on delivering value;
- beginning with the MVP;
- evolving capabilities incrementally;
- justified by project value in every phase.

One roadmap phase will typically require multiple implementation plans.

The roadmap should remain relatively stable throughout the project.

Individual implementation plans are expected to evolve much more frequently.

---

## Success Criteria

The skill is complete when:

- the implementation strategy is clear;
- project phases are logically ordered;
- dependencies are understood;
- the roadmap supports incremental delivery;
- the human approves the resulting `ROADMAP.md`.

---

## Next Skill

After Roadmap Creation is complete, continue with:

**Architecture Design**