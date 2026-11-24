---
name: audit-board
description: Summarize the open items on a Keldyn audit board.
---

# Audit board

1. Call `list-frameworks` when the user has not named a framework.
2. Call `get-audit-board` for that framework. If several boards match, ask which one to open.
3. Summarize the board counts and the open controls returned by the tool.
4. Call `get-audit-board-control` only for a control the user asks about.
5. Do not change audit state, evidence, or comments.
