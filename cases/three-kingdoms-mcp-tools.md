# Three Kingdoms XIV: trainer functions as an MCP server

**Target:** Romance of the Three Kingdoms XIV (single-player strategy game), VAN editor and trainer functions
**Goal:** Expose the editor and trainer functions as MCP tools so an agent can batch-edit scenarios
**Status:** Needs verification (REA unconfirmed)
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The author reports analyzing the VAN editor and a trainer, then combining their functions into an MCP server (case summary).
- No MCP implementation or modification recipe is published in the case.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/three-kingdoms-mod-mcp.md

## What Flisk built

Not built yet. Proposed app types and stack:

- Types: `mcp` (tool server for editor functions), `backend` (scenario store and batch jobs), `worker` (apply edits to save files).
- Commands: `flisk project --yes`, `flisk resource tools --type mcp --stack tk14 --yes`, `flisk resource scenario-api --type backend --stack tk14 --yes`, `flisk resource batch-edit --type worker --stack tk14 --yes`, `flisk up tk14 --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md)
