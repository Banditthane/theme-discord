---
name: cawf-refresh-module
description: >
  Refresh exactly one stale module card and its snapshot records from current evidence.
---


# Refresh One Module

1. Read module card, module-map entry, snapshot baseline and relevant changed paths.
2. Use `module_mapper` for one module only.
3. Update purpose, paths, interfaces, dependencies, state ownership, validation, risks and verification evidence.
4. Update direct dependency edges and snapshot metadata when affected.
5. Validate JSON maps; never rebuild unrelated cards/modules.
