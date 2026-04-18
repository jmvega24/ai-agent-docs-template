# CONTEXT.md

Short operational context for the current project.

Last updated: `[YYYY-MM-DD]`

## Operational agents

| Agent | Role | Configuration |
|---|---|---|
| Orchestrator | Analysis, handoff, audit, documentation sync | `AGENTS.md` |
| Executor | Technical implementation | `CLAUDE.md` |

## Usage

This file should not replace plans, ADRs, or architecture documentation.

Use it to expose only:

- active focus,
- current status,
- nearest priority,
- and quick references for daily work.

## Naming convention

Use one consistent format for work tracking. Example:

- `Milestone N - Name`
- `Phase N - Name`
- `Sprint N - Name`
- `Slice N - Name`

Choose one model and use it everywhere.

## Current status

- Active focus: `[CURRENT_WORKSTREAM]`
- Current status: `[IN_PROGRESS | READY_FOR_AUDIT | READY_FOR_SYNC | CLOSED]`
- Last verified outcome: `[SHORT_SUMMARY]`
- Immediate priority: `[NEXT_PRIORITY]`

## Living references

- `AGENTS.md`
- `CLAUDE.md`
- `docs/context/architecture.md`
- `docs/plans/implementation-plan.md`
- `docs/logs/slice-log.md`
