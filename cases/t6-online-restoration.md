# Call of Duty: Black Ops (T6) rollback and online play

**Target:** Discontinued T6 multiplayer service
**Goal:** Restore usable online play with a community-run backend
**Status:** Needs verification
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The case records a community discussion, not a development log; no protocol, repository, or build is supplied.
- Treat any claim of restored online play as unverified.

Source case and evidence: https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/t6-ai-rollback-online-restoration-report.md

## What TDK built

Not built yet. Proposed stack:

- Stack idea: `lobby-server`, `match-server`, `stats-db` (Postgres), all run locally.
- Commands: `tdk project --yes`, `tdk resource lobby-server --type backend --stack t6 --yes`, `tdk resource stats-db --type bring-your-own --stack t6 --yes`, `tdk up t6 --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on a target you may analyze, and save `findings.md`.
2. Follow [prompts/tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md)
