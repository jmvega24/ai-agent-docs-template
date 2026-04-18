# Architecture

## Purpose

Describe the technical structure of the system.

This file should explain:

- major layers,
- main modules,
- component responsibilities,
- runtime boundaries,
- and important structural patterns.

## Suggested sections

### Stack

| Area | Technology |
|---|---|
| Runtime | `[RUNTIME]` |
| Framework | `[FRAMEWORK]` |
| Database | `[DATABASE]` |
| Auth | `[AUTH_STRATEGY]` |
| Testing | `[TEST_STACK]` |
| Deployment | `[DEPLOYMENT_MODEL]` |

### High-level flow

```text
[Client]
  -> [Gateway / Router]
  -> [Application Layer]
  -> [Domain / Services]
  -> [Persistence / External Providers]
```

### Modules

List the main modules and responsibilities.

### Data flow

Explain the most important request or event flows.

### Cross-cutting concerns

Document:

- auth,
- permissions,
- logging,
- observability,
- caching,
- tenancy,
- error handling,
- or feature flags.

### Limits of this document

This file is not a plan, changelog, or ADR log.
