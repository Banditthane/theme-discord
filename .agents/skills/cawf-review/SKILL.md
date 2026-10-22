---
name: cawf-review
description: >
  Review a bounded change for correctness, regressions, contracts, state ownership, security, performance, and maintainability.
---
# General Review

Review the diff against task criteria and verified project contracts. Prioritize concrete defects and regressions over style commentary. Check direct dependents when public APIs, schemas, shared libraries, auth/permissions, build/CI, or persistence behavior changed. Escalate specialized security/architecture/database/UI review only when the change warrants it.
