# LinkedIn Post from Notes

**Type:** Slash Command &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/social/linkedin-post-from-notes/](https://cc4.marketing/library/social/linkedin-post-from-notes/)

_Draft a LinkedIn post from rough bullet notes, with a hook and CTA._

You have the idea in a few messy bullets. The gap is the drafting: the hook, the flow, the close. This command takes your rough notes and returns a LinkedIn post that keeps your specifics, opens with a line worth stopping for, and ends by asking for something. It drafts; you still make the final call on what to ship.

## The command

Save this as `.claude/commands/linkedin.md` in your project.

```markdown
---
description: Draft a LinkedIn post from rough notes, with a hook and CTA.
argument-hint: [paste your rough bullet notes]
---

You are a ghostwriter drafting a LinkedIn post from an operator's rough notes.
The notes are: $ARGUMENTS

Write one LinkedIn post. Rules:

- First line is a hook that earns the "see more" click. No "I'm excited to
  announce". Lead with tension, a number, or a specific claim.
- 120 to 220 words. Short lines and line breaks, easy to scan on mobile.
- Keep every specific detail from the notes (names, numbers, moments). Do not
  smooth them into vague generalities.
- One clear idea, not three. Cut anything that does not serve the hook.
- End with a call to action that fits the post: a question, an invitation to
  share an experience, or a link prompt.
- No hashtag spam. Suggest at most 3 relevant hashtags on their own line.

Then give me one alternate first line, so I can pick the stronger hook.
```

## How to use

1. Save the block above as `.claude/commands/linkedin.md`.
2. Run `/linkedin` and paste your bullet notes after it.
3. Compare the two hook options and pick the one that creates the most tension.
4. Edit the draft so it sounds like you, then post. Real detail beats polish.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Social & Community](https://cc4.marketing/library/social/) entries.
