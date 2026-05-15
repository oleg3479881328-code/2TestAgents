# Lifecycle — Project Execution OS

## 1. Purpose

This document defines lifecycle states for Project Execution OS artifacts.

Lifecycle exists to prevent confusion between:

- raw ideas;
- generated drafts;
- committed documents;
- reviewed artifacts;
- active standards;
- deprecated material.

## 2. Core Lifecycle Principle

Committed does not mean reviewed.
Reviewed does not mean active.
Active requires explicit approval.

Every important artifact must have a visible lifecycle state.

## 3. Universal Artifact Lifecycle

Default lifecycle for documents, templates, workflow contracts, governance rules, review rules, knowledge entries, agents, and skills:

```text
draft
→ candidate
→ reviewed
→ active
→ deprecated
→ retired
```

## 4. State Definitions

### draft

Raw or early artifact.

Characteristics:

- may be incomplete;
- may contain assumptions;
- not safe for reuse;
- not reviewed;
- not active.

### candidate

Structured artifact ready for review.

Characteristics:

- purpose is clear;
- basic structure exists;
- outputs or usage are defined;
- ready to be checked;
- still not active.

### reviewed

Artifact has passed through review.

Characteristics:

- strengths and weaknesses are known;
- required improvements may exist;
- review decision is recorded;
- still not automatically active.

### active

Approved artifact for reuse.

Characteristics:

- reviewed;
- stable enough for operational use;
- accepted as current project truth;
- may be referenced by future workflow runs.

### deprecated

Still available but replaced by a better artifact.

Characteristics:

- should not be used for new work;
- kept for history and compatibility;
- replacement should be referenced.

### retired

Removed from normal project usage.

Characteristics:

- no longer valid;
- kept only for archival or historical reasons;
- must not guide future work.

## 5. Project Lifecycle

A project may move through:

```text
idea
→ clarified
→ researched
→ planned
→ specified
→ reviewed
→ executed_or_decided
→ knowledge_extracted
→ logged
→ closed
```

These states map to the Universal Workflow Contract stages.

## 6. Workflow Run Lifecycle

A workflow run moves through:

```text
created
→ input_recorded
→ clarification_done
→ research_done
→ plan_done
→ execution_spec_done
→ review_done
→ result_recorded
→ knowledge_extracted
→ logged
→ complete
```

A workflow run is not complete until `08_LOG.md` exists.

## 7. Document Lifecycle

Documents use the universal artifact lifecycle:

```text
draft
→ candidate
→ reviewed
→ active
→ deprecated
→ retired
```

Examples:

- `WORKFLOW_CONTRACT.md`
- `GOVERNANCE.md`
- `REVIEW_PROCESS.md`
- `LIFECYCLE.md`
- workflow templates
- reusable specifications

## 8. Agent Lifecycle

Agents use:

```text
draft
→ candidate
→ reviewed
→ active
→ deprecated
→ retired
```

An agent cannot become active unless it defines:

- purpose;
- when to use;
- inputs;
- outputs;
- constraints;
- failure modes;
- review requirements.

Agents are replaceable modules.
They must not override the workflow contract.

## 9. AI Skill Lifecycle

AI skills use:

```text
draft
→ candidate
→ reviewed
→ active
→ deprecated
→ retired
```

A skill cannot become active without:

- clear task boundary;
- required inputs;
- expected outputs;
- workflow;
- constraints;
- failure modes;
- validation checklist;
- source references when adapted;
- review artifact.

## 10. Knowledge Entry Lifecycle

Knowledge-library entries use:

```text
captured
→ structured
→ reviewed
→ active
→ deprecated
→ retired
```

### captured

Raw lesson, pattern, anti-pattern, or insight extracted from a workflow run.

### structured

Converted into a reusable knowledge entry.

### reviewed

Checked for clarity, reuse value, and risk.

### active

Approved for reuse in future workflow runs.

## 11. Decision Lifecycle

Important decisions use:

```text
proposed
→ recorded
→ reviewed
→ accepted
→ superseded
→ retired
```

A decision is not accepted until it is recorded and reviewed.

## 12. Valid Transitions

Normal transition:

```text
draft → candidate → reviewed → active → deprecated → retired
```

Allowed rollback:

```text
candidate → draft
reviewed → candidate
active → deprecated
```

Forbidden shortcuts:

```text
draft → active
candidate → active
committed → active
reviewed → active without explicit approval
```

## 13. Lifecycle Metadata Recommendation

Artifacts should include visible status where practical.

Recommended metadata fields:

```yaml
status: draft | candidate | reviewed | active | deprecated | retired
review_status: not_reviewed | reviewed_with_required_improvements | reviewed_rejected | reviewed_passed
version: 0.1.0
last_updated: YYYY-MM-DD
```

## 14. Current Foundation Artifact Status

Current committed foundation artifacts:

| Artifact | Status | Review Status |
|---|---|---|
| README.md | candidate | not_reviewed |
| PROJECT_INDEX.md | candidate | not_reviewed |
| docs/WORKFLOW_CONTRACT.md | candidate | not_reviewed |
| docs/GOVERNANCE.md | candidate | not_reviewed |
| docs/REVIEW_PROCESS.md | candidate | not_reviewed |
| docs/LIFECYCLE.md | candidate | not_reviewed |

## 15. Activation Rule

No foundation document is active until it receives a review artifact and explicit activation decision.

## 16. Next Required Action

Create `logs/WORKFLOW_LOG.md`.

Purpose:
Record the initialization history of the Project Execution OS repository and prevent invisible project drift.
