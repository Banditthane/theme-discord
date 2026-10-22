---
name: cawf-ui
description: >
  Plan and verify generic web/UI changes with bounded browser evidence, accessibility, responsive behavior, and API boundary awareness.
---
# CAWF Generic UI

Use for React/Vue/Svelte/HTML/CSS or similar UI tasks. Keep visual-only changes in the UI layer. Trace API/state changes only when behavior requires them.

Before substantial implementation define: user goal/flow, component hierarchy, interaction states, responsive constraints, accessibility, performance risks, data/API contracts, and acceptance criteria.

Use Browser MCP only when runtime visual/DOM evidence materially improves verification; keep it opt-in and bounded.
