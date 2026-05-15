# Project Index — Project Execution OS

## Repository

`oleg3479881328-code/2TestAgents`

## Project Name

Project Execution OS

## Project Type

Universal document-first project execution system.

## Core Definition

Project Execution OS is a universal workflow system for guiding any project from raw input to reviewed result and reusable knowledge extraction.

It is not limited to software projects, AI agents, AI skills, Codex workflows, or automation systems.

## System Hierarchy

```text
Project Execution OS
  ├── Workflow System
  ├── Agent System
  ├── AI Skill System
  ├── Knowledge Library
  ├── Governance Layer
  ├── Review Layer
  ├── Execution Layer
  ├── Logging Layer
  └── Project Memory
```

Current implementation mode: document-first.

Most layers are documents, contracts, rules, and manually executed workflow artifacts.

## Current Phase

Foundation phase.

The project is currently defining the minimal universal workflow contract before any runtime, automation, backend, frontend, database, or orchestration system is allowed.

## Current Source of Truth Documents

- `README.md`
- `PROJECT_INDEX.md`
- `docs/WORKFLOW_CONTRACT.md`

## Canonical Workflow Contract

The current invariant workflow is defined in:

`docs/WORKFLOW_CONTRACT.md`

Minimal workflow chain:

```text
00_INPUT.md
01_CLARIFICATION.md
02_RESEARCH.md
03_PLAN.md
04_EXECUTION_SPEC.md
05_REVIEW.md
06_RESULT.md
07_KNOWLEDGE_EXTRACT.md
08_LOG.md
```

## Confirmed Principles

1. Document-first before runtime.
2. Governance before scale.
3. Tool-neutral core with adapters later.
4. Repository as source of truth.
5. Generated vs committed vs reviewed vs active state separation.
6. Reuse-first research before designing from scratch.
7. Review before activation.
8. Atomic workflows first.
9. Execution quality before architectural fantasy.
10. Minimal universal workflow before specialized agents.

## Current Forbidden Priorities

Do not build or prioritize yet:

- runtime engine;
- orchestration engine;
- backend;
- frontend;
- vector database;
- semantic search;
- automation framework;
- marketplace;
- mass agent creation;
- mass skill creation;
- Codex execution layer.

## Current Missing Foundation Documents

Required next foundation documents:

- `docs/GOVERNANCE.md`
- `docs/REVIEW_PROCESS.md`
- `docs/LIFECYCLE.md`
- `logs/WORKFLOW_LOG.md`
- `knowledge-library/README.md`

## First Required Workflow Run

A full manual workflow run must be completed before any automation or runtime work.

Target structure:

```text
workflow-runs/0001-example-run/
  00_INPUT.md
  01_CLARIFICATION.md
  02_RESEARCH.md
  03_PLAN.md
  04_EXECUTION_SPEC.md
  05_REVIEW.md
  06_RESULT.md
  07_KNOWLEDGE_EXTRACT.md
  08_LOG.md
```

## Current Status

Initialized as a document-first Project Execution OS foundation.

Current completed artifacts:

- `README.md`
- `docs/WORKFLOW_CONTRACT.md`
- `PROJECT_INDEX.md`

## Next Required Action

Create `docs/GOVERNANCE.md`.

Purpose:
Define project governance rules, source-of-truth rules, state separation, artifact requirements, and anti-overbuilding constraints.
