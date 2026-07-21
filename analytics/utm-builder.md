# UTM Builder

**Type:** Slash Command &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/analytics/utm-builder/](https://cc4.marketing/library/analytics/utm-builder/)

_Build consistent UTM tagged URLs from your naming rules and flag drift._

UTM tags fall apart the moment two people write them freehand: Facebook and facebook and FB become three sources, and a campaign no longer sums in GA4. This command builds every link against one naming convention (lowercase, a fixed source and medium vocabulary, hyphen separators) and audits links you already have, flagging casing drift, freeform values, and missing tags. Reports stay clean because the links were clean going in.

## The command

Save this as `.claude/commands/utm.md` in your project.

```markdown
---
description: Build and audit UTM tagged URLs against a naming convention.
argument-hint: [base URL plus source, medium, campaign] or [paste links to audit]
---

You are an analytics engineer enforcing UTM hygiene. Input: $ARGUMENTS

House naming convention (apply and enforce all of it):
- Lowercase everything. No spaces: use hyphens inside a value.
- utm_source: the specific platform (google, facebook, linkedin, newsletter,
  partner-acme). One canonical spelling each.
- utm_medium: from this allowed set only: cpc, email, social, organic,
  referral, affiliate, display. Reject anything else and suggest the closest.
- utm_campaign: format {yyyy-mm}-{short-name} (for example 2026-07-summer-sale).
- utm_content: optional, for splitting variants (ad-a, ad-b, header-cta).
- utm_term: optional, for paid keywords only.

Two modes, pick by the input:

BUILD MODE (a base URL plus tag values):
- Output the full tagged URL on one line, ready to copy.
- Below it, list the final tag values so I can confirm.
- If a required tag (source, medium, campaign) is missing, ask before building.

AUDIT MODE (one or more existing tagged URLs pasted):
- For each URL, give a table: Tag, Value, Verdict (ok / fix), Corrected value.
- Flag: uppercase, spaces, a medium outside the allowed set, a source with a
  known variant spelling, a campaign not matching the date-name format, and
  any missing required tag.
- Then output the corrected URL on one line.

Always end with one line: the canonical source and medium these links roll up
to, so I can confirm they land in one bucket in GA4.
```

## How to use

1. Save the block above as `.claude/commands/utm.md`.
2. To build: run `/utm` with the base URL and your source, medium, and campaign values.
3. To audit: run `/utm` and paste links you already published to catch casing and vocabulary drift.
4. Paste the built URL into your ad, email, or social scheduler.
5. Keep the allowed medium set and source spellings in the command so every teammate builds to the same rules.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Analytics & Data](https://cc4.marketing/library/analytics/) entries.
