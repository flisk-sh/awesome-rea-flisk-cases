# Awesome REA + Flisk Cases

**English** | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md)

A curated collection of **reverse-engineering cases where an AI agent analyzes an app with [REA](https://github.com/morluto/rea), and [Flisk CLI](https://github.com/flisk-sh/flisk) turns the findings into a local stack you can run.**

Each case answers three questions:

1. **What did REA find?** Behavior, APIs, data formats, or binary details, with evidence.
2. **What did Flisk build?** The local services, data, and runtime that reproduce the app's useful behavior.
3. **What can you reuse?** The prompts and skills that made it work.

## Cases

Status shows how far each case has gone. Cases below are taken from write-ups in the awesome-REA-cases list. The status column shows what the source supports. None has a Flisk build yet, and some REA claims are unverified.

| Case | Target | Status |
| :--- | :--- | :--- |
| [Brother scan button to NAS](cases/brother-scan-to-nas.md) | Brother scanner, SMB/FTP/S3 storage | Idea |
| [NJFE ear camera bridge](cases/njfe-ear-camera-bridge.md) | Wi-Fi ear camera on a PC | Idea |
| [Smart toilet control](cases/smart-toilet-desktop-control.md) | Bluetooth smart toilet | Idea |
| [Urban Terror in the browser](cases/urban-terror-browser.md) | Browser shooter (Quake III engine) | Reported, not REA |
| [LG PlxNative Plex client](cases/lg-plxnative-plex-client.md) | LG TV media client | Reported, not REA |
| [T6 online restoration](cases/t6-online-restoration.md) | Discontinued multiplayer backend | Needs verification |
| [Pre-CU Star Wars Galaxies emulator](cases/pre-cu-swg-emulator.md) | MMO server emulator | Needs verification |
| [The Incredible Machine in the browser](cases/incredible-machine-browser.md) | Browser puzzle game | Needs verification |
| [H1Z1: from reverse engineering to an MMO backend](cases/h1z1-mmo-backend.md) | H1Z1 | In progress |
| [Red Alert 2: an engine rewrite for reinforcement learning](cases/red-alert-2-rl-environment.md) | Red Alert 2 | Needs verification |
| [Animal Jam / Burrow: client and server](cases/animal-jam-burrow-client-server.md) | Animal Jam / Burrow | Needs verification |
| [Browser Counter-Strike: multiplayer in the browser](cases/browser-counter-strike-multiplayer.md) | Counter-Strike style multiplayer shooter | Needs verification |
| [Three Kingdoms XIV: trainer functions as an MCP server](cases/three-kingdoms-mcp-tools.md) | Romance of the Three Kingdoms XIV | Needs verification |
| [Hearthstone on macOS: game-control agent, deck optimizer and replay review](cases/hearthstone-macos-agent.md) | Hearthstone | Needs verification |
| [Mobile game interactions: an evidence pipeline with Codex and REA](cases/mobile-game-evidence-pipeline.md) | Mobile game | In progress |
| [Dragon Ball Budokai: browser port with a local game server](cases/dragon-ball-budokai-browser-port.md) | Dragon Ball Budokai | Needs verification |

Add one with [CONTRIBUTING.md](CONTRIBUTING.md).

### Related REA-only write-ups (no Flisk build)

- [Open Scrantic: Johnny Castaway in Rust](https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/johnny-castaway-rust-rea.md) (REA + Claude Code)
- [LeanREA: CLI skill vs REA MCP benchmark](https://github.com/songshikang0111/awesome-REA-cases/blob/main/cases/en/leanrea-cli-skill-benchmark.md) (author benchmark)
- More REA cases: [awesome-REA-cases](https://github.com/songshikang0111/awesome-REA-cases)

## Workflow

```text
REA (agent + CLI/MCP)  →  findings.md  →  flisk project / flisk resource  →  flisk up  →  run and check
```

1. Point REA at the app or binary you are allowed to analyze.
2. Save the findings in a `findings.md` file: endpoints, formats, protocols, and open questions.
3. Use Flisk to scaffold the services that match the findings, then start the stack with `flisk up`.
4. Record what worked and what did not in a case file.

Start with the prompts in [prompts/](prompts/).

## Browse

| Section | What is in it |
| :--- | :--- |
| [Cases](cases/) | One file per case, from the template in [cases/_template.md](cases/_template.md) |
| [Prompts](prompts/) | Reusable prompts for REA and Flisk |
| [Skills](skills/) | Agent skills, starting with [rea-to-flisk](skills/rea-to-flisk/SKILL.md) |

## Scope and legal

- Only analyze software you own, have permission to analyze, or may analyze under the law where you live. Do not include proprietary assets, keys, credentials, or private data in a case.
- Summaries and links only. Describe evidence, do not paste whole binaries or copyrighted code.
- Cases report what the author observed. They are not independently verified unless the case says so.

## License

Curated content and code in this repository: [MIT](LICENSE). Linked projects keep their own licenses.
