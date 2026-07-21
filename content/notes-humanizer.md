# Notes Humanizer

**Type:** Skill &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/content/notes-humanizer/](https://cc4.marketing/library/content/notes-humanizer/)

_Strip the AI tells out of a draft so it reads like a person wrote it._

Most AI drafts read smooth and say nothing. They lean on the same tells: em dashes splitting every other sentence, words like "delve" and "leverage", the "it's not just X, it's Y" construction, and transitions that add no information. Readers clock that tone now, and so do AI detectors. Notes Humanizer is a Claude Code skill that runs as a final pass on a draft, cuts those patterns, and puts a human voice back in. You keep the AI speed and ship copy that does not sound like a model wrote it.

## What it does

The skill works in two passes.

**Strip pass.** It removes the default set of AI tells:

- Em dashes used for clause separation.
- "Delve", "leverage", "utilize", "in today's fast-paced", "navigate the landscape".
- The "it's not just X, it's Y" pattern.
- Overuse of trios (the "X, Y, and Z" structure on repeat).
- Hedging adverbs: "essentially", "fundamentally", "ultimately".
- Empty transitions: "moreover", "furthermore", "in conclusion".

**Inject pass.** It adds what a flat draft is missing:

- One concrete number or proper noun about every 80 words.
- One opinion or preference a model would not volunteer on its own.
- Sentence-length variance, mixing short punchlines with longer setups.
- A voice quirk that matches your prior writing.

The result reads like one person wrote it on a good day, not like a template got filled in.

## Install

This one is free. Clone it straight into your Claude Code skills directory, then restart Claude Code.

```bash
git clone https://github.com/cc4-marketing/notes-humanizer ~/.claude/skills/notes-humanizer
```

The source lives at [github.com/cc4-marketing/notes-humanizer](https://github.com/cc4-marketing/notes-humanizer). Once it is installed, draft your copy as usual and ask Claude to run the notes-humanizer skill on it before you publish.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Content & Copy](https://cc4.marketing/library/content/) entries.
