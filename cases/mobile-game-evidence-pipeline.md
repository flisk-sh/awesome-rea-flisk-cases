# Mobile game interactions: an evidence pipeline with Codex and REA

**Target:** Mobile game (interaction recordings and client evidence)
**Goal:** Run a pipeline that stores, maps and reviews interaction evidence from REA and Codex
**Status:** In progress
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The case maps mobile-game interactions to evidence using Codex and REA (case summary).
- The evidence format is not given in the case, so the stack below is a plan.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/mobile-game-interaction-evidence.md

## What TDK built

Not built yet. Proposed app types and stack:

- Types: `backend` (evidence API), `worker` (maps recordings to interactions), `frontend` (review UI).
- Commands: `tdk project --yes`, `tdk resource evidence-api --type backend --stack evidence --yes`, `tdk resource mapper --type worker --stack evidence --yes`, `tdk resource review-ui --type frontend --stack evidence --yes`, `tdk up evidence --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md)
