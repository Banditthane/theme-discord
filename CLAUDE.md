@AGENTS.md

# Claude Code adapter

CAWF supports Claude Code as a first-class client alongside Codex CLI.

- Provider files are installed by `cawf-install` inside Product Root (`SRC/.agents`, `SRC/.codex`, `SRC/.claude`, `SRC/AGENTS.md`, `SRC/CLAUDE.md`); canonical copies remain under `CAWF/` for deterministic synchronization.
- Use project subagents in `.claude/agents/` only for bounded delegation; no nested delegation by default.
- Prefer one implementer/writer at a time and parallelize independent read-only analysis.
- `SRC/` is Product Root and normal working directory. Do not edit `CAWF/` or the managed provider paths under `SRC/` during ordinary product work.
- Use `CAWF_CONTROL_ROOT`, `CAWF_WORKSPACE_ROOT`, `CAWF_PRODUCT_ROOT`, and `CAWF_ACTIVE_ROOT`; do not assume `.cawf` exists in the current working directory.
- Keep MCP strict and task-scoped. Safe mode hides mutation tools; full mode remains approval-gated. Browser and guarded shell are opt-in.
- If Claude Code behavior is version-sensitive, preserve the generic CAWF contract and verify the installed client before changing adapter-specific syntax.
