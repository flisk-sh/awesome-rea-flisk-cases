# Browser Counter-Strike: multiplayer in the browser

**Target:** Counter-Strike style multiplayer shooter (browser version, version not named)
**Goal:** Run a browser client against a local game server
**Status:** Needs verification (reported)
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- A colleague reportedly made a multiplayer browser version in about 20 minutes with AI (case summary).
- The case does not name the original version or give a repository.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/cs-browser-colleague-ai-report.md

## What Flisk built

Not built yet. Proposed stack:

- Stack idea: `game-server`, `web-client`, `match-lobby`.
- Commands: `flisk project --yes`, `flisk resource game-server --type backend --stack cs --yes`, `flisk resource web-client --type frontend --stack cs --yes`, `flisk up cs --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md)
