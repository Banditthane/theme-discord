---
name: cawf-context
description: >
  Build bounded, task-specific context from the deterministic Product Root index, exact dependencies/contracts, current diff, and on-demand source.
---
# Bounded Context

Use progressive disclosure: request -> route -> changed/affected modules -> direct contracts/dependencies -> exact source ranges -> targeted tests/runtime evidence. Separate readable paths from writable paths. Include API/schema/auth/state definitions before implementation when they constrain behavior. Avoid loading unrelated modules, generated output, secrets, or entire monorepos into every worker.

Context manifests use schema 1.2 and include `knowledge_packs` metadata. Project evidence has priority; report skipped pack entries when the budget is full. Omit `context.knowledge_packs` for automatic selection, set explicit IDs for this task, or `[]` for no domain references. Do not read all pack documents manually to bypass a context budget.
