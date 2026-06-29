# Runbook

## Purpose

This document describes how to operate the project.

It explains how to:

* prepare the development environment;
* configure the system;
* run project components;
* validate changes;
* perform common operational tasks;
* troubleshoot operational issues.

Unlike `ENGINEERING.md`, this document focuses on **operating the project**, not **designing or implementing it**.

---

# Relationship to the Project Lifecycle

The runbook evolves alongside implementation.

Typical lifecycle:

```text
PROJECT
        ↓
ENGINEERING
        ↓
IMPLEMENTATION
        ↓
RUNBOOK
```

As new operational procedures appear, they should be documented here.

---

# Current State

Describe the current operational maturity of the project.

Examples:

* development only;
* local runtime available;
* production deployment supported;
* background workers available;
* API available;
* monitoring implemented.

This section helps contributors understand which operational procedures are currently relevant.

---

# Environment Setup

Describe how to prepare a development environment.

Include:

* required software;
* dependency manager;
* virtual environment;
* local services;
* installation steps.

Reference other documentation instead of duplicating information.

---

# Configuration

Describe runtime configuration.

Typical topics:

* environment variables;
* configuration files;
* secrets management;
* local overrides.

Never include credentials or secrets.

---

# Runtime Components

Describe executable components.

Examples:

* API server;
* CLI;
* workers;
* schedulers;
* MCP servers;
* frontend.

For each component describe:

* purpose;
* startup procedure;
* dependencies.

---

# Validation Commands

Describe the standard validation workflow.

Typical examples:

* formatting;
* linting;
* type checking;
* tests;
* build verification.

This section should provide the commands contributors run before considering work complete.

---

# Operational State

Describe persistent operational state.

Examples:

* databases;
* caches;
* generated artifacts;
* uploaded files;
* indexes;
* workflow state.

Clearly distinguish between persistent and disposable state.

---

# Reset Procedures

Describe how to safely reset the local environment.

Examples:

* recreate databases;
* remove generated artifacts;
* clear caches;
* rebuild indexes;
* reset local state.

Contributors should not need to inspect implementation code to perform a reset.

---

# Operational Procedures

Document recurring operational tasks.

Examples:

* running background jobs;
* importing data;
* rebuilding indexes;
* rotating logs;
* refreshing generated artifacts;
* deployment preparation.

Each procedure should contain only the information required to perform the operation safely.

---

# Troubleshooting

Document common operational problems.

For each issue describe:

* symptoms;
* likely causes;
* diagnostic steps;
* resolution.

Keep troubleshooting concise and actionable.

---

# Operational Principles

Examples:

* investigate before restarting services;
* preserve logs before cleanup;
* verify system state before retrying;
* avoid destructive operations without approval;
* validate changes after operational procedures.

These principles should remain stable throughout the project.

---

# Repository Relationships

| Document          | Purpose                              |
| ----------------- | ------------------------------------ |
| `PROJECT.md`      | Defines why the project exists       |
| `ARCHITECTURE.md` | Describes system structure           |
| `ENGINEERING.md`  | Describes implementation conventions |
| Plans             | Describe implementation work         |
| `PROGRESS.md`     | Records completed milestones         |

The runbook complements these documents by describing how to operate the project after it has been implemented.

---

# Change Management

Update this document whenever operational procedures change.

Examples:

* new runtime component;
* deployment changes;
* configuration changes;
* validation workflow changes;
* operational troubleshooting;
* reset procedures.

Do not update the runbook for architectural or implementation changes unless they affect project operation.

---

# Success Criteria

A runbook is successful when a contributor can:

* prepare the development environment;
* configure the project;
* start every runtime component;
* validate changes;
* reset the local environment safely;
* troubleshoot common operational issues;

without relying on chat history or undocumented tribal knowledge.

---

# Summary

The runbook is the operational guide for the project.

It answers questions such as:

* How do I run the project?
* How do I configure it?
* How do I validate my changes?
* How do I recover from common operational problems?

Operational knowledge should become part of the runbook rather than remaining in conversations or personal notes.
