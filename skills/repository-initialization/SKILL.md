# Repository Initialization

## Purpose

This skill transforms approved project documentation into a repository that is ready for implementation.

Repository Initialization does **not** design or implement the project.

Instead, it materializes the approved project and engineering decisions into a consistent repository structure.

The result is a repository ready for the first implementation plan.

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
        ↓
Repository Initialization
        ↓
Plan Creation
```

Repository Initialization is the bridge between project design and implementation.

---

# Role

Primary role:

**Initialization Agent**

---

# When to Use

Use this skill when:

* `PROJECT.md` has been approved;
* `ROADMAP.md` has been approved;
* `ARCHITECTURE.md` has been approved;
* `ENGINEERING.md` has been approved;
* a new project repository is being initialized.

Normally this skill is executed once.

It may later be executed again to synchronize repository metadata without modifying implementation artifacts.

Do not use this skill for:

* architecture design;
* engineering design;
* implementation planning;
* production code;
* dependency installation;
* runtime bootstrap.

---

# Inputs

Required:

* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`
* `ENGINEERING.md`

Additional inputs:

* framework templates;
* framework rules;
* repository skeleton.

Repository Initialization must never invent missing project decisions.

---

# Outputs

Produce an initialized repository by:

* generating project documentation from templates;
* generating project-local Cursor configuration;
* generating project-local Codex configuration;
* generating operational documentation;
* synchronizing repository metadata;
* validating repository structure.

No production source code should be generated.

---

# Procedure

## Step 1 — Validate Project Design

Verify that all required project documentation exists and is approved:

* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`
* `ENGINEERING.md`

Stop immediately if project design is incomplete.

---

## Step 2 — Materialize Documentation

Generate project-specific documents from templates.

Typical outputs:

* `README.md`
* `RUNBOOK.md`

Populate templates using approved project documentation.

---

## Step 3 — Generate Tool Configuration

Generate project-local configuration for supported AI tools.

Examples:

```text
.cursor/templates/90-project-local.mdc

.codex/templates/project-local.md
```

Only project-specific rules should be generated.

Framework rules remain unchanged.

---

## Step 4 — Synchronize Repository Structure

Create or verify:

* documentation directories;
* repository layout;
* project metadata;
* framework integration files.

Do not create implementation code.

---

## Step 5 — Validate Initialization

Verify that:

* required documentation exists;
* generated documentation is consistent;
* project-local rules exist;
* repository structure matches Engineering Design.

The repository should now be ready for implementation planning.

---

# Rules

During Repository Initialization:

Do:

* materialize approved project decisions;
* generate repository artifacts;
* synchronize documentation;
* preserve framework integrity.

Do not:

* redesign the project;
* modify architecture;
* invent engineering decisions;
* install dependencies;
* initialize runtime environments;
* generate production code.

Repository Initialization prepares the repository.

Implementation begins afterwards.

---

# Principles

Repository Initialization should be:

* deterministic;
* repeatable;
* idempotent;
* documentation-driven;
* implementation-independent.

Running the skill multiple times should synchronize repository metadata without damaging existing implementation work.

---

# Success Criteria

The skill is complete when:

* required project documentation exists;
* project artifacts have been generated;
* project-local AI tool configuration has been generated;
* repository structure is synchronized;
* repository metadata is consistent;
* the repository is ready for Plan Creation.

No implementation artifacts should be produced.

---

# Handover

After Repository Initialization is complete, continue with:

**Plan Creation**

The repository is now synchronized with the approved project documentation and ready for incremental implementation through engineering plans.
