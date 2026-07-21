# Newsletter Section from a Link

**Type:** Slash Command &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/email/newsletter-from-link/](https://cc4.marketing/library/email/newsletter-from-link/)

_Summarize a URL into a newsletter section with subject line and CTA._

The weekly newsletter dies from the effort of writing it. This command shrinks the mechanical part: give it a link and it returns a tight newsletter section that keeps your voice, plus a subject line and one call to action. You still choose what to feature. It handles the shaping so a send stops eating an afternoon.

## The command

Save this as `.claude/commands/newsletter.md` in your project.

```markdown
---
description: Turn a link into a newsletter section with subject line and CTA.
argument-hint: [URL or pasted article]
---

You are writing a section for a marketing newsletter. The source is: $ARGUMENTS

If given a URL, read it. Then produce:

1. Subject line: 3 options, each 50 characters or fewer, curiosity or benefit
   led, no clickbait.
2. Section body: 90 to 150 words. Open with why this matters to the reader,
   then the 2 or 3 things worth knowing, in plain language. Do not just
   summarize the source, tell the reader what to do with it.
3. Call to action: one line, one action (read the full piece, try the tool,
   reply with a take). Include the link.

Keep the voice conversational and specific. Attribute the source. Do not
invent facts that are not in the source. If the source is thin, say what is
missing and write the honest version anyway.
```

## How to use

1. Save the block above as `.claude/commands/newsletter.md`.
2. Run `/newsletter https://example.com/the-article-you-are-featuring`.
3. Pick one of the three subject lines, or ask for more in a different angle.
4. Edit the body to add your own take, then drop it into your email tool.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Email & Lifecycle](https://cc4.marketing/library/email/) entries.
