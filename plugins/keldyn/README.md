# Keldyn

Cursor plugin for the Keldyn security and compliance workspace.

The plugin connects Cursor to the hosted MCP server at `https://mcp.keldyn.ai`. The first use opens Keldyn sign-in. Tools then run as that user. There is no API token to paste into the plugin.

## Included

- `mcp.json`: remote Keldyn MCP server
- `rules/keldyn-records.mdc`: how to read and update Keldyn records
- `skills/keldyn-workspace/`: general workspace usage
- `skills/evidence-gaps/`: controls that still need evidence
- `agents/compliance-reviewer.md`: review a change against live controls
- `commands/evidence-gaps.md` and `commands/audit-board.md`

Trust center images and signed contract files stay in the Keldyn web app.
