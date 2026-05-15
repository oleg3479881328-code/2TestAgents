# 07_KNOWLEDGE_EXTRACT — Foundation Review

## Workflow Run

`0001-foundation-review`

## Purpose

Extract reusable knowledge from the first manual Project Execution OS workflow run.

## Extracted Patterns

### Pattern 1 — Run the system on itself first

Type: pattern

Status: captured

Summary:
Before expanding a project execution system, use the system to review its own foundation.

Problem it solves:
Prevents building on unreviewed governance and unstable workflow assumptions.

Reuse rule:
When creating a new workflow system, run a self-review workflow before creating runtime, automation, or specialized modules.

Failure risk:
If overused, self-review can become recursive bureaucracy. Limit it to foundation validation and major governance changes.

Related artifacts:

- `workflow-runs/0001-foundation-review/`
- `docs/WORKFLOW_CONTRACT.md`
- `docs/REVIEW_PROCESS.md`

---

### Pattern 2 — Candidate foundation before active foundation

Type: pattern

Status: captured

Summary:
Foundation documents should start as candidate artifacts and only become active after review and explicit activation.

Problem it solves:
Prevents early drafts from becoming permanent standards without quality control.

Reuse rule:
Use candidate status for initial governance, lifecycle, review, and workflow documents until at least one review run validates them.

Failure risk:
If activation never happens, the project may remain permanently provisional.

Related artifacts:

- `docs/LIFECYCLE.md`
- `docs/GOVERNANCE.md`
- `workflow-runs/0001-foundation-review/05_REVIEW.md`

---

### Pattern 3 — Full workflow first, compact mode later

Type: pattern

Status: captured

Summary:
Validate the full workflow once before creating a compact version for small tasks.

Problem it solves:
Prevents premature simplification before the complete workflow is understood.

Reuse rule:
Use the full 9-stage workflow for foundation validation, then create a compact workflow mode only after the full workflow proves stable.

Failure risk:
If the full workflow is forced onto every small task, the system becomes too heavy.

Related artifacts:

- `docs/WORKFLOW_CONTRACT.md`
- `workflow-runs/0001-foundation-review/05_REVIEW.md`

## Extracted Anti-Patterns

### Anti-Pattern 1 — Runtime before workflow proof

Type: anti-pattern

Status: captured

Summary:
Building backend, automation, orchestration, or UI before the manual workflow is validated creates architectural fantasy instead of execution quality.

Avoidance rule:
No runtime layer until the workflow is manually proven and reviewed.

Related artifacts:

- `docs/GOVERNANCE.md`
- `logs/WORKFLOW_LOG.md`

### Anti-Pattern 2 — Active by commit

Type: anti-pattern

Status: captured

Summary:
Treating committed files as active standards without review corrupts project governance.

Avoidance rule:
Committed means recorded. It does not mean reviewed or active.

Related artifacts:

- `docs/LIFECYCLE.md`
- `docs/REVIEW_PROCESS.md`

## Lessons Learned

1. The universal workflow is usable for reviewing the system itself.
2. The foundation is coherent but still needs a reusable template.
3. Knowledge extraction should happen immediately after review, not later.
4. The full workflow may be too heavy for small tasks, so compact mode should be designed later.

## Recommended Knowledge Library Entries

Create structured entries later for:

- `patterns/run-system-on-itself-first.md`
- `patterns/candidate-foundation-before-active-foundation.md`
- `patterns/full-workflow-first-compact-mode-later.md`
- `anti-patterns/runtime-before-workflow-proof.md`
- `anti-patterns/active-by-commit.md`

## Next Required Action

Create `08_LOG.md` to close the workflow run.
