# Smart toilet control from the desktop

**Target:** A WeChat mini-program controlled smart toilet (device details not published by the author)
**Goal:** Open and close the lid from a computer and extend control to other home devices
**Status:** Idea
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The author used REA and Codex to analyze the mini-program's Bluetooth communication (author report).
- No protocol details are published in the case, so the findings are not reproducible from it.

Source case and evidence: https://x.com/thinkszyg/status/2109526361971073103

## What Flisk built

Not built yet. Proposed stack:

- Stack idea: `device-gateway` (Bluetooth bridge), `control-api` (HTTP endpoints for the desktop control), `status-ui`.
- Commands: `flisk project --yes`, `flisk resource device-gateway --type backend --stack home --yes`, `flisk up home --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on the target, and save `findings.md`.
2. Follow [prompts/flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md)
