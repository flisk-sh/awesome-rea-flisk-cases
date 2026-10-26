# Animal Jam / Burrow: client and server

**Target:** Animal Jam / Burrow (online game client and server)
**Goal:** Run a local client-server setup for research on the protocol
**Status:** Needs verification (reported, unconfirmed)
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- A reader thinks Claude was used to decompile the client, possibly the server too. The case says this is unconfirmed.
- No protocol or repository is linked.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/animal-jam-burrow-claude-report.md

## What Flisk built

Not built yet. Proposed stack:

- Stack idea: `game-server` (local replacement for research), `login-api`, `player-db`.
- Commands: `flisk project --yes`, `flisk resource game-server --type backend --stack burrow --yes`, `flisk resource player-db --type bring-your-own --stack burrow --yes`, `flisk up burrow --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md)
