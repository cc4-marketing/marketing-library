# Meta Title and Description Writer

**Type:** Slash Command &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/seo/meta-title-description-writer/](https://cc4.marketing/library/seo/meta-title-description-writer/)

_Write SERP length checked title and description pairs that fit Google._

A great title tag that gets cut off at 61 characters is a wasted title tag. This command writes title and description pairs, checks the length of each, and shows the count so you can pick one that fits Google without truncation. It writes several options per page so you have variety to test.

## The command

Save this as `.claude/commands/meta.md` in your project.

```markdown
---
description: Write SERP length checked title and meta description pairs.
argument-hint: [page topic or target keyword]
---

You are an SEO copywriter. The page topic or target keyword is: $ARGUMENTS

Write 5 title and meta description pairs for this page. Rules:

- Title: 60 characters or fewer. Include the primary keyword near the front.
  Make it click worthy, not clickbait.
- Description: 155 characters or fewer. Expand on the title, add a specific
  benefit or detail, and end with a light call to action.
- Do not stuff keywords. Each pair should read like a human wrote it.
- Vary the angle across the 5 pairs (benefit led, question led, how to led,
  comparison led, urgency led).

Format each pair like this:

Pair 1
Title (NN chars): the title text
Description (NNN chars): the description text

Replace NN and NNN with the actual character counts you measured. Count
characters including spaces. If any line is over the limit, rewrite it before
you output, do not output an over-limit line.

After the 5 pairs, name which pair you would ship and why, in one sentence.
```

## How to use

1. Save the block above as `.claude/commands/meta.md`.
2. Run `/meta claude code for marketing teams` (swap in your page topic).
3. Check the character counts: if a line looks long, ask Claude to tighten it.
4. Drop the winning pair into your CMS or head tags, then move to the next page.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [SEO](https://cc4.marketing/library/seo/) entries.
