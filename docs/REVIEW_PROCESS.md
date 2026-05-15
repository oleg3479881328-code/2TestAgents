# Review Process — Project Execution OS

## 1. Purpose

The review process exists to prevent weak artifacts from becoming reusable project truth.

It protects Project Execution OS from:

- vague workflows;
- fake execution claims;
- premature architecture;
- untested assumptions;
- missing constraints;
- low-quality reusable knowledge;
- uncontrolled agent growth;
- document drift;
- overbuilt systems.

## 2. Review Scope

The following artifact types require review before they can become active:

- workflow contracts;
- governance documents;
- lifecycle documents;
- project plans;
- execution specifications;
- result documents;
- knowledge-library entries;
- reusable patterns;
- anti-patterns;
- workflow templates;
- specialized agent definitions;
- AI skill definitions;
- major project decisions.

## 3. Review States

### not_reviewed

The artifact exists but has not been reviewed.

### reviewed_with_required_improvements

The artifact was reviewed and is structurally useful, but it must be corrected before activation.

### reviewed_rejected

The artifact failed review and must not be reused as project truth.

### reviewed_passed

The artifact passed review and may be considered for active status.

### active

The artifact has passed review and is approved for reuse.

## 4. Review Checklist

Every review must check:

- purpose clarity;
- scope clarity;
- input clarity;
- output clarity;
- workflow completeness;
- constraints;
- assumptions;
- evidence quality;
- state separation;
- no fake execution claims;
- risks;
- failure modes;
- reuse value;
- overbuilding risk;
- contradictions with existing project rules;
- next action clarity.

## 5. Review Output Contract

Every review artifact must use this structure:

```text
# Review — <artifact name>

## Reviewed Artifact

Path:
Status before review:

## Summary

Short judgment.

## Strengths

- ...

## Weaknesses

- ...

## Checklist Results

| Check | Result | Notes |
|---|---|---|
| Purpose clarity | pass/fail/partial | ... |
| Scope clarity | pass/fail/partial | ... |
| Inputs | pass/fail/partial | ... |
| Outputs | pass/fail/partial | ... |
| Constraints | pass/fail/partial | ... |
| Evidence | pass/fail/partial | ... |
| State separation | pass/fail/partial | ... |
| No fake execution claims | pass/fail/partial | ... |
| Overbuilding risk | pass/fail/partial | ... |
| Reuse value | pass/fail/partial | ... |

## Required Improvements

- ...

## Decision

reviewed_passed / reviewed_with_required_improvements / reviewed_rejected

## Next Required Action

One concrete next action.
```

## 6. Pass Conditions

An artifact can pass review only if:

- its purpose is clear;
- its scope is narrow enough;
- it does not contradict higher-level governance;
- it does not claim unverified execution;
- it includes constraints;
- it includes risks or failure modes when relevant;
- it produces or supports a concrete next action;
- it does not introduce unjustified runtime, automation, backend, database, or orchestration complexity.

## 7. Failure Conditions

An artifact fails review if it:

- is vague;
- has no clear owner or stage;
- has no defined output;
- makes unverifiable execution claims;
- expands scope without justification;
- duplicates an existing active artifact;
- creates architecture before workflow proof;
- hides assumptions;
- cannot be reused or validated;
- conflicts with the Universal Workflow Contract.

## 8. Review Before Activation Rule

No artifact may become active without review.

This applies to:

- governance rules;
- workflow contracts;
- lifecycle rules;
- reusable templates;
- agent definitions;
- AI skill definitions;
- knowledge-library patterns.

Committed does not mean active.
Reviewed does not automatically mean active.
Active requires explicit approval after review.

## 9. Reviewer Role

The reviewer must act as a quality gate, not as a polite summarizer.

The reviewer must identify:

- contradictions;
- missing constraints;
- weak assumptions;
- premature complexity;
- reusable value;
- operational risk;
- unclear next steps.

The reviewer must not rubber-stamp artifacts.

## 10. Review Storage

Reviews must be stored close to the reviewed artifact when possible.

Recommended locations:

```text
docs/reviews/
workflow-runs/<run-id>/05_REVIEW.md
knowledge-library/reviews/
skills/<category>/<skill-name>/validation/REVIEW.md
agents/<agent-name>/validation/REVIEW.md
```

## 11. Current MVP Rule

During the document-first foundation phase, reviews are manual and document-based.

No automated review engine is allowed yet.

## 12. Next Required Action

Create `docs/LIFECYCLE.md`.

Purpose:
Define lifecycle states for projects, workflow runs, artifacts, agents, skills, and knowledge entries.
