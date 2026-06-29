# Agent Roles

## Purpose

This directory defines reusable engineering roles for AI agents.

A role describes **who an agent is acting as** during a task.

Roles are independent of any specific AI tool or model.

They are intended to work with:

* Codex CLI
* Cursor
* Claude Code
* ChatGPT
* future AI coding agents

A role does **not** describe how to perform work.

Reusable engineering procedures are defined in `skills/`.

---

# Relationship to Skills

Roles and skills have different responsibilities.

A role defines:

* responsibilities;
* authority;
* expected inputs;
* expected outputs;
* decision boundaries.

A skill defines:

* execution procedure;
* engineering workflow;
* completion criteria.

Roles use skills.

Skills do not define roles.

---

# Engineering Model

The engineering workflow follows a simple hierarchy.

```text
Task
    ↓
Assigned Role
    ↓
Selected Skill
    ↓
Repository Artifacts
```

A task assigns an agent to a role.

The role determines which skill should be executed.

The skill produces or updates repository artifacts.

---

# Role Assignment

Roles are assigned explicitly by the task.

Agents must not infer or invent their own role.

Example:

```text
You are acting as the Planning Agent.

Use:

- skills/plan-creation/

Create the next implementation plan.
```

The task determines the role.

The role determines the skill.

---

# Repository Relationship

Roles do not replace repository documentation.

Before performing work, every role should follow the repository guidance defined in:

1. `AGENTS.md`
2. Project documentation
3. Relevant skills

Project documentation remains the authoritative source of project knowledge.

---

# Current Roles

This repository defines the following engineering roles:

| Role                 | Primary Responsibility                                    |
| -------------------- | --------------------------------------------------------- |
| Discovery Agent      | Build shared understanding and produce `PROJECT.md`       |
| Roadmap Agent        | Produce `ROADMAP.md` from the approved project definition |
| Architecture Agent   | Produce and evolve `ARCHITECTURE.md` and ADRs             |
| Planning Agent       | Produce implementation plans                              |
| Implementation Agent | Implement approved plans                                  |
| Review Agent         | Review plans and implementations                          |

Future roles may be added as the engineering process evolves.

---

# Design Principles

Roles should be:

* focused;
* reusable;
* tool-agnostic;
* clearly scoped;
* aligned with repository methodology.

Each role should have a single primary responsibility.

Avoid combining multiple engineering responsibilities into a single role.

---

# Relationship to AI Tools

The engineering methodology is independent of AI tooling.

Tool-specific configuration belongs outside this directory.

Examples:

```text
.cursor/
.codex/
.claude/
```

These directories adapt the methodology to specific tools.

The role definitions remain unchanged.

---

# Summary

Roles define **who performs the work**.

Skills define **how the work is performed**.

Repository documentation defines **what the project is**.

Together they provide a consistent, reusable engineering workflow that can be executed by different AI agents without changing the underlying methodology.
