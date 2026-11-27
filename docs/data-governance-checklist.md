# Data-governance checklist — run before releasing a BOM or a change

Tick every box before marking a revision released. If any box fails, the
release waits.

## BOM checks

- [ ] No duplicate part numbers in the BOM.
- [ ] Every line has a description, quantity, unit, and revision.
- [ ] Every part number's revision matches the revision in the material master.
- [ ] Quantities are consistent with the assembly drawing / routing.
- [ ] No real employer part numbers or customer specs — sample data only.

## Change checks

- [ ] Every BOM edit traces to a released ECN in `data/ecr_ecn_log.csv`.
- [ ] The ECR states the reason, the impact, and the approver.
- [ ] Changes still "Under review" are not in the released BOM.
- [ ] The revision history records the new revision, date, and ECN.

## Release checks

- [ ] Revision letter moved exactly once for this release.
- [ ] MPS / routing updated where the change affects manufacturing.
- [ ] Old revision is kept (never overwritten) — history stays traceable.
