# Project Overview

## Purpose

This document captures the shared understanding of the project before implementation begins.

It defines:

* why the project exists;
* what will be built;
* who it serves;
* which problems it solves;
* what success looks like.

This document describes **project intent**, not implementation.

Architecture, engineering decisions, and implementation belong in later lifecycle stages.

---

# Project Context

Describe the background that led to the project.

Include:

* the original motivation;
* current problems;
* opportunities identified;
* observations from the discovery process.

This section explains why the project should exist.

---

# Core Idea

Describe the project in one or two concise paragraphs.

Answer:

> What is the fundamental idea behind this project?

Avoid discussing implementation.

---

# Vision

Describe the desired future state.

Explain:

* why this project matters;
* what value it should create;
* how success changes the current situation.

---

# Goals

List the primary project goals.

Goals describe what the project should achieve.

Examples:

* improve developer productivity;
* automate repetitive work;
* reduce operational complexity.

---

# Non-Goals

Explicitly define what is outside the project scope.

Clear non-goals reduce scope creep during implementation.

---

# Target Users

Describe the intended users.

For each user group describe:

* who they are;
* their needs;
* how the project helps them.

---

# Primary Use Cases

Describe the most important user scenarios.

Focus on desired outcomes rather than implementation.

Examples:

* create a new project;
* analyze repository architecture;
* execute implementation plans.

---

# Success Criteria

Describe what success means for the project.

Focus on outcomes rather than implementation details.

Examples:

* solves the intended problem;
* improves user workflow;
* achieves adoption goals;
* reduces operational effort.

Detailed acceptance criteria belong in implementation plans.

---

# MVP

Describe the smallest version of the project that delivers meaningful value.

Focus on:

* essential capabilities;
* required functionality;
* minimum user value.

Avoid describing future phases.

---

# Constraints

Describe known project constraints.

Examples:

* infrastructure;
* budget;
* deadlines;
* compatibility requirements;
* external dependencies;
* regulatory requirements.

---

# Assumptions

Document assumptions made during discovery.

Examples:

* expected user behavior;
* available infrastructure;
* technology availability;
* organizational assumptions.

These assumptions should be revisited if they become invalid.

---

# Risks

Describe known project risks.

Examples:

* technical uncertainty;
* organizational risk;
* external dependencies;
* adoption risk.

High-risk items may later become implementation plans or ADRs.

---

# Repository Relationships

This document is the foundation of the project lifecycle.

Subsequent documents build upon it.

| Document          | Relationship                                |
| ----------------- | ------------------------------------------- |
| `ROADMAP.md`      | Defines how the project evolves             |
| `ARCHITECTURE.md` | Defines how the system is organized         |
| `ENGINEERING.md`  | Defines how the project will be implemented |
| ADRs              | Record significant engineering decisions    |
| Plans             | Implement the project incrementally         |

---

# Change Management

Update this document only when project intent changes.

Examples:

* project goals;
* project scope;
* target users;
* success definition;
* major constraints.

Implementation progress should **not** modify this document.

Project intent should remain relatively stable throughout the project.

---

# Summary

This document answers the fundamental questions:

* Why does this project exist?
* What problem does it solve?
* Who is it for?
* What outcomes should it achieve?
* What is intentionally out of scope?

Everything else in the repository builds upon the shared understanding established here.
