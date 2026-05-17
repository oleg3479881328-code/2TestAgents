# Run The System On Itself First

## Type

pattern

## Status

structured

## Source

`workflow-runs/0001-foundation-review/07_KNOWLEDGE_EXTRACT.md`

## Summary

Before expanding a project execution system, use the system to review its own foundation.

## Problem It Solves

This pattern prevents a system from being built on unreviewed governance, unstable workflow assumptions, and architectural fantasy.

A project execution system should prove that its own workflow can process its own foundation before being used to manage other projects.

## Reuse Rule

When creating a new workflow system, agent system, skill system, project OS, or governance-heavy process, run a self-review workflow before creating runtime, automation, dashboards, orchestration, or specialized modules.

Minimum self-review chain:

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

## Failure Risk

If overused, self-review can become recursive bureaucracy.

Limit this pattern to:

- foundation validation;
- major governance changes;
- workflow contract changes;
- activation decisions.

Do not use this pattern to delay small execution tasks forever.

## Related Artifacts

- `workflow-runs/0001-foundation-review/`
- `docs/WORKFLOW_CONTRACT.md`
- `docs/REVIEW_PROCESS.md`
- `docs/GOVERNANCE.md`

## Review Status

not_reviewed
