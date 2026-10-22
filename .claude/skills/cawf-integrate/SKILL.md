---
name: cawf-integrate
description: >
  Integrate accepted results and verify cross-task compatibility without broad rereading.
---


# Integrate Run

1. Read run state, accepted task/result/review artifacts and integration-relevant snapshot fragments.
2. Confirm no unresolved overlap, unapproved scope expansion or missing dependency order.
3. Use `integrator`; run aggregate commands from snapshot commands map.
4. Verify public contracts, migrations, module boundaries and artifact ownership.
5. Save integration verification, update affected snapshot/module records if useful, and advance run state.
6. Ask before push, publish, release, deploy or destructive conflict resolution.
