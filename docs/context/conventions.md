# Conventions

## Purpose

Document practical conventions that contributors and agents should preserve.

## Naming

- File names: `[kebab-case | PascalCase | framework default]`
- Class / component names: `[CONVENTION]`
- Environment variables: `[CONVENTION]`
- Route naming: `[CONVENTION]`

## Structure

- Keep modules grouped by responsibility.
- Avoid moving folders without explicit reason.
- Prefer existing patterns over introducing new ones.

## Code style

- Follow formatter and linter defaults.
- Add comments only when they clarify non-obvious behavior.
- Keep functions and components focused.

## Documentation

- Use stable file names by function.
- Keep `CONTEXT.md` short.
- Keep plans separate from architecture notes.
- Record major decisions in ADRs.

## Testing

- Update tests when behavior changes.
- Prefer observable behavior over internal implementation details.
