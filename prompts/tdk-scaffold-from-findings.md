# Prompt: turn findings into a TDK stack

Read `findings.md`. Build a local stack with the TDK CLI that reproduces the parts of the app I need.

1. Run `tdk project --yes` in a new folder.
2. For each service the findings need, run `tdk resource <name> --type <backend|frontend> --stack <stack> --yes`.
3. Fill in the `service.json` for each service from the findings.
4. Preview with `tdk up <stack> --dry-run`, then start it with `tdk up <stack>`.
5. Check each service's health endpoint and write the result to `case-notes.md`.
