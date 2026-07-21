# Content Gap Finder

**Type:** Prompt &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/competitive/content-gap-finder/](https://cc4.marketing/library/competitive/content-gap-finder/)

_Compare a competitor's topic coverage to yours and rank the gaps to target._

Competitive content work stalls at "they just have more stuff." This prompt gets specific: paste their topic list and yours, and it maps coverage against coverage, then returns a ranked list of gaps (topics they cover that you do not) scored by relevance to your buyer, the intent served, and effort to win. It also flags the topics worth ignoring, so the roadmap chases winnable ground instead of matching a rival page for page.

## The prompt

```text
You are a content strategist doing a coverage gap analysis. I will give you two
lists of topics or page titles: a competitor's and mine.

My business and buyer: [one line, for example: project management app for
in-house creative teams].

Do this:

1. Cluster both lists into topic themes (for example: onboarding, pricing,
   integrations, use cases, comparisons, thought leadership). Do not just match
   titles word for word; group by the underlying topic.

2. Build a coverage table by theme: Theme, They cover (yes / partial / no),
   I cover (yes / partial / no), Gap type. Gap types: They have it and I do
   not (true gap), We both have it (parity), I have it and they do not (my
   edge).

3. For every true gap, score it:
   - Relevance to my buyer (high / med / low).
   - Search intent it serves (informational, commercial, transactional).
   - Effort to win (low / med / high), based on how deep the topic looks.
   Then give a priority (chase now / chase later / skip) that favors high
   relevance and lower effort.

4. Output a ranked "Chase now" list: the specific pieces to create, each with
   a working title, the intent it targets, and why it beats matching them.

5. Flag any competitor topics I should deliberately skip because they do not
   fit my buyer, so I do not copy their site out of reflex.

6. End with my strongest existing edge (a theme I own that they do not) and how
   to lean into it.

Be specific and honest. If my list is thin in a theme that matters, say so.

Their topics:
[paste competitor page titles or slugs]

My topics:
[paste my page titles or slugs]
```

## How to use

1. Pull both topic lists: their blog index or sitemap and yours (titles or URL slugs are enough).
2. Paste the prompt, fill in the business and buyer line, and paste both lists.
3. Read the Chase now list first, then sanity-check the Skip flags against your audience.
4. Send the top gaps into the Content Brief Generator to turn each into a full brief.
5. Re-run each quarter to catch new topics a competitor has started ranking for.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Competitive Research](https://cc4.marketing/library/competitive/) entries.
