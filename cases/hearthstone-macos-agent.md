# Hearthstone on macOS: game-control agent, deck optimizer and replay review

**Target:** Hearthstone (macOS client)
**Goal:** Run a local agent that plays, optimizes decks and reviews past games
**Status:** Needs verification
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The case reports reversing the macOS client for model control, deck optimization, and game-by-game reflection (case summary).
- No repository, protocol, or result is given, so these are claims only.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/hearthstone-macos-ai-control-report.md

## What TDK built

Not built yet. Proposed app types and stack:

- Types: `agent` (plays the game through a control interface), `backend` (deck optimizer API), `worker` (replay analysis and reflection notes).
- Commands: `tdk project --yes`, `tdk resource player --type agent --stack hs --yes`, `tdk resource deck-api --type backend --stack hs --yes`, `tdk resource replay-review --type worker --stack hs --yes`, `tdk up hs --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md)
