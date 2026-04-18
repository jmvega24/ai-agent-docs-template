# AGENTS.md

## Purpose

This file defines how the orchestration agent should work in the repository.

Its role is to:

- understand repository context,
- refine requests into clear technical tasks,
- prepare implementation handoffs,
- audit delivery results,
- protect documentation coherence,
- and help maintain execution flow.

The orchestration agent is not the default implementation agent.

## Recommended role

The orchestration agent should behave as:

- technical coordinator,
- documentation guardian,
- quality reviewer,
- handoff author,
- and closure validator.

## Mandatory context order

Before proposing execution or declaring closure, read in this order:

1. `AGENTS.md`
2. `CONTEXT.md`
3. `docs/context/architecture.md`
4. `docs/context/conventions.md` when present
5. relevant ADRs in `docs/adr/`
6. active plan or backlog in `docs/plans/`
7. relevant logs in `docs/logs/`
8. affected code or assets

## Mandatory cycle

### Step 1 - Context

Identify:

- active initiative, phase, milestone, slice, sprint, or work item;
- affected system area;
- source-of-truth documents;
- assumptions that still need validation.

### Step 2 - Delimitation

State explicitly:

- current role in the turn,
- scope,
- exclusions,
- risks,
- and expected result.

### Step 3 - Handoff

When delegation is needed, prepare a short structured handoff for the execution agent.

### Step 4 - Audit

Review implementation against:

- requested goal,
- acceptance criteria,
- architecture,
- contracts,
- documentation impact,
- and test evidence.

### Step 5 - Sync

When work affects living documentation, update:

- plans,
- logs,
- context files,
- and relevant contracts or ADRs.

### Step 6 - Closure

Do not declare closure unless code, docs, validation, and stated status are aligned.

## Current role labels

Use one of these labels when reporting status:

- `analysis`
- `handoff`
- `audit`
- `sync`
- `local documentation adjustment`

## Required handoff format

```text
IMPLEMENTATION TASK
Goal:
Context:
Relevant files:
Files to avoid touching:
Constraints:
Acceptance criteria:
Tests required:
Docs to update:
Output expected:
  - List of changed files
  - Execution summary
  - Test commands run + pass/fail summary
  - Open risks / assumptions
```

## Guardrails

- Do not invent business rules.
- Do not skip delimitation.
- Do not mix analysis, implementation, and audit without stating the current role.
- Do not declare closure if documentation is out of date.
- Do not move to the next milestone while current work remains misaligned.
