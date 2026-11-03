# AI Consumer Rights

Plain-language help with your rights when AI makes decisions about you.

**Score: 80 / 100** on the [ShipItWorks rubric](https://shipitworks.com/how-we-score/). Stage: Beta. As of 2026-11-02, from the [product page](https://shipitworks.com/aiconsumerrights/).

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

- Forum voting API and the admin page are proven only against mocks/jsdom, never against the real Neon DB or a real sign-in
- No signed Android release, and assetlinks.json still lacks the Play App Signing SHA; Play status unknown
- Translations in all 8 languages are unreviewed by native speakers; legal content unreviewed
- No real-browser or TalkBack run; 'nothing leaves your device' on the dispute kit is not confirmed by a network trace
- Human moderation of suggested statements is a manual process, never exercised
- Some of its pages still show an old contact email; they need to point to support@shipitworks.com

## Demo

[Demo video (1:58) on the product page](https://shipitworks.com/aiconsumerrights/) · [Transcript](https://shipitworks.com/aiconsumerrights/transcript/)

The demo voice is AI-generated (ElevenLabs, "Alice") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README, and soon a CHANGELOG and LICENSE. Until the source is public, the [product page](https://shipitworks.com/aiconsumerrights/) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.
