# Blog Post Outline Builder

**Type:** Slash Command &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/content/blog-post-outline/](https://cc4.marketing/library/content/blog-post-outline/)

_Turn a keyword into an H2 and H3 outline with intent notes._

The outline is where a blog post is won or lost. Get the structure right and the draft writes itself; get it wrong and no amount of editing saves it. This command turns a keyword into a full H2 and H3 outline and, next to each section, notes the job that section does for the reader. You approve the structure before anyone writes a sentence.

## The command

Save this as `.claude/commands/outline.md` in your project.

```markdown
---
description: Build an H2 and H3 blog outline with intent notes from a keyword.
argument-hint: [target keyword or working title]
---

You are a content strategist outlining a blog post. The topic is: $ARGUMENTS

Produce an outline using H2 and H3 headings. Rules:

- Open with a one-line note on who the reader is and what they want.
- Use H2s for main sections and H3s for sub-points under them.
- Next to each H2, in parentheses, note the job it does: hook, context,
  main answer, objection, proof, next step, and so on.
- Order the sections so the primary intent is answered early, then supported.
- Include one H2 near the end for a clear call to action.
- After the outline, list 3 questions the post must answer to be complete,
  and suggest one visual or example per main section.

Keep the outline tight enough to hand to a writer without more explanation.
If the topic is broad, note where you narrowed the scope and why.
```

## How to use

1. Save the block above as `.claude/commands/outline.md`.
2. Run `/outline how to run a product launch on a small budget`.
3. Read the parenthetical job notes: reorder sections if the intent is not answered early enough.
4. Approve the structure, then draft each section or hand the outline to a writer.
5. When the post is live, run the Repurpose command to spin it into social copy.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Content & Copy](https://cc4.marketing/library/content/) entries.
