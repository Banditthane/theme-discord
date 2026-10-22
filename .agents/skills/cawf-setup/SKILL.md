---
name: cawf-setup
description: >
  Initialize or validate a General SoloDev CAWF workspace, Product Root, provider layer, and detected project stack.
---
# CAWF Setup

Use for first-run setup or after moving CAWF to another workspace.

- Ensure `SRC/` exists as Product Root.
- Run `CAWF/cawf-setup --auto` (Windows: `CAWF\\cawf-setup.cmd --auto`).
- Inspect `cawf workspace` and `cawf stack`.
- Do not install project dependencies, mutate project source, or change architecture merely because stack detection found a framework.
- Run `cawf scan --full` only when establishing the first baseline; use incremental `cawf scan` afterwards.
