# LG PlxNative: a faster Plex client on LG TVs

**Target:** LG TV native media stack and Plex client
**Goal:** Test a faster native Plex-style client against a local media server
**Status:** Reported (popular, not REA)
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The developer used Ghidra and Claude Code to investigate the TV's native media stack (case summary).
- The author reports user-selection time falling from 30 seconds to 3 seconds (author claim, not measured here).

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/lg-plxnative.md

## What TDK built

Not built yet. Proposed stack:

- Stack idea: `media-server` (a local Plex-compatible API stub for testing), `client-test-ui`.
- Commands: `tdk project --yes`, `tdk resource media-server --type backend --stack tv --yes`, `tdk up tv --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md)
