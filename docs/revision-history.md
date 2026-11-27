# Revision history — SAMPLE-CA-001 (sample assembly)

One line per released revision. A revision is only recorded here after its
ECN is released — never before.

| Revision | Date | ECN | What changed |
| --- | --- | --- | --- |
| A | 2026-10-15 | — (initial release) | First release of the BOM and MPS for the sample assembly. |
| B | 2026-11-03 | SAMPLE-ECN-001 | Connector changed on both ends (see ECR log SAMPLE-ECR-001). BOM lines 30 and 40 updated; MPS routing step updated. |

## Rules

1. The revision letter only moves when a released ECN says so.
2. An ECR that is still "Under review" never changes the revision.
3. A change with no BOM impact (e.g. an MPS-only step) is logged in the
   ECR/ECN log but does not move the BOM revision.
4. If two changes land together, they share one new revision and both ECNs
   are listed on that line.
