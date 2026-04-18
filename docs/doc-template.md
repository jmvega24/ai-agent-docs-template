# Base Documentation Template For Software Projects

This document provides a reusable documentation structure for software teams working on backend, frontend, or full stack projects.

Its purpose is to give any repository a clear documentation baseline that supports:

- onboarding,
- execution,
- architecture visibility,
- contract clarity,
- progress tracking,
- and collaboration between humans and agents.

## Recommended Structure

```text
/
├── AGENTS.md
├── CLAUDE.md
├── CONTEXT.md
├── README.md
├── .env.example
├── docs/
│   ├── agents/
│   │   ├── atlas-operating-checklist.md
│   │   └── closure-gate.md
│   ├── context/
│   │   ├── architecture.md
│   │   ├── conventions.md
│   │   ├── domain-model.md
│   │   ├── glossary.md
│   │   ├── handoff-schema.md
│   │   ├── identity-and-access.md
│   │   ├── integration-model.md
│   │   └── risks-and-open-questions.md
│   ├── contracts/
│   │   ├── frontend-backend/
│   │   │   ├── handoff.md
│   │   │   ├── flows-mvp.md
│   │   │   └── role-matrix.md
│   │   ├── backend-external/
│   │   │   ├── provider-a-contract.md
│   │   │   └── provider-b-contract.md
│   │   └── internal/
│   │       ├── module-a-to-module-b.md
│   │       └── event-contracts.md
│   ├── plans/
│   │   ├── implementation-plan.md
│   │   ├── backlog-slice-1.md
│   │   └── backlog-slice-2.md
│   ├── logs/
│   │   ├── slice-log.md
│   │   ├── decision-log.md
│   │   └── release-log.md
│   ├── api/
│   │   ├── openapi.json
│   │   ├── postman-collection.json
│   │   └── examples/
│   │       └── sample-request.http
│   ├── adr/
│   │   ├── README.md
│   │   ├── _template.md
│   │   ├── 0001-architecture-choice.md
│   │   ├── 0002-auth-strategy.md
│   │   └── 0003-data-model.md
│   ├── ux/
│   │   ├── screen-map.md
│   │   ├── ui-rules.md
│   │   └── content-guidelines.md
│   ├── template-index.md
│   └── doc-template.md
├── scripts/
├── src/
├── tests/
└── infra/
```

## Quick Purpose Of Each File And Folder

### Root

#### `AGENTS.md`
Rules for the orchestration layer. It explains how to analyze work, prepare handoffs, review results, and protect documentation coherence.

#### `CLAUDE.md`
Rules for the execution layer. It explains how to implement bounded tasks, preserve conventions, validate work, and report outcomes.

#### `CONTEXT.md`
Short operational context. It gives the current focus, status, and quick references for day-to-day work.

#### `README.md`
Entry-point file for humans. It explains what the template is, how to use it, and how to adapt it to a real repository.

#### `.env.example`
Safe environment-variable template with placeholders only. It documents the minimum runtime configuration expected by the project.

### `docs/agents/`

#### `atlas-operating-checklist.md`
Short checklist for orchestration work. Useful before handing off, auditing, or closing work.

#### `closure-gate.md`
Defines what must be true before a task, milestone, phase, or slice can be considered closed.

### `docs/context/`

#### `architecture.md`
Explains the technical structure of the system: layers, modules, runtime boundaries, and cross-cutting concerns.

#### `conventions.md`
Documents practical repository conventions such as naming, structure, documentation rules, and testing expectations.

#### `domain-model.md`
Describes the core business or product concepts, main entities, relationships, and important rules.

#### `glossary.md`
Keeps language consistent across engineering, product, design, and operations.

#### `handoff-schema.md`
Defines the recommended format for structured delegation from an orchestration layer to an execution layer.

#### `identity-and-access.md`
Documents authentication, authorization, roles, permissions, claims, sessions, and access rules.

#### `integration-model.md`
Explains how the project integrates internally and externally, including patterns, dependencies, and failure handling.

#### `risks-and-open-questions.md`
Tracks unresolved issues, assumptions, and open questions that may affect implementation or delivery.

### `docs/contracts/`

#### `frontend-backend/handoff.md`
Summarizes what the frontend team needs from backend or service contracts without exploring the entire implementation.

#### `frontend-backend/flows-mvp.md`
Documents the minimum cross-layer flows that must remain aligned between UI and service behavior.

#### `frontend-backend/role-matrix.md`
Defines what each user role can see or do from a product perspective.

#### `backend-external/provider-a-contract.md`
Template for documenting one external provider integration.

#### `backend-external/provider-b-contract.md`
Template for documenting another external provider integration when needed.

#### `internal/module-a-to-module-b.md`
Documents one internal module-to-module contract, including responsibilities and compatibility rules.

#### `internal/event-contracts.md`
Documents internal events or messages exchanged between modules or services.

### `docs/plans/`

#### `implementation-plan.md`
High-level execution map for the project. It explains how work is sequenced and how completion is evaluated.

#### `backlog-slice-1.md`
Operational backlog example for one work item, milestone, phase, slice, or sprint.

#### `backlog-slice-2.md`
Second backlog example using the same structure as the first one.

### `docs/logs/`

#### `slice-log.md`
Chronological work log with verified delivery entries, outcomes, validation, and follow-up notes.

#### `decision-log.md`
Compact log for important decisions that do not need a full ADR.

#### `release-log.md`
Tracks relevant releases, deployments, or delivery drops over time.

### `docs/api/`

#### `openapi.json`
API contract placeholder for HTTP-based systems.

#### `postman-collection.json`
Postman collection placeholder for manual testing or quick integration setup.

#### `examples/sample-request.http`
Simple example request that teams can adapt to their stack.

### `docs/adr/`

#### `README.md`
Explains when and how to write Architecture Decision Records.

#### `_template.md`
Generic ADR template that teams can duplicate for new decisions.

#### `0001-architecture-choice.md`
Starter example for an architectural decision.

#### `0002-auth-strategy.md`
Starter example for an authentication decision.

#### `0003-data-model.md`
Starter example for a persistence or data-structure decision.

### `docs/ux/`

#### `screen-map.md`
High-level map of screens, routes, or views in the product.

#### `ui-rules.md`
Defines consistency and interaction rules for the interface.

#### `content-guidelines.md`
Defines tone, wording, and messaging rules for user-facing copy.

### Support files inside `docs/`

#### `template-index.md`
Quick index for what to replace first and what can be removed if not relevant.

#### `doc-template.md`
This file. It gives the visual structure and short purpose summary of the whole documentation system.

## Practical Usage Rules

- Keep the repository root small and easy to scan.
- Keep operational context separate from structural documentation.
- Keep plans separate from logs.
- Document major technical decisions in ADRs.
- Use stable file names based on function, not temporary intent.
- Remove optional folders that do not apply to the project.
- Replace placeholders early so the template becomes project-specific quickly.

## Recommended Minimum For Small Projects

For smaller repositories, the minimum recommended set is:

- `AGENTS.md`
- `CLAUDE.md`
- `CONTEXT.md`
- `README.md`
- `docs/context/`
- `docs/contracts/`
- `docs/plans/`
- `docs/logs/`
- `docs/api/`

## Final Goal

This template is meant to help teams create repositories with:

- clear context,
- organized execution,
- visible contracts,
- traceable decisions,
- and reusable documentation practices.

## Usage Note

Use this template freely in your projects and team workflows. If it helps your work, please keep a visible credit to the original idea.

Created by Juan Vega.
