# Division 2 Community Data Hub

A community-driven hub for Tom Clancy's The Division 2 game data and tools.

Division 2 game data has traditionally been community-maintained in Google Sheets — a huge effort by dedicated contributors over the years. But spreadsheets are hard to build on: formats vary between sheets, automation is limited, and the data is tied to whoever owns the document. Division 2 Community Data Hub takes that same community effort and puts it into version-controlled, schema-validated, machine-readable CSVs — open source and designed to be consumed by any tool, not just ours. Contributions go through pull requests, so the data belongs to the community, not any single maintainer.

## What's here

- **[data](https://github.com/div2hub/data)** — Community-maintained Division 2 game data (weapons, gear, talents, attributes, mods, and more). Every CSV follows a documented schema with build-time validation — no empty cells, no ambiguous formats, no guesswork.

## Principles

- **Open data, open tools.** Game data should be a shared community resource, not locked behind any one person's spreadsheet. Tools built on this data are open source too.
- **Schema over convention.** Every CSV column has defined syntax, validated at build time. This isn't a suggestion — the build fails if the data doesn't conform. Consistent data means any developer can write a parser once and trust it.
- **Built for reuse.** The data library exists independently of any single tool. If you're building a DPS calculator, a gear optimizer, a build planner, or something we haven't thought of — the data is here for you.

## Contributing

We welcome contributors — whether you're filling in missing stats, correcting values, or building your own tools on top of the data.

- **Data contributions:** Fork [div2hub/data](https://github.com/div2hub/data), read the [CSV conventions](https://github.com/div2hub/data/blob/main/README.md), and open a PR. The validation pipeline will catch formatting issues before review.
- **Tool developers:** The data repo is designed as a git submodule you can pull into any project. Use it however you like.
- **Questions or ideas:** Open an issue on the relevant repo, or start a discussion.
