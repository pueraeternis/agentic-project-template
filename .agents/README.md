# Agent Roles

## Purpose

This directory defines reusable engineering roles for AI agents.

A role defines **who an agent is** within the engineering process.

Roles are independent of AI models, IDEs, and coding tools.

They describe responsibilities, decision boundaries, and expected outputs.

Execution procedures are defined separately as reusable skills.

---

# Roles and Skills

Roles and skills serve different purposes.

A **role** defines:

* responsibilities;
* authority;
* decision boundaries;
* expected inputs;
* expected outputs.

A **skill** defines:

* execution procedure;
* lifecycle stage;
* engineering workflow;
* completion criteria.

Roles perform work.

Skills describe how that work is performed.

---

# Engineering Model

Projects follow a lifecycle.

Each lifecycle stage is executed by a specialized role using a corresponding skill.

```text
Task
        ↓
Lifecycle Stage
        ↓
Assigned Role
        ↓
Selected Skill
        ↓
Repository Artifacts
```

This separation keeps engineering workflows reusable while allowing different AI tools to execute the same methodology.

---

# Repository Relationship

Roles never replace repository documentation.

Before performing work, every role should read:

1. `AGENTS.md`
2. Project documentation
3. Relevant skills

Repository documentation remains the authoritative source of project knowledge.

---

# Current Roles

| Role                 | Primary Responsibility                              |
| -------------------- | --------------------------------------------------- |
| Discovery Agent      | Produce `PROJECT.md`                                |
| Roadmap Agent        | Produce `ROADMAP.md`                                |
| Architecture Agent   | Produce `ARCHITECTURE.md` and ADRs                  |
| Engineering Agent    | Produce `ENGINEERING.md`                            |
| Initialization Agent | Initialize a repository from approved documentation |
| Planning Agent       | Produce implementation plans                        |
| Implementation Agent | Implement approved plans                            |
| Review Agent         | Review plans and implementation                     |

Each role has a single primary responsibility.

---

# Lifecycle Mapping

| Lifecycle Stage           | Role                 | Primary Artifact       |
| ------------------------- | -------------------- | ---------------------- |
| Project Discovery         | Discovery Agent      | `PROJECT.md`           |
| Roadmap Creation          | Roadmap Agent        | `ROADMAP.md`           |
| Architecture Design       | Architecture Agent   | `ARCHITECTURE.md`      |
| Engineering Design        | Engineering Agent    | `ENGINEERING.md`       |
| Repository Initialization | Initialization Agent | Initialized repository |
| Plan Creation             | Planning Agent       | `PLAN.md`              |
| Plan Review               | Review Agent         | Reviewed plan          |
| Plan Implementation       | Implementation Agent | Source code            |
| Code Review               | Review Agent         | Review report          |

---

# Role Assignment

Roles are assigned explicitly by the current task.

Agents should not invent or switch roles during execution.

Example:

```text
You are acting as the Planning Agent.

Use:

skills/plan-creation/

Create the next implementation plan.
```

The task determines the role.

The role selects the appropriate skill.

The skill produces repository artifacts.

---

# Design Principles

Roles should be:

* focused;
* reusable;
* tool-independent;
* clearly scoped;
* aligned with the project lifecycle.

Avoid combining multiple engineering responsibilities into a single role.

---

# Tool Independence

Role definitions are independent of AI tools.

Tool-specific adaptation belongs in dedicated configuration directories such as:

```text
.cursor/
.codex/
```

The engineering methodology remains unchanged regardless of the execution environment.

---

# Summary

Roles define **who performs the work**.

Skills define **how the work is performed**.

Project documentation defines **what is being built**.

Together they form a reusable engineering framework that enables consistent collaboration between humans and AI agents across different tools and projects.
