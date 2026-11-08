# AI Consumer Rights

Plain-language help with your rights when AI makes decisions about you.

**Score: 80 / 100** on our own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-01; this record was updated 2026-11-07 from the [product page](https://shipitworks.com/aiconsumerrights/).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Web (aiconsumerrights.org) and an Android app that is not on Google Play yet.

## What works today

- Situation guides + rights by country (help pages)
- Dispute-kit letter (fill in, copy, mailto)
- Algorithm Decision Explorer (3 steps)
- Suggest a statement (140 chars) + automated precheck + report
- Privacy page, sources page, how-it-works page
- Live site reachable

## Not done yet

- Forum voting, suggesting and reporting ran on a throwaway local Postgres 17 on 2026-11-07, not against the real Neon DB or a real sign-in; the admin page is proven only against mocks/jsdom
- No signed Android release, and assetlinks.json still lacks the Play App Signing SHA; Play status unknown
- Translations in all 8 languages are unreviewed by native speakers (README.md:39); legal content unreviewed
- No TalkBack run. A Chrome 157 run on a local build traced the help tools' requests (13 routes) and exercised the dispute-kit deadline tracker on 2026-11-07; the live site was not traced, and the dispute kit's own network use is not confirmed by a trace
- Human moderation of suggested statements is a manual process, not exercised
- Some of its pages still show an old contact email; they need to point to support@shipitworks.com.

## What changed

- 2026-11-07: Recorded runs on a local production build, not the live site: the dispute-kit deadline tracker keeps its list on the device, survives a reload and clears (Chrome); the Algorithm Decision Explorer browser run in 8 languages; and the help tools made no off-site request, no write and no request carrying typed text (575 requests, 13 routes, Chrome 157). Each check also failed when a fault was planted.
- 2026-11-07: Forum: suggesting a statement, reporting it, and the forum_voter cookie behave as the privacy page says, on a throwaway local Postgres 17, not the real database. Release v0.2.0.

Full list with release tags: [CHANGELOG](CHANGELOG.md).

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
