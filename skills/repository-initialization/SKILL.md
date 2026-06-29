# Repository Initialization

## Purpose

This skill transforms approved project documentation into a repository that is ready for implementation.

Repository Initialization does not implement the project.

Instead, it synchronizes the repository with the approved engineering decisions and prepares it for the first implementation plan.

The output of this skill is an initialized repository that is ready for development.

---

## Role

Initialization Agent

---

## When to Use

Use this skill when:

- `PROJECT.md` has been approved;
- `ROADMAP.md` has been approved;
- `ARCHITECTURE.md` has been approved;
- `ENGINEERING.md` has been approved;
- a new project repository is being initialized.

This skill is normally executed once at the beginning of a project.

It may be executed again later to synchronize repository metadata and documentation, provided no implementation artifacts are overwritten.

Do not use this skill for:

- implementation planning;
- writing production code;
- repository bootstrap;
- dependency installation;
- project implementation.

---

## Inputs

The skill requires:

- approved `PROJECT.md`;
- approved `ROADMAP.md`;
- approved `ARCHITECTURE.md`;
- approved `ENGINEERING.md`;
- repository framework templates.

All engineering decisions should already be documented.

Repository Initialization must not invent missing decisions.

---

## Outputs

The skill produces an initialized repository by:

- creating project documentation from templates;
- creating project-local Cursor rules;
- creating project-local Codex rules;
- creating project operational documentation;
- synchronizing repository metadata;
- validating repository structure.

The repository should be ready for the first implementation plan.

---

## Procedure

### Step 1 — Validate Project Documentation

Verify that the following documents exist and have been approved:

- `PROJECT.md`
- `ROADMAP.md`
- `ARCHITECTURE.md`
- `ENGINEERING.md`

Stop if required project documentation is missing.

Repository Initialization never invents missing project information.

---

### Step 2 — Create Project Documentation

Generate project-specific documentation from repository templates.

Examples:

- `README.md`
- `RUNBOOK.md`

Populate templates using the approved project documentation.

---

### Step 3 — Create Project Rules

Generate project-local development rules.

Examples:

- `.cursor/rules/90-project-local.mdc`
- `.codex/project-local.md`

Only include project-specific conventions.

Global framework rules remain unchanged.

---

### Step 4 — Synchronize Repository Structure

Verify that the repository structure matches the approved architecture.

Create missing documentation directories when required.

Do not generate implementation code.

---

### Step 5 — Validate Repository

Verify that:

- required documentation exists;
- repository structure is complete;
- generated project rules exist;
- project metadata is consistent.

The repository should be ready for implementation planning.

---

## Rules

During Repository Initialization:

- synchronize the repository with approved documentation;
- never invent project decisions;
- never redesign architecture;
- never modify project goals;
- never implement production code;
- never install dependencies;
- never bootstrap the runtime environment;
- never create implementation artifacts.

Repository Initialization prepares the repository.

Implementation begins later.

---

## Initialization Principles

Repository Initialization should be:

- deterministic;
- repeatable;
- idempotent;
- documentation-driven;
- implementation-independent.

Running the skill multiple times should update repository metadata without damaging existing implementation work.

---

## Success Criteria

The skill is complete when:

- required project documents exist;
- project documentation has been generated;
- project-local rules have been created;
- repository structure is synchronized;
- the repository is ready for Plan Creation.

No production code should be generated.

---

## Next Skill

After Repository Initialization is complete, continue with:

**Plan Creation**