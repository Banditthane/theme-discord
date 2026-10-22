---
name: cawf-plan
description: >
  Plan routed work into the smallest dependency-aware task packs and explicit approval gates.
---


# Plan Work

1. Preconditions: route is STANDARD, FULL or ARCHITECTURE and relevant snapshot facts are usable.
2. Read request, route decision, snapshot fragments and focused unknowns only.
3. Produce `impact-map.json`, `plan.md`, task graph and schema-valid task packs.
4. Each pack declares exact context routes, path scopes, budgets, criteria, commands, approvals and stop conditions.
5. Mark tasks `BLOCKED`, `READY`, or `AWAITING_APPROVAL` in canonical run state.
6. Serialize overlapping writes; parallelize only disjoint, independent tasks.
7. Prefer fewer coherent tasks and update one `next_action` in run state.
