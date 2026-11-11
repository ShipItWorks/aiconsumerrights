# AI Consumer Rights

Plain-language help with your rights when AI makes decisions about you.

**Score: 78 / 100** on our own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-10; this record was updated 2026-11-10 from the [product page](https://shipitworks.com/aiconsumerrights/).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Web (aiconsumerrights.org) and an Android app that is not on Google Play yet.

## What works today

- Situation guides + rights by country (help pages) (Tested with sample data)
- Dispute-kit letter (fill in, copy, mailto) (Tested with sample data)
- Algorithm Decision Explorer (3 steps) (Proven)
- Forum voting API + consensus across language groups (Proven)
- Suggest a statement (140 chars) + automated precheck + report (Tested with sample data)
- Admin review page (Tested with sample data)
- Privacy page, sources page, how-it-works page (Tested with sample data)
- 8 languages (Tested with sample data)
- Live site reachable (Tested with sample data)

## Not done yet

- Installed Android app (Not built)
- Forum voting, suggesting and reporting ran on a throwaway local Postgres 17 on 2026-11-07, not against the real Neon DB or a real sign-in; the admin page is tested only against mocks/jsdom
- The automated precheck call to OpenRouter was not exercised in any recorded run (key removed, proof/suggest-and-report.log), and no recorded run presses the dispute-kit mailto action
- Numbers on the help pages were compared with archived copies of their sources on 2026-11-08: 29 of 30 passages found; the EU 12 months is not on its cited page (proof/help-numbers.log, exit 1). Not legal review
- No signed Android release, and assetlinks.json still lacks the Play App Signing SHA; Play status unknown
- Translations in all 8 languages are unreviewed by native speakers (README.md:39); legal content unreviewed
- No TalkBack run. Chrome 157 runs on a local build (2026-11-07) traced the help tools and dispute kit (13 routes, 575 requests, none off-site, none carrying the typed text) and exercised the deadline tracker in 8 languages; the live site and the Android app were not traced (not yet traced)
- Human moderation of suggested statements is a manual process, not exercised
- Public contact is feedback@/reviewers@aiconsumerrights.org, not support@shipitworks.com (plan rule 14) - owner decision

## What changed

- 2026-11-10: Site copy only: a dated correction now sits under the demo video for the narration line at 1:27. No code or score change.
- 2026-11-10: Land PR #84 merged into main as c369e47 (55 lane PRs included); no feature label changed this round. Tagged v0.4.0 at c369e47.
- 2026-11-08: Rescored under the new feature rule: each of 10 features is worth 2.5 of 25. 2 count as proven by a logged run (Algorithm Decision Explorer; forum voting on a local Postgres 17, not the real database), 7 as built and tested with sample data, 1 not built. Score 78/100 on our own rubric (was 80/100 on the old rule). Ops line corrected: CHANGELOG.md exists. Tag v0.3.0 is on main.
- 2026-11-08: California help text now says the 45 days can reach 90 if the business tells you it needs longer, in 8 languages; new run npm run proof:help-numbers compares help-page numbers with their sources: 29 of 30 found, exit 1 (EU 12 months not on its cited page). PR #81, tag v0.3.0. CI moved to a self-hosted runner, PR #79.
- 2026-11-07: Recorded runs on a local production build, not the live site: the dispute-kit deadline tracker keeps its list on the device, survives a reload and clears (Chrome); the Algorithm Decision Explorer browser run in 8 languages; and the help tools made no off-site request, no write and no request carrying typed text (575 requests, 13 routes, Chrome 157). Each check also failed when a fault was planted.
- 2026-11-07: Forum: suggesting a statement, reporting it, and the forum_voter cookie behave as the privacy page says, on a throwaway local Postgres 17, not the real database. Release v0.2.0.

See [CHANGELOG](CHANGELOG.md).

## Demo

[Demo video (1:58) on the product page](https://shipitworks.com/aiconsumerrights/) · [Transcript](https://shipitworks.com/aiconsumerrights/transcript/)

The demo voice is AI-generated (ElevenLabs, "Alice") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README and a CHANGELOG, and soon a LICENSE. Until the source is public, the [product page](https://shipitworks.com/aiconsumerrights/) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.
