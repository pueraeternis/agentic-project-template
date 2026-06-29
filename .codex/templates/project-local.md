# Project-Specific Codex Configuration

## Purpose

This document contains Codex-specific guidance for this repository.

It supplements the shared engineering methodology with project-specific instructions.

Do not duplicate information already documented in:

* `AGENTS.md`
* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`

Only record information that affects how Codex should work with this repository.

---

# Repository Overview

Briefly describe the repository.

Examples:

* application type;
* primary purpose;
* major technologies.

---

# Development Environment

Document project-specific development requirements.

Examples:

* dependency manager;
* runtime;
* package manager;
* build commands;
* local services.

---

# Project Conventions

Document repository-specific conventions.

Examples:

* directory layout;
* configuration style;
* naming conventions;
* logging conventions;
* dependency injection patterns.

Only include conventions that differ from the shared engineering framework.

---

# Validation Commands

Document the commands that Codex should execute before considering work complete.

Examples:

```bash
uv run ruff format --check .
uv run ruff check .
uv run basedpyright
uv run pytest
```

Include any project-specific validation commands.

---

# Repository Constraints

Document constraints that affect implementation.

Examples:

* supported Python version;
* deployment environment;
* compatibility requirements;
* infrastructure limitations.

---

# Codex Notes

Document any additional guidance specific to Codex.

Examples:

* preferred workflow;
* sandbox considerations;
* approval preferences;
* repository-specific execution rules.

Keep this section focused on Codex-specific behavior rather than general project documentation.
