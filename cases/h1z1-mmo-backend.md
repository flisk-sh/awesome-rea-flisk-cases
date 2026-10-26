# H1Z1: from reverse engineering to an MMO backend

**Target:** H1Z1 (online survival shooter), used as research for a new MMO
**Goal:** Run a local MMO backend (login, world, chat, assets) for a game built with AI tools
**Status:** In progress (reported)
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The poster says reverse engineering of H1Z1 is finished and a new MMO is being built with AI tools (case summary).
- No protocol, repository, or build is given.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/h1z1-ai-mmo-research.md

## What Flisk built

Not built yet. Proposed stack:

- Stack idea: `login-server`, `world-server`, `chat-service`, `asset-cdn`, `player-db` (Postgres).
- Commands: `flisk project --yes`, `flisk resource login-server --type backend --stack mmo --yes`, `flisk resource world-server --type backend --stack mmo --yes`, `flisk resource player-db --type bring-your-own --stack mmo --yes`, `flisk up mmo --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md)
