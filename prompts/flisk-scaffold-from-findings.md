# Prompt: turn findings into a Flisk stack

Read `findings.md`. Build a local stack with the Flisk CLI that reproduces the parts of the app I need.

1. Run `flisk project --yes` in a new folder.
2. For each service the findings need, run `flisk resource <name> --type <backend|frontend|worker|mcp|agent|bring-your-own> --stack <stack> --yes`.
3. Fill in the `service.json` for each service from the findings.
4. Preview with `flisk up <stack> --dry-run`, then start it with `flisk up <stack>`.
5. Check each service's health endpoint and write the result to `case-notes.md`.
