---
name: cawf-resume
description: >
  Resume a v4 run from canonical state, active task context manifest, budget state, and current Git delta.
---

# Resume

1. Select run and read run-state only.
2. Load active task, direct dependency results/reviews, context manifest, budget state, snapshot metadata, and current runtime delta.
3. Do not replay conversation, all results, or raw logs.
4. If file hashes/state conflict, run incremental scan and repair/replan.
5. Continue with scoped runtime operations and retain existing budget accounting unless an approved task revision resets it.
