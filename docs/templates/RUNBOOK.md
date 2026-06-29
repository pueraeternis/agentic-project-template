# Runbook

## Purpose

This document describes the operational procedures for the project.

It explains how to prepare the development environment, configure the system, run its components, validate changes, troubleshoot common issues, and safely operate the project.

Unlike architecture documentation, the runbook focuses on **how to operate the system**, not **how the system is designed**.

---

# Current State

Describe the current operational state of the project.

Examples:

* development only;
* local runtime available;
* production deployment available;
* background workers implemented;
* API available.

This section helps contributors understand which operational procedures are currently relevant.

---

# Environment Setup

Describe how to prepare a development environment.

Include:

* required software;
* package manager;
* dependency installation;
* virtual environment (if applicable);
* local services required for development.

Do not duplicate information already maintained elsewhere.

Reference other documentation when appropriate.

---

# Configuration

Describe how the project is configured.

Examples include:

* environment variables;
* configuration files;
* secrets management;
* local configuration overrides.

Never store credentials or secrets in this document.

Document only how configuration should be provided.

---

# Runtime Components

Describe the executable parts of the system.

Examples:

* API server;
* CLI;
* background workers;
* schedulers;
* MCP servers;
* web frontend.

For each component describe:

* purpose;
* how to start it;
* required dependencies.

---

# Validation Commands

Describe the commands required to verify the project.

Typical examples include:

* formatting;
* linting;
* type checking;
* unit tests;
* integration tests;
* build verification.

This section should provide the standard validation workflow for contributors.

---

# State and Persistence

Describe where operational state is stored.

Examples:

* local databases;
* generated files;
* cache directories;
* workflow state;
* uploaded assets.

Explain which data is persistent and which data may be safely deleted.

---

# Reset Procedures

Describe how to safely reset the development environment.

Examples:

* removing temporary state;
* recreating local databases;
* clearing caches;
* regenerating derived artifacts.

Reset procedures should never require reading implementation code.

---

# Operational Procedures

Document common operational tasks.

Examples:

* running background jobs;
* importing data;
* rebuilding indexes;
* rotating logs;
* refreshing generated artifacts.

Each procedure should contain only the information necessary to perform the operation safely.

---

# Troubleshooting

Document common operational issues.

For each issue include:

* symptoms;
* likely causes;
* diagnostic steps;
* resolution.

Keep troubleshooting concise and actionable.

---

# Incident Principles

Describe general operational principles.

Examples:

* investigate before restarting services;
* preserve logs before cleanup;
* avoid modifying production data without approval;
* verify system state before retrying failed operations.

These principles should remain stable throughout the project.

---

# Related Documents

Reference relevant project documentation.

Typical references include:

* `PROJECT.md`
* `ROADMAP.md`
* `ARCHITECTURE.md`
* `PROGRESS.md`
* relevant ADRs
* active implementation plans

The runbook complements those documents by describing how to operate the system rather than how it is designed.

---

# Success Criteria

A runbook is successful when a contributor can:

* prepare the development environment;
* configure the project correctly;
* start all runtime components;
* validate changes;
* reset the local environment safely;
* diagnose common operational problems;

without relying on chat history or undocumented tribal knowledge.
