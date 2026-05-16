# START HERE FOR AI — Project Execution OS

## 1. Purpose

This file is the entry point for any AI assistant, agent, or chat that is pointed to this repository.

If a user gives you this repository link, you must treat this file as the first document to read and follow.

Repository:

`oleg3479881328-code/2TestAgents`

Project:

Project Execution OS

## 2. What This Project Is

Project Execution OS is a universal document-first system for running any project through a repeatable workflow.

It is designed to guide projects from raw idea to reviewed result and reusable knowledge extraction.

It can be used for:

- software projects;
- AI systems;
- Telegram bots;
- websites;
- automation;
- OSINT;
- business projects;
- learning projects;
- physical-world projects;
- any structured task that needs execution discipline.

## 3. What This Project Is Not

This project is not only:

- an AI Skill System;
- an agent framework;
- a Codex workflow;
- an orchestration engine;
- a backend project;
- a runtime system;
- a prompt collection.

AI Skill System is only one subsystem inside Project Execution OS.

## 4. Core Rule

Do not start by writing code.
Do not start by building runtime.
Do not start by creating automation.
Do not start by designing a giant architecture.

Start with the universal document-first workflow.

## 5. Required Reading Order

Before helping with any new project, read these files in order:

1. `README.md`
2. `PROJECT_INDEX.md`
3. `docs/WORKFLOW_CONTRACT.md`
4. `docs/GOVERNANCE.md`
5. `docs/REVIEW_PROCESS.md`
6. `docs/LIFECYCLE.md`
7. `knowledge-library/README.md`
8. `workflow-templates/universal-workflow-v1/README.md`
9. `logs/WORKFLOW_LOG.md`

If time or context is limited, read at minimum:

1. `PROJECT_INDEX.md`
2. `docs/WORKFLOW_CONTRACT.md`
3. `docs/GOVERNANCE.md`
4. `workflow-templates/universal-workflow-v1/README.md`

## 6. Universal Workflow

Every real project should be guided through this chain:

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

The domain may change. The workflow stays stable.

## 7. How To Start A New Project

When the user gives a new project idea, do this:

1. Create or identify the project repository.
2. Create a workflow run folder:

```text
workflow-runs/0001-initial-project-definition/
```

3. Use `workflow-templates/universal-workflow-v1/` as the template.
4. Start with `00_INPUT.md`.
5. Do not skip to code or execution.
6. Proceed stage by stage.
7. Ask only necessary clarification questions.
8. Keep the project MVP-first.
9. Record the result.
10. Extract reusable knowledge.
11. Log the workflow run.

## 8. State Separation

Always distinguish:

- generated state: proposed but not committed;
- committed state: written to repository;
- reviewed state: checked by review process;
- active state: approved for reuse.

Do not claim something is saved, applied, executed, tested, committed, reviewed, or active unless there is evidence.

## 9. Forbidden Current Priorities

Do not prioritize:

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

These may be considered later only after the document-first workflow is proven and reviewed.

## 10. How To Respond To The User

Be direct.

Do not give a large theoretical explanation unless asked.

For a new project, your first response should usually be:

1. confirm that Project Execution OS is being used;
2. identify the project goal;
3. create or propose the first workflow run;
4. begin with `00_INPUT.md` and `01_CLARIFICATION.md`;
5. give one concrete next action.

## 11. Default Next Action

If the user only points you to this repository and says they want to start a project, the next action is:

Create the first workflow run folder and begin `00_INPUT.md`.

## 12. Critical Warning

If you ignore this file and jump directly to coding, automation, agent creation, or architecture expansion, you are violating the project system.
