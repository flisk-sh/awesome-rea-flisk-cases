# Pre-CU Star Wars Galaxies emulator

**Target:** Pre-Combat Upgrade Star Wars Galaxies (server emulator research)
**Goal:** Run a local emulator stack for the pre-CU game
**Status:** Needs verification
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The case is a reader's question about how long AI would take to speed up emulator research. No protocol, client version, or benchmark is given.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/swg-precu-ai-emulator-idea.md

## What Flisk built

Not built yet. Proposed stack:

- Stack idea: `login-server`, `zone-server`, `world-db` (Postgres).
- Commands: `flisk project --yes`, `flisk resource login-server --type backend --stack swg --yes`, `flisk resource zone-server --type backend --stack swg --yes`, `flisk up swg --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md)
