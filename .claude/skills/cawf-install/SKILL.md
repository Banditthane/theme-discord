---
name: cawf-install
description: >
  Install or synchronize CAWF provider integration for Codex CLI and Claude Code inside Product Root while keeping managed provider files outside ordinary product write scope.
---
# CAWF Install

Use when bootstrapping or refreshing the Product-Root provider layer.

1. Confirm `CAWF/` and `SRC/` are sibling roots.
2. Run `CAWF/cawf-install` (Windows: `CAWF\\cawf-install.cmd`) with `--provider all` unless the user requests one provider.
3. Write only managed provider files under `SRC/` during installation; preserve product source. Bundled production MCP SDK avoids downloads when complete; browser remains an explicit option.
4. Preserve user-modified provider files unless `--force` was explicitly requested.
5. Verify with `cawf provider status`, then `cawf doctor codex` / `cawf doctor claude` when the respective CLI is available.

Installed provider layer: `SRC/.agents/`, `SRC/.codex/`, `SRC/.claude/`, `SRC/AGENTS.md`, `SRC/CLAUDE.md`. CAWF dependencies/runtime and canonical provider sources remain inside `CAWF/`.
