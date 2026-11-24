---
name: evidence-gaps
description: Find Keldyn controls that still need evidence and explain the gap from the live record. Use when the user asks which controls are incomplete, insufficient, or missing evidence.
---

# Evidence gaps

1. Call `list-frameworks` when the user has not named a framework.
2. Call `list-controls` for the signed-in team. Prefer the gap or insufficient-evidence filters, and pass `useCaseId` only when the user named a use case.
3. Follow `nextCursor` until the pages the user asked for are covered, or report that more pages remain.
4. For each control you discuss in detail, call `get-control` and use its tracking status, acceptance criteria, and linked finding.
5. Summarize only what those tools returned. Separate open gaps from controls that are already complete.
6. Do not call `update-control` unless the user asks to save evidence, and confirm the control and the text first.
