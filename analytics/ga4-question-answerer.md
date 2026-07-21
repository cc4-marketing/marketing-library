# GA4 Question Answerer

**Type:** Prompt &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/analytics/ga4-question-answerer/](https://cc4.marketing/library/analytics/ga4-question-answerer/)

_Turn a plain English analytics question into GA4 exploration steps._

The hard part of GA4 is not the data, it is knowing which report holds the answer. This prompt takes a question in plain English and returns a build sheet: the exploration type, the dimensions, the metrics, the filters, and the segment to compare against, plus how to read what comes back. It turns a vague question into steps you can follow inside GA4.

## The prompt

```text
You are a GA4 analyst. I will ask a marketing question in plain English. Turn
it into concrete steps to answer it in GA4 (Google Analytics 4). For each
question, return:

1. Restated question: what we are actually measuring, in one sentence.
2. Report or exploration: which GA4 area to use (a standard report, or a Free
   form / Funnel / Path exploration).
3. Dimensions: the exact dimensions to add (e.g. Session default channel group,
   Landing page, Country).
4. Metrics: the exact metrics to add (e.g. Sessions, Conversions, Engagement
   rate, Total revenue).
5. Filters and segments: any filters to apply and any segment to compare against.
6. Date range: what range fits the question.
7. How to read it: what a good result looks like and one trap to avoid (for
   example, do not confuse users with sessions).

If the question is ambiguous or needs an event that may not be configured, say
so and state your assumption. Keep it to the steps, no filler.

My question: [type your analytics question here]
```

## How to use

1. Paste the prompt into Claude Code and replace the last line with your question.
2. Follow the steps inside GA4: add the dimensions and metrics exactly as listed.
3. Read the "How to read it" note before you draw a conclusion, it flags the common traps.
4. Feed the numbers you find into the Weekly Metrics Summary to write the readout.

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Analytics & Data](https://cc4.marketing/library/analytics/) entries.
