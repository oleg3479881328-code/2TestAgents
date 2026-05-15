# Universal Workflow Contract v1

## 1. Purpose

The Universal Workflow Contract defines the invariant project execution loop for Project Execution OS.

It must be usable for any project type:

- software;
- websites;
- Telegram bots;
- furniture selection;
- home repair;
- cooking;
- OSINT;
- business planning;
- automation;
- learning;
- AI systems.

The domain may change. The workflow contract must remain stable.

## 2. Core Principle

Do not build giant architecture before the workflow is proven.

Execution quality is more important than architectural fantasy.

## 3. Universal Execution Loop

Every project must pass through this minimal chain:

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

## 4. Stage Definitions

### 00_INPUT.md

Raw user request, project idea, problem, goal, or task.

Must preserve the original intent without over-interpreting it.

### 01_CLARIFICATION.md

Clarifies ambiguity, scope, constraints, success criteria, and missing context.

Must avoid endless questioning.

### 02_RESEARCH.md

Finds reusable patterns, existing solutions, documentation, prior examples, and risks.

Research must be reuse-first and evidence-backed when possible.

### 03_PLAN.md

Converts clarified intent and research into a practical project plan.

The plan must stay MVP-first.

### 04_EXECUTION_SPEC.md

Defines what must be executed, built, written, purchased, tested, or decided.

For software projects, this can become a coder-ready specification.
For non-software projects, this becomes an action-ready execution brief.

### 05_REVIEW.md

Audits the plan, execution spec, assumptions, risks, contradictions, and missing pieces.

Nothing should be treated as stable without review.

### 06_RESULT.md

Records the final result of the workflow run.

The result may be a decision, document, implementation spec, recommendation, design, or completed artifact.

### 07_KNOWLEDGE_EXTRACT.md

Extracts reusable lessons, patterns, anti-patterns, templates, and decisions.

Reusable knowledge must be separated from one-off project output.

### 08_LOG.md

Records what happened, what changed, what was decided, what remains open, and what should happen next.

## 5. State Separation

The system must distinguish:

- generated state: proposed by AI or user but not committed;
- committed state: written to repository;
- reviewed state: checked by reviewer;
- active state: approved for reuse.

No agent may claim something is executed, saved, committed, tested, reviewed, or active without evidence.

## 6. Specialized Agents

Specialized agents are replaceable execution modules.

They may be created only when needed for:

- a specific workflow stage;
- a specific domain;
- a specific quality bottleneck.

Examples:

- OSINT Research Agent;
- Telegram Bot Architect;
- Website UX Reviewer;
- Furniture Selection Reviewer;
- Cooking Research Agent.

Agents are replaceable. The workflow contract is invariant.

## 7. Forbidden Current Priorities

Do not prioritize now:

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

## 8. First Validation Rule

Before expanding the system, complete one full manual workflow run from `00_INPUT.md` to `08_LOG.md`.

No automation before one complete manual run proves the workflow.

## 9. Success Criteria for v1

Universal Workflow Contract v1 is acceptable only if it:

- can guide any project domain;
- stays minimal;
- prevents premature runtime building;
- supports review;
- supports knowledge extraction;
- keeps repository state truthful;
- produces one concrete next action per workflow run.
