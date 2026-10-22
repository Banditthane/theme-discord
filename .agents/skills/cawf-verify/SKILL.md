---
name: cawf-verify
description: >
  Verify accepted behavior with the smallest deterministic evidence set that matches impact and risk.
---
# General Verification

Verification order: diff/scope -> acceptance criteria -> static/type/schema checks -> affected unit/integration tests -> build/package checks -> runtime/API/UI/CLI smoke when relevant -> specialized review for high-risk changes. Public contracts, persistent schema, shared core, security/permissions, CI/deployment, destructive/external effects, and wide dependency impact trigger broader verification. Production/deployment mutations require explicit approval.
