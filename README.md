# Shikshagraha partner ecosystem — dashboard

A single self-contained page showing the partner ecosystem of the Shikshagraha
movement: where partners work, what stage each relationship is at, and — just as
importantly — what the underlying data cannot tell you.

**Live:** https://anishsaha-cell.github.io/shikshagraha-partner-dashboard/

## What this repository is

Build output, and nothing else. `index.html` is generated — every page, style
and record inlined into one file with no server, no network calls and no
dependencies. Editing it here is pointless: the next build overwrites it.

The source, the data pipeline and the checks live in a private repository
maintained by the ShikshaLokam ecosystem team.

## Reading the numbers honestly

The dashboard is built on a working copy of the team's partner tracker, and it
is deliberate about its own gaps rather than hiding them:

- **A blank means a blank in the tracker.** Nothing is inferred, averaged, or
  filled with a plausible value.
- Three things are absent for *every* partner because no column records them:
  stage-entry dates, engagement level, and block-level geography. The pages say
  so in place instead of rendering an empty timeline that reads as
  "nothing happened".
- Not every partner has geography recorded, so the map shows fewer partners than
  the total. The banner on the map says how many are missing.
- District names come from hand-typed tracker cells. Those that cannot be
  matched to a real district are shown on their state's page rather than being
  silently dropped.

The **Coverage** tab in the dashboard is the full accounting. Read it before
quoting any number from this page.

## Provenance

Stage definitions come from the team's own *Partner Stages & Engagement Menu*:
Stage 1 Aware · Stage 2 Understanding · Stage 3 Aligned · Stage 4 Contributing ·
Stage 5 Champion. Map boundaries are ShikshaLokam's own India map, as used in the
Shikshagraha dashboard.

Contact details, individuals' names and financial figures are excluded by an
automated check that runs on every build and blocks publication if it finds any.
