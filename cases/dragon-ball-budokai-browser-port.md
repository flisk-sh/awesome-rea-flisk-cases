# Dragon Ball Budokai: browser port with a local game server

**Target:** Dragon Ball Budokai (fighting game)
**Goal:** Play a browser port against a local game server
**Status:** Needs verification (REA unconfirmed)
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The case is an unverified report of an AI-assisted browser port (case summary).
- No repository, build, or network protocol is given.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/dragon-ball-budokai-browser.md

## What TDK built

Not built yet. Proposed app types and stack:

- Types: `frontend` (browser game), `backend` (match and save server), `worker` (asset conversion).
- Commands: `tdk project --yes`, `tdk resource game-web --type frontend --stack budokai --yes`, `tdk resource match-server --type backend --stack budokai --yes`, `tdk resource asset-convert --type worker --stack budokai --yes`, `tdk up budokai --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md)
