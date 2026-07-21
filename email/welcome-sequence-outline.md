# Welcome Sequence Outline

**Type:** Slash Command &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/email/welcome-sequence-outline/](https://cc4.marketing/library/email/welcome-sequence-outline/)

_Outline a 4 to 5 email onboarding drip with goal, subject, and CTA per email._

Most welcome flows are one email that says "thanks for subscribing" and then silence. This command outlines the whole arc instead: 4 to 5 emails, each with a clear goal, subject line options, the beats the body should hit, a send delay, and one call to action. You review the journey as a shape (does it build trust before it asks?) before anyone writes a word of final copy.

## The command

Save this as `.claude/commands/welcome-sequence.md` in your project.

```markdown
---
description: Outline a 4 to 5 email welcome and onboarding sequence.
argument-hint: [product, audience, the signup source, and the sequence goal]
---

You are a lifecycle email strategist. The brief is: $ARGUMENTS

If the product, audience, where people signed up, or the goal of the sequence
(for example first purchase, activation, first login) is missing, ask for it
first. Then outline a 4 to 5 email welcome sequence.

For each email, give:
- Email number and its single goal in one line.
- Send delay from the previous step (for example: immediately, day 2, day 4).
- Two subject line options, written to be opened, not clever for its own sake.
- Body beats: 3 to 5 bullet points for what the email covers, in order.
- One CTA: the exact action and where it points.

Arc to follow across the sequence:
1. Welcome and set expectations: confirm what they get and how often.
2. Deliver a quick win or the single most useful thing right away.
3. Handle the top objection or friction that stops people acting.
4. Show proof (a result, a case, a number, a testimonial).
5. Make the ask: the primary conversion, with a reason to act now.

If four emails fit better than five, merge steps 3 and 4 and say so.

Rules:
- One goal and one CTA per email. Do not stack asks.
- Keep it specific to the product and audience, not generic onboarding filler.
- End with a short note on what should happen when the sequence finishes
  (move to the main list, tag as engaged, or enter a nurture track).
```

## How to use

1. Save the block above as `.claude/commands/welcome-sequence.md`.
2. Run `/welcome-sequence` and describe the product, audience, signup source, and goal.
3. Read the goals column top to bottom: the sequence should build trust before the ask in the last email.
4. Adjust send delays to match your tool, then build the automation.
5. Draft each email's full copy in a follow up pass, one email at a time.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Email & Lifecycle](https://cc4.marketing/library/email/) entries.
