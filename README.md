# Project Documentation Template

This folder contains a reusable documentation base for software projects.

It is designed to work for:

- backend projects,
- frontend projects,
- full stack products,
- and teams using human workflows, AI agents, or both.

## Goal

Provide a documentation structure that is:

- easy to clone into a new repository,
- clear enough for onboarding,
- structured enough for execution,
- and generic enough to adapt to different stacks.

## Recommended usage

1. Copy this folder into a new repository.
2. Rename or relocate files as needed.
3. Replace placeholders with project-specific information.
4. Remove sections that do not apply to the project.
5. Keep the structure stable once the team starts using it.

## Structure

```text
new-doc-git/
├── AGENTS.md
├── CLAUDE.md
├── CONTEXT.md
├── README.md
├── .env.example
└── docs/
    ├── agents/
    ├── adr/
    ├── api/
    ├── context/
    ├── contracts/
    ├── logs/
    ├── plans/
    └── ux/
```

## Notes

- All content is intentionally generic.
- Replace bracket placeholders like `[PROJECT_NAME]` and `[TEAM_NAME]`.
- Delete folders that are not relevant for the project.
- Keep file names functional and stable.

## Usage Note

Use this template freely in your projects and team workflows. If it helps your work, please keep a visible credit to the original idea.

Created by Juan Vega.
