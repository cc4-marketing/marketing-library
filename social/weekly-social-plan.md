# Weekly Social Plan

**Type:** Slash Command &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/social/weekly-social-plan/](https://cc4.marketing/library/social/weekly-social-plan/)

_Turn your content pillars into a 7 day social plan with hooks and CTAs._

A week of social usually dies as a vague intention to "post more." This command turns your content pillars into a concrete 7 day plan: one post per day, each with a channel, a hook line, a format, and a call to action. You approve or swap at the plan level in two minutes, then hand each day to a drafting step. No blank calendar, no Monday scramble.

## The command

Save this as `.claude/commands/social-plan.md` in your project.

```markdown
---
description: Build a 7 day social content plan from content pillars.
argument-hint: [pillars, channels, audience, and the week's goal]
---

You are a social media strategist. The brief is: $ARGUMENTS

If the content pillars, channels, audience, or the goal for this week are
missing, ask for them first. Then build a 7 day plan as a table, one row per
day (Monday to Sunday).

Columns: Day, Channel, Pillar, Format, Hook, CTA.

Rules:
- Assign each day exactly one pillar. Spread the pillars across the week so no
  pillar runs two days in a row.
- Match the format to the channel and pillar (for example: carousel, short
  video, text post, poll, single image, thread). Vary formats across the week.
- Write the Hook as a real opening line a reader would stop on, not a topic
  label. Make it specific to the audience.
- Give each day one clear CTA (comment, save, click, sign up, DM). Do not put
  the same CTA on every day.
- Keep one lighter or community day in the week so it does not read as seven
  sales posts.

After the table:
- List 2 backup posts that fit any pillar, for a day that falls through.
- Note the single best-performing day to boost if there is budget, and why.

Keep it realistic for one person to ship in a week.
```

## How to use

1. Save the block above as `.claude/commands/social-plan.md`.
2. Run `/social-plan` and give it your pillars, channels, audience, and this week's goal.
3. Skim the Hook column first: if a hook is dull, ask for three alternates on that row.
4. Copy the table into your scheduler and set the dates.
5. Expand any single day into a finished post with the LinkedIn Post From Notes command.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Social & Community](https://cc4.marketing/library/social/) entries.
