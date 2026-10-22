---
name: cawf-route
description: >
  Classify a request into the smallest safe CAWF route before planning or broad inspection.
---


# Route Request

1. Read request, config, snapshot index/metadata and minimal Git status.
2. Use `router` to produce `route-decision.json`.
3. Select `DIRECT`, `STANDARD`, `FULL`, or `ARCHITECTURE` from evidence and risk flags.
4. Require snapshot refresh only when relevant routing facts are stale.
5. Do not create a plan or inspect implementation broadly during routing.
6. Re-route if later evidence materially changes scope or risk.
