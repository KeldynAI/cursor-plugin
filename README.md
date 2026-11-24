# Keldyn Cursor plugin

Marketplace repository for the Keldyn Cursor plugin.

Import this repository as a Cursor team marketplace, or install the `keldyn` plugin from it. The plugin connects to the hosted MCP server at `https://mcp.keldyn.ai` and signs in with Keldyn OAuth.

## Layout

```text
.cursor-plugin/marketplace.json
plugins/keldyn/
```

Plugin contents live in `plugins/keldyn/`. See that folder's README for the rules, skills, agent, and commands.

## Validate

```bash
node scripts/validate-template.mjs
```
