# Project Discovery

## Purpose

This skill guides a collaborative discovery process between the human and the AI agent.

Its objective is to establish a shared understanding of the project before architecture or implementation begins.

Project Discovery produces the foundation for all subsequent engineering work.

---

# Lifecycle Stage

```text
Idea
        ↓
Project Discovery
        ↓
Roadmap Creation
```

Project Discovery defines **what should be built**.

It intentionally avoids defining **how it will be implemented**.

---

# Role

Primary role:

**Discovery Agent**

---

# When to Use

Use this skill when:

* starting a new project;
* evaluating a new idea;
* defining an MVP;
* clarifying project scope;
* exploring requirements.

Do not use this skill for:

* architecture design;
* engineering decisions;
* implementation planning;
* repository initialization;
* production code.

---

# Inputs

Discovery may begin with any amount of information.

Typical inputs include:

* an initial idea;
* business goals;
* user discussions;
* existing systems;
* constraints;
* assumptions;
* desired outcomes.

Inputs may be incomplete.

A major purpose of this skill is discovering the missing information.

---

# Outputs

Produce:

* `PROJECT.md`

Optionally identify engineering assumptions that will later become inputs for `ENGINEERING.md`.

The discovery process should produce sufficient understanding for roadmap creation.

---

# Procedure

## Step 1 — Understand the Problem

Identify:

* the problem;
* target users;
* expected value;
* project motivation.

Focus entirely on understanding.

---

## Step 2 — Build Shared Understanding

Work collaboratively.

The agent should:

* ask clarifying questions;
* challenge assumptions;
* simplify ideas;
* identify risks;
* refine project boundaries.

Avoid technical implementation discussions.

---

## Step 3 — Define the MVP

Identify the smallest version that delivers meaningful value.

Clearly distinguish:

* MVP;
* future capabilities.

Remove unnecessary scope.

---

## Step 4 — Define Project Boundaries

Document:

* goals;
* non-goals;
* assumptions;
* constraints;
* risks;
* open questions.

Not every uncertainty must be resolved during discovery.

---

## Step 5 — Capture Engineering Assumptions

When obvious engineering decisions are already known, record them as assumptions for future Engineering Design.

Examples:

* primary programming language;
* deployment environment;
* expected technology stack;
* runtime assumptions.

Do not fully design the engineering solution.

Simply preserve knowledge discovered during discussion.

---

## Step 6 — Produce PROJECT.md

Populate the project template.

The document should capture the agreed understanding rather than the discussion itself.

---

# Rules

During Project Discovery:

Do:

* understand the problem;
* clarify goals;
* identify users;
* define MVP;
* identify risks;
* identify assumptions.

Do not:

* design the architecture;
* define repository structure;
* choose engineering tooling in detail;
* create implementation plans;
* write production code.

---

# Principles

Discovery should:

* prioritize understanding over design;
* challenge assumptions constructively;
* simplify rather than expand scope;
* defer implementation decisions;
* converge toward shared understanding.

The objective is clarity, not technical completeness.

---

# Success Criteria

The skill is complete when:

* project goals are clear;
* MVP is defined;
* project boundaries are understood;
* assumptions are documented;
* risks are identified;
* `PROJECT.md` has been approved.

---

# Handover

After Project Discovery is complete, continue with:

**Roadmap Creation**

Engineering assumptions identified during discovery become useful inputs for later Engineering Design but should not replace it.
