# SKILL.md

# Plan Creation

## Purpose

This skill transforms the current project state into one implementation increment.

The implementation increment should be derived from:

- project vision;
- roadmap;
- architecture;
- completed work.

The goal is to define one bounded, reviewable, and implementable increment of work.

The plan becomes the engineering contract for the next implementation iteration and serves as the contract between planning, implementation, and review.

---

## Role

Planning Agent

---

## When to Use

Use this skill when:

- an approved `ROADMAP.md` exists;
- the next implementation increment needs to be defined;
- a previous implementation plan has been completed.

Do not use this skill to implement code.

Do not use this skill to redesign the project.

---

## Inputs

The skill requires the following inputs. Planning should reconcile all of them before creating a new plan.

**`PROJECT.md`** provides:

- Background;
- Core Idea;
- Vision;
- MVP.

**`ROADMAP.md`** provides:

- current phase;
- delivery strategy.

**`ARCHITECTURE.md`** provides:

- component boundaries;
- dependency rules.

**Completed plans** provide:

- implementation history.

**Current implementation** provides:

- actual repository state.

The planning agent should understand the existing repository before creating a new plan.

---

## Outputs

The skill produces one new implementation plan.

The plan should include:

- objective;
- scope;
- acceptance criteria;
- implementation approach;
- risks;
- validation requirements;
- implementation checklist.

The plan becomes the authoritative specification for the next implementation step.

---

## Procedure

### Step 1 — Build Project Context

Review:

- PROJECT.md;
- ROADMAP.md;
- ARCHITECTURE.md;
- relevant ADRs;
- completed plans;
- current implementation.

The objective is to understand both project intent and implementation history.

Understand what already exists.

Avoid duplicating previous work.

---

### Step 2 — Select the Next Increment

Choose the smallest meaningful increment that moves the project forward.

The increment should:

- deliver measurable value;
- have clear boundaries;
- be independently reviewable;
- be realistically implementable;
- support the MVP or current roadmap phase;
- not require unresolved architectural decisions;
- have a clear dependency chain.

Avoid selecting work that is too large.

---

### Step 3 — Define Scope

Clearly define:

- what is included;
- what is excluded;
- assumptions;
- dependencies.

The implementation agent should never need to guess the scope.

---

### Step 4 — Define Acceptance Criteria

Acceptance criteria should be:

- objective;
- testable;
- observable;
- unambiguous.

A reviewer should be able to determine whether the implementation satisfies the plan.

---

### Step 5 — Consider Risks

Identify:

- architectural risks;
- implementation risks;
- compatibility concerns;
- migration requirements;
- validation challenges.

Not every plan has significant risks, but they should always be considered.

---

### Step 6 — Produce the Plan

Before producing the plan, perform a traceability check.

Verify that every major implementation item can be traced to:

- PROJECT;
- ROADMAP;
- ARCHITECTURE;
- or an approved ADR.

The plan should never introduce undocumented work.

Create a complete implementation plan.

The plan should be immediately executable by an implementation agent without requiring additional design work.

---

## Rules

A plan should describe one implementation increment.

Do not:

- redesign the project;
- rewrite the roadmap;
- introduce unrelated improvements;
- combine multiple roadmap phases;
- silently expand project scope.

Every implementation decision should be traceable back to the roadmap.

---

## Planning Principles

Prefer:

- small plans;
- explicit scope;
- independent increments;
- simple implementation paths;
- measurable acceptance criteria;
- every implementation increment traceable to documented project intent;
- plans that minimize future redesign.

Avoid:

- speculative engineering;
- unnecessary abstraction;
- future-proofing beyond the current increment;
- implementation details unrelated to the current scope.

One plan should normally be implementable within a single development iteration.

---

## Success Criteria

The skill is complete when:

- one implementation increment has been defined;
- the scope is explicit;
- acceptance criteria are measurable;
- implementation boundaries are clear;
- validation requirements are documented;
- the human approves the resulting plan.

---

## Next Skill

After Plan Creation is complete, continue with:

**Plan Review**