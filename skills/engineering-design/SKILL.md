# Engineering Design

## Purpose

This skill transforms an approved project architecture into concrete engineering decisions.

It defines **how the approved architecture will be implemented**.

The primary output is `ENGINEERING.md`, which becomes the engineering specification for repository initialization and future implementation.

Engineering Design bridges architecture and implementation.

---

# Lifecycle Stage

```text
Architecture Design
        ↓
Engineering Design
        ↓
Repository Initialization
```

Architecture defines **how the system is organized**.

Engineering Design defines **how that architecture will be implemented**.

---

# Role

Primary role:

**Engineering Agent**

This skill may also be executed by another reasoning-capable agent acting in the Engineering Agent role.

---

# When to Use

Use this skill when:

* `PROJECT.md` has been approved;
* `ROADMAP.md` has been approved;
* `ARCHITECTURE.md` has been approved;
* engineering conventions must be defined;
* repository initialization is the next lifecycle stage.

Do not use this skill for:

* project discovery;
* roadmap creation;
* architecture design;
* repository initialization;
* implementation planning;
* production code.

---

# Inputs

Required:

* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`

Optional:

* ADRs;
* project constraints;
* engineering assumptions discovered earlier.

Architecture should already be sufficiently stable.

---

# Outputs

Produce:

* `ENGINEERING.md`

The document should define:

* programming language;
* runtime versions;
* dependency management;
* quality tooling;
* runtime technologies;
* repository structure;
* testing strategy;
* configuration strategy;
* development workflow;
* coding conventions;
* operational assumptions;
* deferred engineering decisions.

The result should provide sufficient information for Repository Initialization.

---

# Procedure

## Step 1 — Understand the Project

Review:

* project goals;
* roadmap;
* architecture;
* ADRs;
* engineering assumptions.

Identify the engineering implications of the approved architecture.

---

## Step 2 — Select Engineering Stack

Define:

* programming language;
* runtime version;
* dependency manager;
* formatter;
* linter;
* type checker;
* test framework.

Prefer mature, stable, and simple tooling.

---

## Step 3 — Define Runtime Technologies

Document technologies required by the architecture.

Examples:

* web framework;
* agent framework;
* MCP framework;
* LLM provider;
* database;
* vector database;
* configuration library;
* logging.

Only document technologies required by the approved architecture or near-term roadmap.

---

## Step 4 — Define Repository Structure

Describe:

* repository layout;
* source layout;
* documentation layout;
* testing layout;
* configuration files;
* generated artifacts.

The structure should be sufficiently concrete for Repository Initialization.

---

## Step 5 — Define Engineering Workflow

Document:

* validation commands;
* testing strategy;
* development workflow;
* coding conventions;
* configuration strategy.

The workflow should be reproducible by both humans and AI agents.

---

## Step 6 — Document Operational Assumptions

Record assumptions such as:

* development environment;
* deployment targets;
* runtime services;
* infrastructure constraints.

Detailed operational procedures belong later in `RUNBOOK.md`.

---

## Step 7 — Record Deferred Decisions

Explicitly document engineering decisions intentionally postponed.

Examples:

* CI/CD;
* deployment platform;
* observability;
* production infrastructure;
* release process.

Avoid making speculative decisions.

---

## Step 8 — Produce Documentation

Complete `ENGINEERING.md`.

The document should become the engineering specification for repository initialization.

Avoid duplicating:

* project intent;
* roadmap;
* architecture.

---

# Rules

Do:

* derive engineering decisions from approved architecture;
* keep engineering conventions explicit;
* prefer simple tooling;
* distinguish accepted and deferred decisions;
* optimize for maintainability.

Do not:

* redefine project goals;
* redesign architecture;
* create implementation plans;
* generate production code;
* introduce technologies without justification.

Engineering Design translates architecture into engineering practice.

---

# Principles

Engineering decisions should be:

* explicit;
* maintainable;
* reproducible;
* architecture-driven;
* appropriate for the MVP;
* easy for humans and AI agents to follow.

Prefer the simplest engineering solution that satisfies the approved architecture.

---

# Success Criteria

The skill is complete when:

* `ENGINEERING.md` is complete;
* engineering conventions are documented;
* tooling is defined;
* repository structure is specified;
* validation workflow is documented;
* deferred engineering decisions are explicit;
* the document is sufficient for Repository Initialization;
* the human approves the engineering design.

---

# Handover

After Engineering Design is approved, continue with:

**Repository Initialization**

The Initialization Agent will materialize the approved engineering design into a repository that is ready for implementation planning.
