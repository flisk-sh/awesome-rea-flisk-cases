# NJFE: ear camera on the PC as an inspection scope

**Target:** Hopefox Find T Wi-Fi ear camera (one device tested by the project)
**Goal:** Bridge the camera stream to a PC viewer
**Status:** Idea
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- The NJFE project documents protocol work built on the GPL otoscope project (rbeilvert/otoscope); credits are in its README.
- The camera Wi-Fi is open and unauthenticated, per the project README.

Source case and evidence: https://github.com/WildweaselMS/NJFE

## What TDK built

Not built yet. Proposed stack:

- Stack idea: `camera-bridge` (USB bridge logic), `viewer` (PC web viewer), `recorder` (saves frames).
- Commands: `tdk project --yes`, `tdk resource camera-bridge --type backend --stack scope --yes`, `tdk up scope --dry-run`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on the target, and save `findings.md`.
2. Follow [prompts/tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [tdk-scaffold-from-findings.md](../prompts/tdk-scaffold-from-findings.md)
