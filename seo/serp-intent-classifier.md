# SERP Intent Classifier

**Type:** Prompt &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/seo/serp-intent-classifier/](https://cc4.marketing/library/seo/serp-intent-classifier/)

_Label a keyword list by search intent, with a reason for each call._

Ranking starts with matching intent. A transactional keyword needs a product or comparison page, not a 2,000 word guide. This prompt takes a raw keyword list and sorts it by intent, with a one-line reason for each call, so you can decide what kind of page each keyword deserves before you write a word.

## The prompt

```text
You are an SEO analyst. I will give you a list of keywords. For each keyword,
classify the dominant search intent as one of:

- informational (the searcher wants to learn or understand)
- commercial (the searcher is comparing options before buying)
- transactional (the searcher is ready to act, buy, sign up, download)
- navigational (the searcher wants a specific brand, product, or page)

Return a table with three columns: Keyword, Intent, Reason. The reason is one
short sentence explaining the signal you used (modifiers like "best" or "vs"
suggest commercial, "buy" or "pricing" suggest transactional, "how to" or
"what is" suggest informational, a brand name suggests navigational).

If a keyword could carry two intents, pick the dominant one and note the
secondary intent in the reason. Do not skip any keyword.

After the table, add a short section called "Grouping" that buckets the
keywords by intent and, for each bucket, names the page type that fits best
(guide, comparison, landing page, product page, and so on).

Here is the list:
[paste your keywords, one per line]
```

## How to use

1. Paste the prompt into Claude Code and replace the last line with your keyword list.
2. Read the Reason column to sanity check the calls: intent labels drive your whole content plan.
3. Use the Grouping section to assign each bucket to a page type.
4. Send informational keywords to the Content Brief Generator to build the article briefs.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [SEO](https://cc4.marketing/library/seo/) entries.
