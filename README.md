# AI Consumer Rights

Plain-language help with your rights when AI makes decisions about you.

Paused since 18 November 2026, while I finish patchowner. See [patchowner](https://shipitworks.com/patchowner/).

**Score: 78 / 100** on my own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-12; this record was updated 2026-11-18 from the [product page](https://shipitworks.com/aiconsumerrights/).

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

- 2026-11-12: Merged into the product: the sentence on the dispute kit page that said everything stays on your device, and the line on the help letter that said what you type is not sent or saved, were taken out and replaced with a plain statement that the letter is built in your browser as you type (this does not change the privacy page, and no network trace was run here); every law on the law-changes page now shows when it was last checked, by whom, and whether the official source still gave the same date or could not be opened; and each complaint route on the help page shows the day its source was read, with Italy, France and Germany listed under their own headings. This scorecard round did not run any of it, so no feature label or score changed (PRs #98, #99 and #103).
- 2026-11-11: Merged into the product: a link on the dispute letter that opens it in your own email app (it was not clicked in a real email app, and some apps cut long links); a tracker of dated rule changes under the comparison on the guide page (a named person re-reads the sources on a schedule; nothing watches them automatically); and an archived copy with a fingerprint for the last of the 96 sources on the sources page. Proof scripts and automated checks were also added, including for the AI helper and the send-the-letter option; the AI helper still has no real-model run recorded, and no real letter sent through the live site is recorded. This scorecard round did not run any of it, so no feature label or score changed (PRs #97, #92, #88, #91 and #94). Scorecard row: "Dispute-kit letter (fill in, copy, mailto)" (works true, Tested with sample data) covers the letter link; the rule tracker, the archived-source fingerprints and the proof scripts are not scored (no row covers them).
- 2026-11-11: Merged into the site's code, as its change titles describe them: an option to send the dispute letter from the dispute kit, an AI helper on the help page that stays off until it is switched on, and archive fingerprints on the sources page. This scorecard round did not run them, so no feature label or score changed (PRs #87 and #86).
- 2026-11-10: Site copy only: a dated correction now sits under the demo video for the narration line at 1:27. No code or score change.
- 2026-11-10: Land PR #84 merged into main as c369e47 (55 lane PRs included); no feature label changed this round. Tagged v0.4.0 at c369e47.
- 2026-11-08: Rescored under the new feature rule: each of 10 features is worth 2.5 of 25. 2 count as proven by a logged run (Algorithm Decision Explorer; forum voting on a local Postgres 17, not the real database), 7 as built and tested with sample data, 1 not built. Score 78/100 on our own rubric (was 80/100 on the old rule). Ops line corrected: CHANGELOG.md exists. Tag v0.3.0 is on main.

See [CHANGELOG](CHANGELOG.md).

## Demo

[Demo video (2:02) on the product page](https://shipitworks.com/aiconsumerrights/) · [Transcript](https://shipitworks.com/aiconsumerrights/transcript/)

The demo voice is AI-generated (ElevenLabs, "Bella") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README and a CHANGELOG, and soon a LICENSE. Until the source is public, the [product page](https://shipitworks.com/aiconsumerrights/) is the source of truth, and the score above is the one to trust.

## How I work

I say only what I can back. I say what is not finished before anyone asks. I name people, companies and tools to give credit. I collect as little data as possible. Built with Claude, by Anthropic: Claude helps write the code and wrote this README. Directed, tested and owned by Robert Sweetman in Stoughton, Massachusetts.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.
