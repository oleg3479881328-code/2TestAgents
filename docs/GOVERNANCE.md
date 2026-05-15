# Governance — Project Execution OS

## 1. Purpose

This document defines the governance rules for Project Execution OS.

Governance exists to prevent:

- architectural drift;
- fake execution claims;
- premature runtime building;
- document chaos;
- unreviewed decisions;
- uncontrolled agent or skill growth;
- loss of project state.

## 2. Source of Truth

The GitHub repository is the source of truth.

A project state is valid only if it is represented by a committed repository artifact.

Verbal discussion, generated drafts, chat messages, and uncommitted ideas are not final project state.

## 3. State Separation

The system must always separate these states:

### Generated State

Content proposed by AI, user, or another agent but not yet written to the repository.

Generated state is not execution.

### Committed State

Content written to the repository through a confirmed commit.

Committed state is the minimum valid project record.

### Reviewed State

Committed content that has been checked by a reviewer stage or human reviewer.

Reviewed state may still require corrections.

### Active State

Reviewed content approved for reuse as a stable project rule, workflow, pattern, template, or operational artifact.

No artifact may become active without review.

## 4. No Fake Execution Rule

No agent, assistant, or workflow stage may claim that something was:

- executed;
- saved;
- applied;
- committed;
- tested;
- reviewed;
- approved;
- activated;
- deployed;
- completed;

unless there is evidence.

Acceptable evidence:

- repository commit;
- user-provided execution result;
- reviewed artifact;
- log entry;
- explicit external system output.

## 5. Artifact Requirement

Every important project result must become a repository artifact.

Required artifact types include:

- workflow contract;
- governance rule;
- lifecycle rule;
- review process;
- workflow run stage output;
- project decision;
- research report;
- execution specification;
- review report;
- final result;
- knowledge extraction;
- workflow log;
- reusable pattern;
- anti-pattern;
- lesson learned.

## 6. Universal Workflow Invariant

All projects must follow the Universal Workflow Contract unless the contract is explicitly updated.

Current invariant chain:

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

The domain may change.
The workflow contract remains stable.

## 7. MVP Boundary

The project must remain document-first until the first complete manual workflow run is finished and reviewed.

Current forbidden priorities:

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

## 8. Anti-Overbuilding Rule

Do not build infrastructure before the workflow proves it needs infrastructure.

The correct sequence is:

```text
manual workflow
→ review
→ stabilization
→ repeatable templates
→ specialized agents
→ adapters
→ automation only if justified
```

Wrong sequence:

```text
runtime
→ dashboard
→ database
→ automation
→ unclear workflow
```

## 9. Reuse-First Rule

Before designing from scratch, the relevant workflow stage must look for:

- existing open-source patterns;
- documentation;
- known workflows;
- reusable templates;
- prior project artifacts;
- internal knowledge-library entries.

Reuse does not mean blind copying.

Reusable ideas must be adapted, attributed when needed, and reviewed before becoming active.

## 10. Review Requirement

Any artifact that affects future project behavior must be reviewed before activation.

Artifacts requiring review:

- workflow contracts;
- governance rules;
- lifecycle definitions;
- reusable templates;
- agent definitions;
- skill definitions;
- reusable patterns;
- execution specifications for important projects.

Review must check:

- clarity;
- scope;
- contradictions;
- missing assumptions;
- premature complexity;
- evidence quality;
- reuse value;
- failure modes.

## 11. Specialized Agent Governance

Specialized agents are allowed only when they solve a clear stage or domain bottleneck.

Agents must not replace the workflow contract.

Agents are execution modules.
The workflow contract is invariant.

A specialized agent must define:

- purpose;
- when to use;
- inputs;
- outputs;
- constraints;
- failure modes;
- review requirements.

## 12. Knowledge Library Governance

Reusable knowledge must be extracted after workflow runs.

Knowledge entries must be separated into:

- patterns;
- anti-patterns;
- workflow lessons;
- reusable templates;
- project decisions.

No knowledge entry should be treated as active until reviewed.

## 13. Logging Governance

Major repository changes and workflow milestones must be logged.

A valid log entry should include:

- date or workflow reference;
- action taken;
- affected files;
- reason;
- resulting state;
- risks or lessons;
- next action.

Logs must not claim generated drafts as executed history.

## 14. Decision Governance

Important decisions must be written as repository artifacts or log entries.

A valid decision should include:

- decision statement;
- reason;
- scope;
- affected documents;
- risks;
- reversal condition if applicable.

## 15. Current Governance Status

Status: foundation-draft.

This governance document is committed project state, but it must later be reviewed through the formal review process before becoming active governance.

## 16. Next Required Action

Create `docs/REVIEW_PROCESS.md`.

Purpose:
Define how project artifacts, workflow runs, agents, skills, patterns, and governance documents are reviewed before activation.
