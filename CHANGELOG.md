# Changelog

Public record of changes to aiconsumerrights.org, written from the product page on shipitworks.com. The source is private. Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Release tags exist on the private repository's default branch.

## 2026-11-08 (release v0.3.0)

- 2026-11-08: Rescored under the new feature rule: each of 10 features is worth 2.5 of 25. 2 count as proven by a logged run (Algorithm Decision Explorer; forum voting on a local Postgres 17, not the real database), 7 as built and tested with sample data, 1 not built. Score 78/100 on our own rubric (was 80/100 on the old rule). Ops line corrected: CHANGELOG.md exists. Tag v0.3.0 is on main.
- 2026-11-08: California help text now says the 45 days can reach 90 if the business tells you it needs longer, in 8 languages; new run npm run proof:help-numbers compares help-page numbers with their sources: 29 of 30 found, exit 1 (EU 12 months not on its cited page). PR #81, tag v0.3.0. CI moved to a self-hosted runner, PR #79.

Score 78 / 100 on our own rubric, scored 2026-11-08. Product page: https://shipitworks.com/aiconsumerrights/

## 2026-11-07 (release v0.2.0)

- Recorded runs on a local production build, not the live site: the dispute-kit deadline tracker keeps its list on the device, survives a reload and clears (Chrome); the Algorithm Decision Explorer browser run in 8 languages; and the help tools made no off-site request, no write and no request carrying typed text (575 requests, 13 routes, Chrome 157). Each check also failed when a fault was planted.
- Forum: suggesting a statement, reporting it, and the forum_voter cookie behave as the privacy page says, on a throwaway local Postgres 17, not the real database. Release v0.2.0.

Score 80 / 100 on our own rubric, scored 2026-11-01; no score or proof label changed in this update. Product page: https://shipitworks.com/aiconsumerrights/
