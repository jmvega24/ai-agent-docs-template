# CLAUDE.md

## Purpose

This file defines how the execution agent should operate in the repository.

The execution agent is expected to:

- implement bounded tasks,
- preserve repository conventions,
- keep changes reviewable,
- run relevant validation,
- and report results clearly.

## Required inputs before starting

Read in this order:

1. the task handoff;
2. `CONTEXT.md`;
3. `docs/context/architecture.md` when the task affects architecture or core flows;
4. `docs/context/conventions.md` when present;
5. relevant plans in `docs/plans/`;
6. relevant ADRs in `docs/adr/`;
7. the affected code or assets.

If the handoff conflicts with the repository, report the conflict.

## Execution rules

- Implement only the requested scope.
- Prefer small and consistent changes.
- Avoid unrelated refactors.
- Preserve naming, structure, and conventions unless the task requires otherwise.
- Update docs only when the task changes behavior, contracts, workflow, or closure state.

## Tests

Tests are required when the task changes:

- user-visible behavior,
- API contracts,
- authorization rules,
- persistence behavior,
- data flow,
- or critical UI logic.

Tests are optional for:

- documentation-only work,
- pure wording changes,
- non-functional metadata updates.

## Output format

```text
Execution summary
- Goal completed:
- Files changed:
- Tests written / updated:
- Tests actually executed:
- Docs updated:
- Assumptions:
- Risks / pending items:
```

## What not to do

- Do not invent missing requirements.
- Do not broaden scope.
- Do not claim tests were run if they were not run.
- Do not rewrite unrelated files.
- Do not create commits unless explicitly requested.
