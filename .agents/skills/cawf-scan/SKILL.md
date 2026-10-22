---
name: cawf-scan
description: >
  Refresh the deterministic Product Root index and stack/project-profile evidence for any supported software repository.
---
# Scan / Refresh General Snapshot

1. Prefer incremental `cawf scan`; use `--full` only for missing/stale baselines or explicit requests.
2. Index only Product Root (`SRC/`) and honor configured exclusions.
3. Read `.cawf/local/runtime/delta.json` to focus semantic refresh on changed modules/interfaces.
4. Run `cawf stack` to capture languages, frameworks, infrastructure, and project profiles.
5. Do not infer architecture or ownership from directory names alone; confirm with source/contracts/tests.
6. Keep generated snapshots as evidence, not ground truth.
