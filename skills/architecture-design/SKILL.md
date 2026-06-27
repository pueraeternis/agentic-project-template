# SKILL.md

# Architecture Design

## Purpose

This skill transforms an approved `PROJECT.md` and `ROADMAP.md` into a stable system architecture.

The architecture defines how the system is organized before implementation planning begins.

It establishes system structure, component boundaries, dependency rules, and major components so that implementation plans can be written against a shared technical foundation.

Architecture Design bridges project strategy and implementation planning.

---

## Role

Reasoning Agent or Architecture Agent

---

## When to Use

Use this skill when:

- an approved `ROADMAP.md` exists;
- the system structure needs to be defined before the first implementation plan;
- a roadmap phase introduces new major components or boundaries;
- architectural boundaries or dependency rules need to change.

Do not use this skill for:

- project vision definition;
- roadmap creation;
- implementation planning;
- writing production code.

Architecture is created after roadmap approval and before plan creation.

---

## Inputs

The skill requires:

- an approved `PROJECT.md`;
- an approved `ROADMAP.md`;
- current project documentation (when updating an existing architecture);
- relevant ADRs (when architecture already exists).

The roadmap should already be stable before architecture design begins.

---

## Outputs

The skill produces:

- a completed or updated `ARCHITECTURE.md`;
- defined system structure and major components;
- documented architectural boundaries;
- explicit dependency rules;
- one or more ADRs when significant architectural decisions are made.

The architecture should provide enough structure for implementation plans to be created without redesigning the system.

---

## Procedure

### Step 1 — Understand the Project and Roadmap

Review:

- `PROJECT.md`;
- `ROADMAP.md`;
- existing architecture documentation (if any);
- relevant ADRs.

Identify:

- project goals and constraints;
- MVP scope and near-term phases;
- major capabilities to be delivered;
- external systems and integration points;
- constraints that affect system structure.

The architecture should support the approved roadmap, not replace it.

---

### Step 2 — Define System Structure

Identify the major components of the system.

For each component, define:

- purpose;
- responsibilities;
- inputs and outputs;
- allowed dependencies;
- constraints.

Focus on components required for the current and immediately upcoming roadmap phases.

Avoid defining components that exist only for distant future phases.

---

### Step 3 — Establish Boundaries and Dependency Rules

Define:

- architectural boundaries between components;
- allowed dependency directions;
- prohibited dependencies;
- ownership of data and control flow.

Boundaries should prevent coupling that would make future implementation harder to reason about.

Dependency rules should be explicit enough that an implementation agent can follow them without guessing.

---

### Step 4 — Document External Systems and Flows

Describe:

- external systems and integration boundaries;
- primary data flow paths;
- primary control flow paths;
- validation and safety boundaries relevant to the architecture.

Keep the description at the architectural level.

Implementation details belong in plans.

---

### Step 5 — Record Significant Decisions

When a design choice has long-term consequences, create an ADR.

Significant decisions include choices about:

- major component structure;
- integration patterns;
- persistence strategy;
- communication models;
- security or safety boundaries;
- technology selection with architectural impact.

Not every architectural detail requires an ADR.

Use ADRs for decisions that future work must respect or revisit.

---

### Step 6 — Validate the Architecture

Review the architecture for:

- alignment with `PROJECT.md` and `ROADMAP.md`;
- clear component boundaries;
- explicit dependency rules;
- scope limited to current and near-term needs;
- no overdesign of future phases;
- sufficient detail for plan creation.

Every major component should have a clear reason to exist in the current roadmap context.

---

### Step 7 — Produce ARCHITECTURE.md

Populate the architecture template.

Describe the system clearly enough that implementation plans can be created without additional architectural design.

Document deferred decisions explicitly rather than solving problems before they are relevant.

---

## Rules

During Architecture Design:

- define system structure, boundaries, dependency rules, and major components;
- align architecture with the approved roadmap;
- scope architecture to current and near-term roadmap phases;
- defer design for future phases unless required now;
- record significant decisions as ADRs;
- focus on organization, not implementation tasks.

Do not:

- redefine project vision;
- rewrite the roadmap;
- create implementation plans;
- overdesign for future phases;
- specify file-level implementation details;
- choose technologies without architectural justification;
- document ordinary implementation changes in `ARCHITECTURE.md`.

The architecture defines *how the system is organized*, not *what code to write next*.

---

## Architecture Principles

An architecture should be:

- stable;
- explicit;
- boundary-driven;
- aligned with the roadmap;
- sufficient for planning;
- resistant to unnecessary complexity.

Near-term roadmap phases should be architecturally supported.

Future phases may be acknowledged but should not drive premature design.

Individual implementation plans are expected to evolve more frequently than the architecture.

---

## Success Criteria

The skill is complete when:

- system structure is defined;
- major components and their responsibilities are documented;
- architectural boundaries are explicit;
- dependency rules are documented;
- the architecture supports the approved roadmap;
- future phases are not overdesigned;
- significant decisions are recorded in ADRs where appropriate;
- the human approves the resulting `ARCHITECTURE.md`.

---

## Next Skill

After Architecture Design is complete, continue with:

**Plan Creation**
