# Red Alert 2: an engine rewrite for reinforcement learning

**Target:** Red Alert 2 (RTS), browser reimplementation Chrono Divide
**Goal:** Run a game environment server that RL agents can train against
**Status:** Needs verification (reported)
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The case reports a rewritten RTS engine with over 6,000 unit tests, built with Opus 5.5 (author report).
- The case does not give a repository or training results.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/red-alert-2-rl-engine.md

## What Flisk built

Not built yet. Proposed stack:

- Stack idea: `env-server` (game engine over HTTP), `trainer` (RL loop), `metrics-db`.
- Commands: `flisk project --yes`, `flisk resource env-server --type backend --stack rl --yes`, `flisk resource trainer --type backend --stack rl --yes`, `flisk up rl --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md)
