---
name: cawf-close
description: >
  Close a CAWF v4 run with truthful criteria, verification, telemetry report, and residual risks.
---

# Close Run

1. Confirm no active task or unresolved required approval.
2. Record model usage from available Codex/provider usage when known; never invent it.
3. For each task verify scope, inferred approvals, current budget, all criterion evidence and required verification level with `cawf accept`. Then run `cawf report --run-id <run>`; a passing later task cannot hide an earlier failure.
4. Reconcile task results, reviews, integration report, Git diff, and telemetry caveats.
5. Mark completed/partial/failed/cancelled honestly.
6. Save final report with changed files, commands, failures, skipped checks, risks, scope deviations, budget blocks, exact/estimated token fields, and unsupported telemetry coverage.
