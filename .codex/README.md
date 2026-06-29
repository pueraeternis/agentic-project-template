# Codex Integration

## Purpose

This directory contains Codex-specific configuration for repositories using the Agentic Engineering Methodology.

Its purpose is to adapt Codex to the repository engineering workflow without duplicating repository knowledge.

The repository remains the authoritative source of project knowledge.

---

# Repository Knowledge

Project knowledge lives outside `.codex`.

Repository artifacts remain authoritative:

* `AGENTS.md`
* `docs/project/`
* `.agents/`
* `skills/`

Codex configuration should reference these artifacts rather than redefine them.

---

# Design Principles

The Codex integration should be:

* minimal;
* documentation-driven;
* tool-specific only where necessary;
* reusable across repositories.

Whenever possible, repository documentation should be preferred over Codex-specific instructions.

---

# Directory Structure

```text
.codex/
├── README.md
├── config.toml
├── prompts/
└── templates/
```

---

## config.toml

Contains Codex runtime configuration.

Typical examples include:

* model selection;
* approval policy;
* sandbox configuration;
* subagent configuration.

Do not store repository knowledge here.

---

## prompts/

Reusable prompts for common engineering tasks.

Examples:

* implementation;
* plan creation;
* plan review;
* code review;
* repository audit.

Prompts should invoke the repository workflow rather than replace it.

---

## templates/

Templates copied into newly initialized repositories.

Examples:

* project-local Codex configuration;
* project bootstrap files.

Templates should contain project-specific starting points rather than framework documentation.

---

# Relationship to the Engineering Framework

The engineering workflow is defined by the repository.

Typical execution flow:

```text
User Request
        ↓
Role (.agents/)
        ↓
Skill (skills/)
        ↓
Repository Documentation
        ↓
Codex Prompt (optional)
        ↓
Implementation
```

Codex prompts support the workflow.

They do not define it.

---

# Relationship to Other Directories

| Location        | Responsibility                  |
| --------------- | ------------------------------- |
| `AGENTS.md`     | Repository rules and read order |
| `.agents/`      | Engineering roles               |
| `skills/`       | Engineering procedures          |
| `docs/project/` | Project knowledge               |
| `.cursor/`      | Cursor-specific integration     |
| `.codex/`       | Codex-specific integration      |

Each directory has a single responsibility.

Avoid duplicating information between them.

---

# Guiding Principle

The engineering methodology is tool-independent.

Codex adapts to the methodology.

The methodology never adapts to Codex.
