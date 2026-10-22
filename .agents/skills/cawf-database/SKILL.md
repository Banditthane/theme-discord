---
name: cawf-database
description: >
  Plan/review SQL/ORM/schema/migration changes with ownership, compatibility, rollback, data integrity, query performance, and read-only evidence safety.
---
# Database / Persistence

Identify state owner, transaction boundary, migration order, compatibility window, constraints/indexes, backfill/rollback strategy, query plans for risky paths, and affected readers/writers. Persistent schema changes require approval. Prefer static project evidence first; live DB access remains read-only and opt-in.
