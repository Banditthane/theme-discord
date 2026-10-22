---
name: cawf-execute
description: >
  Execute one approved READY v4 task with prepared context, runtime-observed evidence, hard budgets, and compressed results.
---

# Execute Task

1. Read run state, selected task, direct dependency results, and relevant snapshot fragments only.
2. Confirm scope, operations, inferred approvals and budgets. Record only actual user authorization; approval grants bind to task scope/policy.
3. Run `cawf prepare-task --run-id <run> --task <task>` and inspect its manifest.
4. For a write task run `cawf scope begin --run-id <run> --task <task>` before editing. Prefer the primary agent as the single writer; delegation is optional and must follow user/provider instructions. Supply complete context to any explicitly delegated worker.
5. Additional reads/searches must use runtime commands and exact ranges/patterns.
6. If runtime blocks required scope/budget, save expansion request and stop.
7. Run specified validation through `cawf run` where possible.
8. Run `cawf scope verify`, then `cawf budget`; save complete criterion evidence, validation results and budget references in the result pack. Create a matching verification report before `cawf accept`.
9. Update run state atomically and checkpoint after repeated failure, changed assumptions, or saturation.
