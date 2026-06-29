# Roadmap Creation

## Purpose

This skill transforms an approved project definition into a long-term project evolution strategy.

It produces a roadmap that defines the major capability increments required to evolve the project from the MVP to the complete vision.

The roadmap bridges project intent and system design while remaining implementation-independent.

---

# Lifecycle Stage

```text
Project Discovery
        ↓
Roadmap Creation
        ↓
Architecture Design
```

Roadmap Creation defines **how the project will evolve**.

Architecture Design later defines **how those capabilities will be organized into a system**.

---

# Role

Primary role:

**Roadmap Agent**

This skill may also be executed by another reasoning-capable agent acting in the Roadmap Agent role.

---

# When to Use

Use this skill when:

* `PROJECT.md` has been approved;
* the project implementation strategy must be defined;
* project scope changes significantly;
* major capabilities need to be reorganized.

Do not use this skill for:

* project discovery;
* architecture design;
* engineering design;
* implementation planning;
* production code.

---

# Inputs

Required:

* `PROJECT.md`

The project definition should already be approved and stable.

---

# Outputs

Produce:

* `ROADMAP.md`

The roadmap should define:

* major project phases;
* capability evolution;
* phase dependencies;
* incremental delivery strategy.

The roadmap should provide sufficient structure for Architecture Design.

---

# Procedure

## Step 1 — Understand the Project

Review:

* project vision;
* goals;
* MVP;
* target users;
* constraints;
* assumptions;
* risks.

The roadmap must remain aligned with the approved project definition.

---

## Step 2 — Identify Major Capabilities

Break the project into a small number of meaningful phases.

Each phase should:

* deliver clear user value;
* build upon previous phases;
* remain independently understandable.

Describe capabilities rather than implementation work.

---

## Step 3 — Organize Evolution

Arrange phases into a logical sequence.

Verify:

* MVP appears early;
* dependencies are minimized;
* each phase naturally enables the next.

Avoid implementation-driven ordering.

---

## Step 4 — Validate

Verify that:

* every phase supports project goals;
* the roadmap remains implementation-independent;
* capability progression is logical;
* future work is not overplanned.

Every phase should move the project meaningfully forward.

---

## Step 5 — Produce Documentation

Complete `ROADMAP.md`.

The resulting roadmap should allow Architecture Design to begin without redefining project strategy.

---

# Rules

Do:

* focus on project evolution;
* describe capabilities;
* prioritize incremental value;
* minimize dependencies;
* keep the roadmap stable.

Do not:

* define architecture;
* select technologies;
* define repository structure;
* create implementation plans;
* discuss engineering tooling.

Those responsibilities belong to later lifecycle stages.

---

# Principles

A good roadmap is:

* incremental;
* value-driven;
* stable;
* implementation-independent;
* easy to understand;
* directly traceable to project goals.

One roadmap phase will usually require multiple implementation plans.

---

# Success Criteria

The skill is complete when:

* `ROADMAP.md` is complete;
* project phases are clearly defined;
* capability progression is logical;
* dependencies are understood;
* the roadmap supports Architecture Design;
* the human approves the roadmap.

---

# Handover

After Roadmap Creation is approved, continue with:

**Architecture Design**

The Architecture Agent will translate roadmap phases into a stable system architecture while preserving the project direction established during discovery.
