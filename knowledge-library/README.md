# Knowledge Library — Project Execution OS

## 1. Purpose

The Knowledge Library stores reusable knowledge extracted from Project Execution OS workflow runs.

It exists to prevent useful lessons, patterns, decisions, and mistakes from being lost after individual projects.

The Knowledge Library is not a random notes folder.
It is a reviewed repository of reusable project execution knowledge.

## 2. Scope

The Knowledge Library may contain:

- reusable patterns;
- anti-patterns;
- workflow lessons;
- reusable templates;
- project decisions;
- domain-specific lessons;
- agent improvement notes;
- skill improvement notes;
- execution quality rules.

## 3. Core Rule

Knowledge must be extracted after workflow runs.

A project is not fully complete until useful knowledge has been extracted or explicitly marked as having no reusable knowledge.

## 4. Current Directory Structure

Recommended structure:

```text
knowledge-library/
  README.md
  patterns/
  anti-patterns/
  workflow-lessons/
  templates/
  decisions/
```

## 5. Knowledge Entry Types

### patterns

Reusable successful approaches.

Examples:

- document-first before runtime;
- governance before scale;
- repository as source of truth;
- review before activation.

### anti-patterns

Repeated mistakes or dangerous approaches.

Examples:

- building runtime before workflow proof;
- creating mass agents before governance;
- treating generated drafts as executed state;
- creating dashboards before the execution loop works.

### workflow-lessons

Lessons learned from specific workflow runs.

Examples:

- where clarification was too weak;
- where research prevented bad architecture;
- where review caught contradictions;
- where knowledge extraction produced reusable value.

### templates

Reusable document structures.

Examples:

- workflow run template;
- review template;
- execution spec template;
- knowledge extract template.

### decisions

Important project decisions that may affect future work.

Examples:

- keep core workflow tool-neutral;
- delay automation until manual workflow is validated;
- treat AI Skill System as a subsystem.

## 6. Lifecycle

Knowledge entries use this lifecycle:

```text
captured
→ structured
→ reviewed
→ active
→ deprecated
→ retired
```

Captured knowledge is not automatically active.
Structured knowledge is not automatically active.
Reviewed knowledge is not automatically active unless explicitly approved.

## 7. Required Knowledge Entry Format

Every reusable knowledge entry should include:

```text
# <Knowledge Entry Title>

## Type

pattern / anti-pattern / workflow-lesson / template / decision

## Status

captured / structured / reviewed / active / deprecated / retired

## Source

Workflow run, artifact, conversation, repository file, or external reference.

## Summary

Short explanation.

## Problem It Solves

What issue this knowledge helps with.

## Reuse Rule

How this knowledge should be reused.

## Failure Risk

What can go wrong if reused badly.

## Related Artifacts

Links or paths to related repository files.
```

## 8. Review Requirement

Knowledge entries must be reviewed before becoming active.

Review must check:

- clarity;
- reuse value;
- scope;
- source quality;
- risk;
- contradiction with existing governance;
- whether it is truly reusable or only project-specific.

## 9. What Must Not Go Here

Do not store:

- random thoughts;
- unstructured chat dumps;
- unverified claims;
- one-off details with no reuse value;
- duplicate versions of the same pattern;
- active rules without review.

## 10. First Seed Patterns

Initial candidate patterns to extract later:

- Document-first before runtime.
- Governance before scale.
- Tool-neutral core with adapters later.
- Repository as source of truth.
- Generated vs committed vs reviewed vs active state separation.
- Reuse-first research before designing from scratch.
- Review before activation.
- Atomic workflows first.
- Minimal universal workflow before specialized agents.

These are candidate patterns until structured and reviewed as separate knowledge entries.

## 11. Next Required Action

Create the first manual workflow run folder:

```text
workflow-runs/0001-foundation-review/
```

Purpose:
Run the Project Execution OS against itself and review the foundation documents before activating them.
