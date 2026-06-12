# Envelope — Claude Code Skill

A Claude Code skill that teaches Claude how to create valid `.envelope.json` team definition files — the open standard for AI agent teams.

## What this skill does

When installed, Claude Code can:

- Design multi-agent teams from a natural-language description
- Generate schema-valid `.envelope.json` files ready to deploy
- Explain the `reportsToKey` hierarchy, `accessPolicy` rules, gates, and other schema concepts
- Validate definitions against the published JSON schema

## Install

```sh
claude mcp add https://raw.githubusercontent.com/openenvelope/claude-plugin/main/.claude-plugin/plugin.json
```

Or find it on [buildwithclaude.com](https://buildwithclaude.com) — search for **Envelope**.

## Usage

After installing, just describe the team you want:

```
Build me an Envelope team for customer support triage — one supervisor,
two agents that read Zendesk tickets, and a Slack notifier for escalations.
```

Claude Code will generate a `.envelope.json` file you can deploy directly via the [Envelope UI](https://openenvelope.org) or the [Envelope API](https://openenvelope.org/api-docs).

## Links

- [openenvelope.org](https://openenvelope.org) — deploy and run teams
- [schema.openenvelope.org/team/v1.json](https://schema.openenvelope.org/team/v1.json) — JSON schema
- [npmjs.com/package/@openenvelope/schema](https://www.npmjs.com/package/@openenvelope/schema) — TypeScript types + validator
- [openenvelope.org/mcp](https://openenvelope.org/mcp) — MCP reference for running teams programmatically
