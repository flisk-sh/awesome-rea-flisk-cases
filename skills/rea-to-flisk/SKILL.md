---
name: rea-to-flisk
description: Turn REA reverse-engineering findings into a local Flisk CLI stack. Use when the user has findings from REA (endpoints, protocols, data formats) and wants a runnable local stack for them.
---

# REA to Flisk

Use this skill only on software the user is allowed to analyze.

## Steps

1. Read `findings.md`. If it does not exist, ask the user to run REA first (see `prompts/rea-analyze-app.md`).
2. Group the findings into services: one per endpoint or protocol family, plus storage if data is kept.
3. Run `flisk project --yes` in a new folder.
4. For each service, run `flisk resource <name> --type <backend|frontend|worker|mcp|agent|bring-your-own> --stack <stack> --yes`.
5. Edit each `service.json` from the findings: ports, routes, and environment.
6. Run `flisk up <stack> --dry-run`, then `flisk up <stack>`. Check each health endpoint.
7. Write `case-notes.md`: what matched the original behavior and what did not.

## Limits

- Flisk runs local services only. It does not deploy them.
- Do not copy proprietary assets, keys, or credentials into `service.json` or the output.
