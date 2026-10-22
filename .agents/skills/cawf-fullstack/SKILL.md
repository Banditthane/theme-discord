---
name: cawf-fullstack
description: >
  Plan cross-layer full-stack changes across UI, API/service, persistence, validation, tests, and deployment boundaries without losing ownership or contract clarity.
---
# Full-Stack Change

Trace the request end-to-end: user flow -> UI state -> API/transport -> application/domain logic -> persistence -> observable result. Identify the authoritative validation/state owner at each boundary. Split work by independent ownership only when useful; keep contract changes explicit and verify both producer and consumer. Avoid changing database/API/UI simultaneously without a minimal integration plan.
