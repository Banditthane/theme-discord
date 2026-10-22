---
name: cawf-benchmark
description: >
  Benchmark CAWF v4 against another run only after quality parity, using telemetry and recorded model usage.
---

# Benchmark

1. Require same repository revision, request, model/reasoning level, criteria, approvals, and quality gates.
2. Generate v4 telemetry report and obtain exact model usage when available.
3. Compare elapsed time, input/output, tasks/retries, unique/duplicate reads, searches, raw/compressed command bytes, verification scope, and findings.
4. Separate measured values from character/token estimates.
5. Do not claim percentage savings when exact usage or quality parity is missing.
