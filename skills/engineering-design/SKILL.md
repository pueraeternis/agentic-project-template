# Engineering Design

## Purpose

This skill transforms an approved project architecture into concrete engineering decisions.

The primary outcome is a completed `ENGINEERING.md` that defines how the project will be implemented from an engineering perspective.

Engineering Design bridges system architecture and repository initialization.

It defines the project-specific engineering environment, tooling, conventions, runtime assumptions, validation commands, and implementation constraints.

---

## Role

Engineering Agent

---

## When to Use

Use this skill when:

* `PROJECT.md` has been approved;
* `ROADMAP.md` has been approved;
* `ARCHITECTURE.md` has been approved;
* the repository needs project-specific engineering decisions before initialization;
* implementation tooling or conventions need to be defined or revised.

Do not use this skill for:

* project discovery;
* roadmap creation;
* architecture design;
* repository initialization;
* implementation planning;
* production code implementation.

---

## Inputs

The skill requires:

* approved `PROJECT.md`;
* approved `ROADMAP.md`;
* approved `ARCHITECTURE.md`;
* relevant ADRs, if any;
* known project constraints;
* known development environment constraints.

The architecture should already be stable enough to guide engineering decisions.

---

## Outputs

The skill produces:

* completed or updated `ENGINEERING.md`;
* selected language and runtime versions;
* dependency management decisions;
* quality tooling decisions;
* validation commands;
* repository layout conventions;
* testing strategy;
* configuration strategy;
* operational assumptions;
* deferred engineering decisions.

The output should provide enough project-specific information for Repository Initialization.

---

## Procedure

### Step 1 — Build Project Context

Review:

* `PROJECT.md`;
* `ROADMAP.md`;
* `ARCHITECTURE.md`;
* relevant ADRs;
* known project constraints.

Understand:

* what is being built;
* how the system is organized;
* which capabilities are required in the MVP;
* which architectural boundaries must be supported;
* which engineering constraints are already known.

Engineering decisions should support documented project intent and architecture.

---

### Step 2 — Define Runtime and Tooling

Select and document:

* primary language;
* target runtime version;
* dependency manager;
* formatter;
* linter;
* type checker;
* test framework;
* build tools, if applicable.

Prefer simple, stable, widely supported tooling.

Avoid introducing tools without clear project value.

---

### Step 3 — Define Project Technology Stack

Document project technologies such as:

* web framework;
* agent framework;
* MCP framework;
* LLM provider or serving approach;
* database;
* vector database;
* queue or workflow engine;
* frontend framework;
* configuration library;
* logging approach.

Only include technologies that are already justified by the project architecture or near-term roadmap.

Defer speculative technology choices.

---

### Step 4 — Define Repository Layout

Describe the expected repository layout.

Include:

* source directory;
* test directory;
* configuration files;
* documentation locations;
* generated artifact locations;
* runtime or deployment files if known.

The layout should be specific enough for repository initialization but should not overdefine future implementation details.

---

### Step 5 — Define Validation Strategy

Document required validation commands and expectations.

Examples:

* formatting;
* linting;
* type checking;
* unit tests;
* integration tests;
* build checks.

Validation should match the selected tooling and project constraints.

---

### Step 6 — Define Configuration and Operational Assumptions

Document:

* configuration sources;
* environment variable conventions;
* secrets handling;
* local development assumptions;
* deployment assumptions;
* state and persistence assumptions.

Operational details that require executable procedures may later be expanded in `RUNBOOK.md`.

---

### Step 7 — Identify Deferred Engineering Decisions

Record engineering decisions that are intentionally postponed.

Examples:

* CI/CD platform;
* deployment infrastructure;
* observability stack;
* production database choice;
* packaging and release strategy.

Deferred decisions should be explicit so future agents do not invent them prematurely.

---

### Step 8 — Produce ENGINEERING.md

Populate the engineering template.

The document should be concrete enough for repository initialization while remaining easy to revise as implementation evolves.

Do not duplicate architecture documentation.

Do not include product vision content.

---

## Rules

During Engineering Design:

* derive decisions from `PROJECT.md`, `ROADMAP.md`, and `ARCHITECTURE.md`;
* prefer simple and maintainable tooling;
* document project-specific engineering conventions;
* distinguish accepted decisions from deferred decisions;
* avoid speculative technology choices;
* avoid unnecessary infrastructure;
* keep implementation details out unless needed for repository initialization.

Do not:

* redefine project goals;
* rewrite the roadmap;
* redesign the architecture;
* create implementation plans;
* implement code;
* introduce tools only because they are popular.

---

## Engineering Principles

Engineering decisions should be:

* explicit;
* justified;
* maintainable;
* aligned with architecture;
* suitable for the MVP;
* easy for agents and humans to follow.

Prefer the simplest tooling and repository structure that supports the approved architecture.

Add complexity only when it is justified by documented project requirements.

---

## Success Criteria

The skill is complete when:

* `ENGINEERING.md` is completed or updated;
* language and runtime decisions are documented;
* tooling choices are documented;
* repository layout conventions are defined;
* validation commands are documented;
* configuration strategy is documented;
* deferred engineering decisions are explicit;
* the human approves the resulting engineering design.

---

## Next Skill

After Engineering Design is complete, continue with:

**Repository Initialization**
