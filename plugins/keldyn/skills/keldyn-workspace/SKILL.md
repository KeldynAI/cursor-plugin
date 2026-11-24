---
name: keldyn-workspace
description: Use the signed-in Keldyn workspace through the Keldyn MCP server for controls, evidence, audits, documents, risks, tasks, and organizational knowledge. Use when the user asks about Keldyn, compliance, frameworks, controls, audits, the trust center, or company policies.
---

# Keldyn workspace

The `keldyn` MCP server runs as the signed-in user. Read live tool results. Do not invent control status, evidence, findings, or policy text.

## Before you answer

1. If the team, framework, or use case is ambiguous, call `list-frameworks` or `list-use-cases` and ask which one to use.
2. Use list tools for a page of rows and the matching get tool for one record.
3. List tools are paginated. Follow `nextCursor` when the user needs more than the first page.

## Writes

Ask the user before a write. This includes `update-control`, task changes, `approve-build-document`, trust center publishing, and changes to the risk, data, or third-party registers.

Trust center images and signed contract files are uploaded in the Keldyn web app. Do not claim those files were uploaded from chat.

## Common jobs

- Evidence gaps: `list-controls` with the gap or insufficient-evidence filters, then `get-control` for one control.
- Audits: `get-audit-board`, then `get-audit-board-control` for one control.
- Policies and context: `search-knowledge` or `answer-knowledge`. Use `list-build-documents` for drafted policy documents.
- Use cases and architecture: `list-use-cases`, then `get-use-case`.

If a tool returns an authorization error, ask the user to reconnect Keldyn. Do not retry with a different team or a guessed id.
