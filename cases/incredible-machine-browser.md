# The Incredible Machine in the browser

**Target:** The Incredible Machine (Sierra puzzle game)
**Goal:** Play a browser rebuild with regenerated assets
**Status:** Needs verification (reported, Claude)
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The case reports that Claude Opus 5.5 studied the original game and regenerated assets for a browser version (video shown by the author).
- No repository or build is linked in the case.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/incredible-machine-browser.md

## What Flisk built

Not built yet. Proposed stack:

- Stack idea: `game-web` (browser client), `asset-service` (serves regenerated assets), `level-db` (puzzle levels).
- Commands: `flisk project --yes`, `flisk resource game-web --type frontend --stack puzzle --yes`, `flisk resource asset-service --type backend --stack puzzle --yes`, `flisk up puzzle --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md)
