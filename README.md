# Agentic Project Template

A reusable framework for building software with AI agents. The repository is the shared working memory where project intent, architecture, decisions, plans, and history live together — not just source code.

## What This Is

This repository provides a **documentation-first engineering methodology** for human–AI collaboration. It defines how to organize project knowledge, authorize implementation work, record architectural decisions, and preserve traceability over time.

It is a **template**, not a finished application. Copy or fork it, then populate `docs/project/` with your own project artifacts using the templates in `docs/templates/`.

## Who This Is For

- **Engineering leads and architects** who want structured, traceable development with AI assistance
- **Developers** starting a new project and wanting a clear documentation workflow from day one
- **Teams** that use Cursor, Codex, Claude Code, or other AI coding agents and need a tool-agnostic process
- **Anyone** who has lost context in chat history and wants durable project memory in the repository

## Core Idea

Chat history is temporary. Agent memory is unreliable. Human memory is incomplete.

**The repository is the durable place where knowledge must converge.**

Documentation drives implementation. Plans authorize change. Architecture evolves intentionally. Validation is part of the work — not an afterthought.

For the full philosophy, see [METHODOLOGY.md](METHODOLOGY.md).

## Repository Structure

```text
.
├── README.md              # Human entry point (start here)
├── AGENTS.md              # Rules for AI agents
├── REPOSITORY_MAP.md      # Navigation guide for all knowledge
├── METHODOLOGY.md         # Engineering principles
├── KNOWLEDGE_MODEL.md     # How knowledge is organized
│
├── docs/
│   ├── project/           # Your project-specific documentation
│   │   ├── adr/           # Architecture Decision Records
│   │   └── plans/         # backlog / active / completed
│   └── templates/         # Reusable document templates
│
└── skills/                # Reusable engineering procedures for agents
```

| Location | Purpose |
|----------|---------|
| Root `.md` files | Framework rules, methodology, and navigation |
| `docs/templates/` | Blank structures to copy into `docs/project/` |
| `docs/project/` | Living project knowledge (vision, roadmap, architecture, plans, ADRs) |
| `skills/` | Step-by-step workflows (discovery, planning, implementation, review) |

For detailed navigation, see [REPOSITORY_MAP.md](REPOSITORY_MAP.md).

## Minimal Workflow

A typical project follows this flow:

```text
Idea
  → PROJECT.md          (what and why)
  → ROADMAP.md          (phases and delivery strategy)
  → ARCHITECTURE.md     (system structure and boundaries)
  → Implementation Plan (authorized scope in plans/active/)
  → Implementation
  → Validation
  → PROGRESS.md         (record what was completed)
```

Architectural decisions can happen at any stage and are recorded as ADRs in `docs/project/adr/`.

Key rules:

1. **Clarify before coding** — shared understanding precedes implementation
2. **Only implement active plans** — plans in `plans/active/` define the current boundary
3. **Keep the repository consistent** — update documentation when intent or architecture changes
4. **Record significant decisions** — use ADRs for choices that affect future work

## Where to Start

### Using this template for a new project

1. Copy templates from `docs/templates/` into `docs/project/` (e.g. `PROJECT.md`, `ROADMAP.md`, `ARCHITECTURE.md`)
2. Fill in `PROJECT.md` with vision, goals, scope, and non-goals
3. Define phases in `ROADMAP.md`
4. Create your first implementation plan in `docs/project/plans/active/` using the plan template
5. Point your AI agent at `AGENTS.md` so it follows repository conventions

### Joining an existing project that uses this framework

Read in this order:

1. [AGENTS.md](AGENTS.md) — agent and contributor rules
2. [REPOSITORY_MAP.md](REPOSITORY_MAP.md) — where everything lives
3. [METHODOLOGY.md](METHODOLOGY.md) — engineering principles
4. [KNOWLEDGE_MODEL.md](KNOWLEDGE_MODEL.md) — knowledge hierarchy
5. `docs/project/PROJECT.md` — what the project is building
6. `docs/project/ROADMAP.md` — current direction
7. Active plans in `docs/project/plans/active/`

### For AI agents

Start with [AGENTS.md](AGENTS.md), then follow the read-first order defined there.

## Further Reading

| Document | Description |
|----------|-------------|
| [METHODOLOGY.md](METHODOLOGY.md) | Core engineering principles |
| [KNOWLEDGE_MODEL.md](KNOWLEDGE_MODEL.md) | Conceptual model of repository knowledge |
| [REPOSITORY_MAP.md](REPOSITORY_MAP.md) | Complete navigation guide |
| [AGENTS.md](AGENTS.md) | Universal rules for AI agents |
