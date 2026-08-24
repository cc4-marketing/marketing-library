# B2B Enterprise Naming

**Type:** Skill &middot; **Access:** Free &middot; **Live page:** (added when it ships on the site)

_Turn a naming brief into a scored shortlist that reads like enterprise software, not a myth._

Most naming approaches default to story and metaphor. That's the wrong register for a PMO platform, an internal tool, or a B2B campaign, where the name needs to read as business vocabulary on first pass, not a legend that needs explaining. This skill sources candidates from two lanes (plain category words the audience already uses daily, and a short glossary of borrowed industry terms like Control Tower or Command Center that carry built-in meaning), structures each candidate as a Core Name plus a Subtitle pulled straight from the brief's existing pillars, and scores finalists on a five-axis B2B fit matrix: short, B2B-aware, domain related, easy and not too broad, not too distant or strange. It also flags the tradeoff when a candidate bakes in a department word (PMO, Sales Ops) and offers a broader swap for audiences that span more than one function.

## The skill

`SKILL.md`

```markdown
---
name: b2b-enterprise-naming
description: Build names for B2B and enterprise products, internal platforms, corporate events, or campaigns using grounded business vocabulary instead of mythic or story-driven names. Use when the object is an enterprise product, PMO/IT platform, corporate event, or B2B campaign; when the user explicitly rejects mythic/story naming ("not some theme for star", "not anduril like", "too generic", "keep it business"); or when the audience is a business function (PMO, IT, sales, ops) rather than consumer. Produces a "Core Name: Subtitle" shortlist scored on a 5-axis B2B fit matrix, dials concreteness to audience seniority, and flags domain-word scope tradeoffs (e.g. keeping vs swapping a department name like PMO). Route to anduril-naming instead when the user wants mythic, story-driven, or symbolically deep names.
---

# B2B Enterprise Naming

Turn a business naming brief (event, product, platform, campaign) into a shortlist grounded in real enterprise vocabulary, not myth or metaphor. Sibling to `anduril-naming`: that skill owns story-driven names with narrative depth, this skill owns names that read as business software or corporate event language on first pass.

## When to use vs anduril-naming

Use this skill when the object is B2B/enterprise-facing and the user wants it to sound like it belongs in that world (or explicitly says no to myth/story framing). Use `anduril-naming` when the user wants symbolic depth, a retellable story, or explicitly references Anduril-style naming. If unsure, ask which register fits, don't guess.

## Workflow

### Step 1: Brief intake
Capture: what's being named, audience and its seniority (exec vs mid-level vs operational), and any pillars/value props the business has already defined (three pillars, a tagline, a positioning line). Reuse those pillars verbatim in the subtitle later, never invent new ones. Note if a department/function word (PMO, Sales Ops, IT) is in play and whether the audience is exactly that function or broader.

### Step 2: Source vocabulary, two lanes
Lane A, plain category words the audience uses daily: project, delivery, portfolio, operations, the department name itself.
Lane B, borrowed industry terms that carry built-in meaning without needing a myth: Control Tower, Command Center, Single Pane of Glass, Nerve Center. See `references/industry-terms.md` for the glossary and when each term fits.
Don't reach for Lane B by default, only when Lane A reads too flat for the brief.

### Step 3: Structure candidates as Core Name: Subtitle
Core Name: 1 to 3 plain nouns, no metaphor required. Subtitle: state the brief's existing pillars or value prop directly (e.g. "Align, Predict, Optimize" or "Full Visibility, Total Control"). This is the deliverable unit, always generate both halves together.

### Step 4: Two dials for iteration
Concreteness axis: mythic/story (anduril-naming territory), then borrowed industry term (Lane B), then plain descriptive (Lane A). Seniority axis: executive-abstract to operational-concrete.
When the user reacts "too generic", move one step toward Lane B. "Too strange / too distant / needs explaining", move one step toward Lane A. "Audience is more senior/junior", slide the seniority axis and regenerate, don't restart from scratch, reuse what already scored well.

### Step 5: Domain-word scope check
For every shortlist, if a candidate bakes in a department/function word, produce both variants: keep-word (precise, strong if audience is exactly that function) and swap-word (broader term, safer if audience spans departments). State the tradeoff in one line, don't silently pick one.

### Step 6: Score with the B2B fit matrix
Score each finalist (full Core Name: Subtitle) 1 to 5 on five axes and present as a markdown table:
- Short: is the core name itself compact, not the tagline
- B2B-aware: reads as enterprise/business software or consulting language, not consumer marketing
- Domain-related: clearly signals the specific function from the brief, or is broadened by design
- Easy and not too broad: parses instantly and can't be mistaken for an unrelated product category
- Not too distant/strange: no unfamiliar words or borrowed terms the audience won't already recognize, no explainer sentence needed

Follow the table with a one-line verdict naming the top pick and one backup, referencing the specific tradeoff (usually domain-word breadth or seniority fit) that decided it.

### Step 7: Deliver
Always end with the finalists written out in full as complete "Core Name: Subtitle" strings, exactly as they'd appear on a banner or title slide, plus one line on which is recommended and why.

## Resources

- `references/industry-terms.md`: Lane B glossary (Control Tower, Command Center, Single Pane of Glass, etc), what each signals, and when it outperforms plain description.
```

`references/industry-terms.md`

```markdown
# Lane B: borrowed industry terms

Terms with built-in meaning from an adjacent enterprise field, on loan for a new brief. Reach for these only when Lane A (plain category words) reads too flat. Each entry: what it signals, native field, when it fits, when it's a stretch.

## Control Tower
Signals: real-time visibility across many moving parts plus the authority to direct them. Native field: supply chain, IT operations, increasingly PPM/portfolio vendors (Planview, ServiceNow already market "Project/Portfolio Control Tower").
Fits: briefs about visibility plus coordinated decision-making across a portfolio. Audience: mid-to-senior, comfortable with ops vocabulary.
Stretch: single-project or single-team scope, no portfolio-level view to justify the term.

## Command Center
Signals: centralized, decisive control, leans more "act now" than "observe calmly." Native field: military/ops rooms, borrowed heavily by security and NOC tooling.
Fits: briefs that emphasize response speed or crisis/incident handling.
Stretch: routine planning or steady-state reporting, where "command" overstates the stakes.

## Single Pane of Glass
Signals: one unified view replacing several fragmented tools/dashboards. Native field: IT infrastructure monitoring.
Fits: briefs where the pain point is literally tool sprawl or scattered reporting.
Stretch: as a standalone event/product name it reads flat, works better as subtitle language ("...in a single pane of glass") than as the Core Name itself.

## Nerve Center
Signals: coordination hub, less military than Command Center, more organic/biological metaphor for central coordination.
Fits: briefs wanting "central hub" without the command/military edge.
Stretch: audience unfamiliar with the idiom outside English business writing, riskier for non-native-English audiences.

## Mission Control
Signals: high-stakes, high-precision oversight of a complex operation in progress. Native field: aerospace.
Fits: launch-style events, go-live moments, briefs with a literal "launch" framing.
Stretch: everyday/recurring operations, "mission" overstates one-off drama for something ongoing.

## Choosing among them
Match the verb the brief already implies. Visibility plus steer: Control Tower. Speed plus respond: Command Center. Consolidate scattered tools: Single Pane of Glass (subtitle, not core name). Coordinate a hub: Nerve Center. One big moment: Mission Control.

If none of these verbs match the brief, stay in Lane A. A forced Lane B term scores worse on "not too distant/strange" than an honest plain descriptive name.
```

## How to use

1. Save the first block as `~/.claude/skills/b2b-enterprise-naming/SKILL.md`.
2. Save the second block as `~/.claude/skills/b2b-enterprise-naming/references/industry-terms.md`.
3. Restart Claude Code, then describe the naming brief: what's being named, how senior the audience is, and any pillars or tagline already agreed on.
4. React to the shortlist in plain language ("too generic," "too strange," "audience is more senior than that"), the skill moves along the concreteness or seniority dial instead of starting over.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Content & Copy](https://cc4.marketing/library/content/) entries.
