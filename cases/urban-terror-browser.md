# Urban Terror in the browser

**Target:** Urban Terror (Quake III engine shooter)
**Goal:** Play multiplayer Urban Terror in a browser
**Status:** Reported (popular, not REA)
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- Per the case summary, the model located data-layout differences between engine structures that had blocked the ioquake3 WebAssembly build.
- Reported engagement at the time of the case: 479 likes, 111,000 views. REA was not used.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/urban-terror-web.md

## What Flisk built

Not built yet. Proposed stack:

- Stack idea: `game-server` (dedicated server), `web-client` (WebAssembly build), `matchmaker` (lobby list).
- Commands: `flisk project --yes`, `flisk resource game-server --type backend --stack shooter --yes`, `flisk resource web-client --type frontend --stack shooter --yes`, `flisk up shooter --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md)
