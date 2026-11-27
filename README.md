# PLM BOM & ECR Tracker

A clean, ready-to-use tracker for RF cable assemblies — BOM, engineering change
(ECR/ECN), revision history, and a data-governance checklist — built around the
day-to-day work of a Technical Product Coordinator (RF) in SAP / PLM.

> **Sample data only.** Every part number, customer name, and quantity in this
> repo is fictional and illustrative (prefixed `SAMPLE-`). No real employer part
> numbers, customer specs, or company data are used. Replace the sample rows
> with your own generic examples before sharing.

## What's inside

| File | What it is |
| --- | --- |
| `data/bom_template.csv` | BOM template for one RF cable assembly, with sample rows |
| `data/ecr_ecn_log.csv` | ECR/ECN log — one row per change request, with status and revision |
| `docs/revision-history.md` | How revision control works in this tracker |
| `docs/data-governance-checklist.md` | Checks to run before releasing a BOM or a change |
| `docs/guide-for-yogita.md` | Short walkthrough: how to fill this in, step by step |

## How it maps to the real work

- **BOM** — material master, product structure, routing, and revision for RF
  cables, connectors, and cable assemblies (SAP S/4HANA / PLM / PDM).
- **ECR/ECN** — engineering change requests and notices: what changed, why,
  who approved it, and which revision it landed in.
- **Revision history** — one line per released revision, so any BOM can be
  traced back to the change that produced it.
- **Data governance** — the checks that keep a BOM releasable: no duplicate
  part numbers, no missing fields, consistent revisions, approved changes only.

## How to use it

1. Copy `data/bom_template.csv` for each new assembly and fill in the real
   (generic) structure — see `docs/guide-for-yogita.md`.
2. Log every change in `data/ecr_ecn_log.csv` before editing the BOM.
3. Run the `docs/data-governance-checklist.md` checks before marking a
   revision released.
4. Record the release in `docs/revision-history.md`.

## Skills this shows

SAP S/4HANA · PLM / PDM · BOM & Material Master · ECR/ECN & configuration
management · NPI & revision control · data governance & traceability ·
RF cable assemblies & connectors
