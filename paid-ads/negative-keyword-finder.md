# Negative Keyword Finder

**Type:** Prompt &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/paid-ads/negative-keyword-finder/](https://cc4.marketing/library/paid-ads/negative-keyword-finder/)

_Mine a Google Ads search terms export for negative keywords, grouped by reason._

Search terms reports are where paid budgets quietly leak: clicks on queries that were never going to buy. This prompt reads your export and proposes a negative keyword list, but grouped by reason (wrong intent, wrong product, job seekers, free-seekers, competitor names, and so on) so you can approve whole buckets at once. It also protects anything with conversions and flags borderline terms as do-not-block, so cleanup does not cut into what works.

## The prompt

```text
You are a paid search analyst cleaning up wasted spend. I will paste a Google
Ads search terms report (CSV rows with search term, clicks, cost, conversions,
and if present impressions and CTR).

The product and its ideal buyer: [one line, for example: paid B2B invoicing
software for small agencies].

Do this:

1. Scan every search term and judge relevance against the product and buyer
   above, weighed against its cost and conversions.

2. Propose negative keywords, grouped by the reason they waste spend. Use
   groups like: Wrong intent (research or how-to only), Wrong product or
   feature, Free or DIY seekers, Job and career seekers, Competitor brand
   terms, Location or audience mismatch, Adult or unrelated. Add groups if the
   data needs them.

3. For each group, give a table: Search term, Clicks, Cost, Conversions,
   Suggested negative, Match type (phrase, exact, or broad), Why.
   - Suggest exact or phrase negatives for specific junk terms.
   - Suggest a broad negative only for a whole irrelevant theme, and name the
     root word.

4. Protect performers: never propose negating any term that has conversions.

5. Output a separate "Do not block yet" list: borderline terms that look
   off-topic but have spend and no clear verdict, so I can watch them.

6. End with the total clicks and cost the proposed negatives would have saved
   in this report, and the single biggest waste theme.

Be conservative: when a term could plausibly convert, leave it and explain.
Here is the report:
[paste the CSV rows]
```

## How to use

1. In Google Ads, open the search terms report, set a meaningful date range, and export to CSV.
2. Paste the prompt, fill in the product and buyer line, and paste the rows (or attach the file).
3. Review group by group. Approve whole buckets, and spot-check the do-not-block list.
4. Add the approved negatives at the right level (ad group, campaign, or a shared negative list) with the match types given.
5. Re-run monthly on the fresh export so new waste themes get caught early.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Ads & Paid](https://cc4.marketing/library/paid-ads/) entries.
