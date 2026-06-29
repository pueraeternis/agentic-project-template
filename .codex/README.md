# Codex Integration

## Purpose

This directory contains Codex-specific configuration for repositories using the Agentic Engineering Methodology.

It adapts the shared engineering framework to Codex without duplicating repository documentation.

Repository knowledge remains in:

* `AGENTS.md`
* `docs/project/`
* `.agents/`
* `skills/`

This directory contains only Codex-specific configuration and prompts.

---

# Design Principles

The Codex configuration should:

* remain minimal;
* avoid duplicating repository documentation;
* reuse the shared engineering workflow;
* stay independent of any specific project.

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

## `config.toml`

Defines Codex runtime configuration.

Examples:

* model selection;
* approval mode;
* sandbox mode;
* subagent configuration.

Avoid storing repository knowledge here.

---

## `prompts/`

Contains reusable prompts for common engineering tasks.

Typical prompts include:

* implementation;
* plan creation;
* plan review;
* code review;
* repository audit.

Prompts should complement the engineering methodology rather than redefine it.

---

## `templates/`

Contains templates that are copied into new repositories during project bootstrap.

Templates are project-specific starting points rather than framework documentation.

---

# Relationship to Other Directories

## `AGENTS.md`

Repository entry point.

Defines repository workflow and documentation hierarchy.

---

## `.agents/`

Defines reusable engineering roles.

Examples:

* Planning Agent
* Review Agent
* Implementation Agent

---

## `skills/`

Defines reusable engineering procedures.

Examples:

* Project Discovery
* Roadmap Creation
* Architecture Design
* Plan Implementation

---

## `.cursor/`

Contains Cursor-specific rules.

Both `.cursor/` and `.codex/` implement the same engineering methodology for different coding assistants.

---

# Guiding Principle

The engineering methodology is tool-independent.

Codex should adapt to the methodology.

The methodology should not adapt to Codex.
