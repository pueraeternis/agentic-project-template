# Repository Map

## Purpose

This document is the navigation guide for the repository.

It explains where information lives, how repository knowledge is organized, and which documents should be used at each stage of the project lifecycle.

Use this document whenever you need to locate project information.

---

# Repository Organization

The repository consists of six major areas.

```text
.
├── Framework Documentation
├── Project Documentation
├── Skills
├── Agents
├── Tool Configuration
└── Templates
```

Each area has a single responsibility.

---

# Framework Documentation

Located in the repository root.

These documents define the framework itself.

| Document             | Purpose                    |
| -------------------- | -------------------------- |
| `README.md`          | Framework overview         |
| `AGENTS.md`          | Universal AI agent rules   |
| `METHODOLOGY.md`     | Development methodology    |
| `KNOWLEDGE_MODEL.md` | Repository knowledge model |
| `REPOSITORY_MAP.md`  | Repository navigation      |
| `VERSION.md`         | Framework version          |

These documents rarely change.

---

# Project Documentation

Location:

```text
docs/project/
```

These documents describe one specific software project.

Typical contents:

```text
PROJECT.md
ROADMAP.md
ARCHITECTURE.md
ENGINEERING.md
RUNBOOK.md
PROGRESS.md
adr/
plans/
```

---

## Project Design Documents

Created before implementation begins.

| Document          | Purpose                  |
| ----------------- | ------------------------ |
| `PROJECT.md`      | Project vision and scope |
| `ROADMAP.md`      | Delivery roadmap         |
| `ARCHITECTURE.md` | System architecture      |
| `ENGINEERING.md`  | Engineering decisions    |

---

## Project Execution Documents

Created during implementation.

| Document      | Purpose                       |
| ------------- | ----------------------------- |
| `RUNBOOK.md`  | Operational procedures        |
| `PROGRESS.md` | Completed work                |
| `adr/`        | Architecture Decision Records |
| `plans/`      | Implementation plans          |

---

# Skills

Location:

```text
skills/
```

Skills describe reusable engineering workflows.

Current lifecycle skills:

* Project Discovery
* Roadmap Creation
* Architecture Design
* Engineering Design
* Repository Initialization
* Plan Creation
* Plan Review
* Plan Implementation
* Code Review

Skills are reusable across projects.

---

# Agents

Location:

```text
.agents/
```

Agents specialize in executing skills.

Each agent is responsible for one engineering workflow.

Agents do not define methodology.

They execute it.

---

# Tool Configuration

Tool-specific configuration lives outside the framework documentation.

Examples:

```text
.cursor/
.codex/
```

These directories contain:

* shared framework configuration;
* project-local configuration;
* prompts;
* templates.

Tool-specific rules should never replace repository documentation.

---

# Templates

Location:

```text
docs/templates/
```

Templates define reusable project documents.

Typical templates:

* PROJECT
* ROADMAP
* ARCHITECTURE
* ENGINEERING
* PLAN
* ADR
* RUNBOOK
* PROGRESS

Templates define document structure only.

---

# Repository Lifecycle

Projects move through the following lifecycle.

```text
Idea
        ↓
PROJECT
        ↓
ROADMAP
        ↓
ARCHITECTURE
        ↓
ENGINEERING
        ↓
Repository Initialization
        ↓
Implementation Plans
        ↓
Implementation
        ↓
Progress
```

Each stage creates repository knowledge for the next stage.

---

# Read Order

## Repository Onboarding

Read:

1. `README.md`
2. `REPOSITORY_MAP.md`
3. `METHODOLOGY.md`
4. `KNOWLEDGE_MODEL.md`
5. `AGENTS.md`

---

## Project Onboarding

Read:

1. `PROJECT.md`
2. `ROADMAP.md`
3. `ARCHITECTURE.md`
4. `ENGINEERING.md`
5. Relevant ADRs
6. Active plans
7. `PROGRESS.md`

---

## Implementation

During implementation consult:

* active plans;
* relevant ADRs;
* engineering documentation.

Follow the read order defined in `AGENTS.md`.

---

# Repository Principles

The repository is organized around the following principles:

* one responsibility per document;
* one source of truth for every piece of knowledge;
* documentation before implementation;
* reusable engineering workflows;
* explicit project lifecycle;
* long-term maintainability.

The repository should remain understandable to both humans and AI agents throughout the lifetime of the project.
