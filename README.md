# Awesome REA + TDK Cases

A curated collection of **reverse-engineering cases where an AI agent analyzes an app with [REA](https://github.com/morluto/rea), and [TDK CLI](https://github.com/tdk-landscape/tdk-cli-core) turns the findings into a local stack you can run.**

Each case answers three questions:

1. **What did REA find?** Behavior, APIs, data formats, or binary details, with evidence.
2. **What did TDK build?** The local services, data, and runtime that reproduce the app's useful behavior.
3. **What can you reuse?** The prompts and skills that made it work.

> **No cases yet.** This list starts empty on purpose. Add the first one: see [CONTRIBUTING.md](CONTRIBUTING.md).

## Workflow

```text
REA (agent + CLI/MCP)  →  findings.md  →  tdk project / tdk resource  →  tdk up  →  run and check
```

1. Point REA at the app or binary you are allowed to analyze.
2. Save the findings in a `findings.md` file: endpoints, formats, protocols, and open questions.
3. Use TDK to scaffold the services that match the findings, then start the stack with `tdk up`.
4. Record what worked and what did not in a case file.

Start with the prompts in [prompts/](prompts/).

## Browse

| Section | What is in it |
| :--- | :--- |
| [Cases](cases/) | One file per case, from the template in [cases/_template.md](cases/_template.md) |
| [Prompts](prompts/) | Reusable prompts for REA and TDK |
| [Skills](skills/) | Agent skills and setup notes that help REA and TDK work together |

## Scope and legal

- Only analyze software you own, have permission to analyze, or may analyze under the law where you live. Do not include proprietary assets, keys, credentials, or private data in a case.
- Summaries and links only. Describe evidence, do not paste whole binaries or copyrighted code.
- Cases report what the author observed. They are not independently verified unless the case says so.

## License

Curated content and code in this repository: [MIT](LICENSE). Linked projects keep their own licenses.
