# Architecture Design

## Purpose

This skill transforms an approved project definition and roadmap into a stable system architecture.

It defines the long-term organization of the system before engineering design and implementation begin.

The resulting architecture becomes the foundation for engineering decisions and implementation planning.

---

# Lifecycle Stage

```text
Project Discovery
        ↓
Roadmap Creation
        ↓
Architecture Design
        ↓
Engineering Design
```

Architecture Design defines **how the system is organized**.

Engineering Design later defines **how that architecture will be implemented**.

---

# Role

Primary role:

**Architecture Agent**

This skill may also be executed by another reasoning-capable agent when acting in the Architecture Agent role.

---

# When to Use

Use this skill when:

* `PROJECT.md` has been approved;
* `ROADMAP.md` has been approved;
* the initial architecture must be created;
* a roadmap phase introduces new architectural capabilities;
* architectural boundaries need to evolve.

Do not use this skill for:

* project discovery;
* engineering decisions;
* repository initialization;
* implementation planning;
* production code.

---

# Inputs

Required:

* `PROJECT.md`
* `ROADMAP.md`

Optional:

* existing `ARCHITECTURE.md`
* existing ADRs

The project vision and roadmap should already be stable.

---

# Outputs

Produce:

* `ARCHITECTURE.md`
* ADRs (when required)

The architecture should provide sufficient structure for Engineering Design without introducing implementation details.

---

# Procedure

## Step 1 — Understand the Project

Review:

* project goals;
* roadmap phases;
* constraints;
* target users;
* expected capabilities.

Architecture must support the approved project direction.

---

## Step 2 — Design the System

Define:

* major components;
* responsibilities;
* ownership boundaries;
* dependency rules;
* integration points.

Focus on stable system organization rather than implementation.

---

## Step 3 — Define Flows

Document:

* control flow;
* data flow;
* external integrations;
* trust boundaries.

Remain at the architectural level.

---

## Step 4 — Record Architectural Decisions

Create ADRs when decisions:

* establish long-term architecture;
* introduce significant trade-offs;
* are expensive to reverse.

Avoid ADRs for implementation details.

---

## Step 5 — Validate

Verify that:

* architecture supports the roadmap;
* boundaries are explicit;
* responsibilities are clear;
* dependency rules are well defined;
* future phases are not overdesigned.

---

## Step 6 — Produce Documentation

Complete:

* `ARCHITECTURE.md`
* ADRs (if required)

The resulting documentation should allow Engineering Design to begin without further architectural discussions.

---

# Rules

Do:

* define stable system structure;
* document responsibilities;
* define architectural boundaries;
* define dependency rules;
* keep architecture implementation-independent;
* defer speculative design.

Do not:

* choose engineering tooling;
* define repository structure;
* select development workflow;
* define testing strategy;
* create implementation plans.

Those responsibilities belong to Engineering Design.

---

# Principles

A good architecture is:

* stable;
* understandable;
* boundary-driven;
* minimally complex;
* aligned with the roadmap;
* implementation-independent.

Design for current and near-term roadmap phases.

Avoid speculative architecture.

---

# Success Criteria

The skill is complete when:

* `ARCHITECTURE.md` is complete;
* major components are documented;
* responsibilities are defined;
* dependency rules are explicit;
* ADRs have been created where appropriate;
* the architecture supports Engineering Design;
* the human approves the resulting architecture.

---

# Handover

After Architecture Design is approved, continue with:

**Engineering Design**

The Engineering Agent will translate the architecture into implementation conventions, repository structure, tooling, and engineering standards before repository initialization begins.
