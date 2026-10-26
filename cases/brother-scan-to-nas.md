# Brother scan button to NAS, SMB, FTP and S3

**Target:** Brother MFC-L2800DW scanner (firmware 1.32 tested by the original author), Scan to PC button software
**Goal:** Receive scans from the printer and store them in SMB, FTP, S3 or a local folder without a PC running Brother software
**Status:** Idea
**Author:** not applicable (summarized from the source below)
**Date:** 2026-10-19

## What REA found

- REA and Ghidra were used on Brother's Linux brscan5 library (libLxBsScanCoreApi), per the original project's README and author thread.
- Protocols identified in prior work: NETserver and BRPhoenixConnection (from the macOS Push Scan Tool).
- Scan events arrive as UDP messages; the project implements the registration and panel formats.

Source case and evidence: https://github.com/aurimasniekis/go-brother-scan-to-network-server

## What Flisk built

Not built yet. Proposed stack:

- Stack idea: `scan-receiver` (UDP listener and registration), `storage-adapter` (SMB, FTP, S3, local), `web-ui` (settings).
- Commands: `flisk project --yes`, `flisk resource scan-receiver --type backend --stack scan --yes`, `flisk resource storage --type backend --stack scan --yes`, `flisk up scan`.

## How to reproduce

1. Follow [prompts/rea-analyze-app.md](../prompts/rea-analyze-app.md) on the target, and save `findings.md`.
2. Follow [prompts/flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md) to create the stack.

## What did not work

- Not tried yet. Add results when someone builds it.

## Reuse

- Prompts: [rea-analyze-app.md](../prompts/rea-analyze-app.md), [flisk-scaffold-from-findings.md](../prompts/flisk-scaffold-from-findings.md)
