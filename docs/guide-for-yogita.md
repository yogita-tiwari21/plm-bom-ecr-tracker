# Guide — how to fill this tracker in (for Yogita, walked through by Anuradha)

A 30-minute walkthrough. Do it with the sample data first, then replace the
sample rows with your own generic examples.

## Step 1 — Read the sample BOM (5 min)

Open `data/bom_template.csv`. It is one finished RF cable assembly, top to
bottom: the assembly itself, the cable, two connectors, sleeves, and a label.
Notice each line has a revision — that is what makes the BOM traceable.

## Step 2 — Raise a change the right way (10 min)

Pick a small change — for example, a different generic connector. Before
touching the BOM:

1. Add a row to `data/ecr_ecn_log.csv` with the reason and the impact.
2. Leave the status as "Under review" and the revision unchanged.

That is the habit the repo is showing: change first, BOM second.

## Step 3 — Release it (10 min)

Once the change is approved:

1. Update the affected BOM lines and move the revision letter (A → B).
2. Mark the ECR row "Released" and fill in the ECN number.
3. Add one line to `docs/revision-history.md` with the date and ECN.

## Step 4 — Run the governance checklist (5 min)

Work through `docs/data-governance-checklist.md`. If a box fails, the release
waits — that is the point of the checklist, and it is worth saying so in an
interview: the tracker exists to stop an unapproved change reaching
manufacturing.

## What not to put in here

No real part numbers, no customer names, no employer specs, no prices. If a
row would only make sense with real company data, rewrite it as a generic
sample instead — the structure is the portfolio piece, not the data.
