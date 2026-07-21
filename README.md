# Claude Code Marketing Library

A curated, free set of prompts, slash commands, subagents, and MCP server lists for marketers using [Claude Code](https://www.claude.com/product/claude-code). Every entry is a real, copyable artifact you paste into Claude Code and run against your own work. Each one also lives on [cc4.marketing](https://cc4.marketing/library/) with a rendered page, FAQ, and related entries.

This repo is the shareable master copy. Copy an artifact, adapt the placeholders to your product and audience, and keep it in your project.

## Browse on the web

Read the rendered versions at **[cc4.marketing/library](https://cc4.marketing/library/)**. The site is the source of truth; this repo mirrors it.

## Directory

20 entries across 9 categories.

| Category | Name | Type | Access | What it does |
| --- | --- | --- | --- | --- |
| SEO | [Content Brief Generator](seo/content-brief-generator.md) | Slash Command | Free | Turn one keyword into a full SEO content brief a writer can follow. |
| SEO | [Meta Title and Description Writer](seo/meta-title-description-writer.md) | Slash Command | Free | Write SERP length checked title and description pairs that fit Google. |
| SEO | [SERP Intent Classifier](seo/serp-intent-classifier.md) | Prompt | Free | Label a keyword list by search intent, with a reason for each call. |
| Content & Copy | [Blog Post Outline Builder](content/blog-post-outline.md) | Slash Command | Free | Turn a keyword into an H2 and H3 outline with intent notes. |
| Content & Copy | [Blog to Social Repurposer](content/repurpose-blog-to-social.md) | Slash Command | Free | Turn one blog post into a LinkedIn post, an X thread, and a carousel. |
| Content & Copy | [Brand Voice Memory Block](content/brand-voice-memory.md) | Prompt | Free | A CLAUDE.md block that keeps every draft on brand across a project. |
| Ads & Paid | [Ad Copy Variant Generator](paid-ads/ad-copy-variants.md) | Slash Command | Free | Generate 10 headline and primary text variants, each with an angle. |
| Ads & Paid | [Negative Keyword Finder](paid-ads/negative-keyword-finder.md) | Prompt | Free | Mine a Google Ads search terms export for negative keywords, grouped by reason. |
| Analytics & Data | [GA4 Question Answerer](analytics/ga4-question-answerer.md) | Prompt | Free | Turn a plain English analytics question into GA4 exploration steps. |
| Analytics & Data | [UTM Builder](analytics/utm-builder.md) | Slash Command | Free | Build consistent UTM tagged URLs from your naming rules and flag drift. |
| Email & Lifecycle | [Newsletter Section from a Link](email/newsletter-from-link.md) | Slash Command | Free | Summarize a URL into a newsletter section with subject line and CTA. |
| Email & Lifecycle | [Welcome Sequence Outline](email/welcome-sequence-outline.md) | Slash Command | Free | Outline a 4 to 5 email onboarding drip with goal, subject, and CTA per email. |
| Social & Community | [LinkedIn Post from Notes](social/linkedin-post-from-notes.md) | Slash Command | Free | Draft a LinkedIn post from rough bullet notes, with a hook and CTA. |
| Social & Community | [Weekly Social Plan](social/weekly-social-plan.md) | Slash Command | Free | Turn your content pillars into a 7 day social plan with hooks and CTAs. |
| Reporting & Dashboards | [Monthly Report Outline](reporting/monthly-report-outline.md) | Slash Command | Free | Produce an executive monthly marketing report outline leaders will read. |
| Reporting & Dashboards | [Weekly Metrics Summary](reporting/weekly-metrics-summary.md) | Prompt | Free | Turn a metrics CSV into a plain language weekly readout with deltas. |
| Competitive Research | [Competitor Page Teardown](competitive/competitor-page-teardown.md) | Prompt | Free | Analyze one competitor landing page for offer, proof, CTA, and gaps. |
| Competitive Research | [Content Gap Finder](competitive/content-gap-finder.md) | Prompt | Free | Compare a competitor's topic coverage to yours and rank the gaps to target. |
| Project & Ops | [Content Calendar Scaffold](project-ops/content-calendar-scaffold.md) | Slash Command | Free | Build a 90 day rolling content calendar from a short description. |
| Project & Ops | [Marketing MCP Starter](project-ops/marketing-mcp-starter.md) | MCP Server | Free | A starter set of MCP servers marketers actually use with Claude Code. |

## How to use an entry

1. Open the entry file (or its live page) and read the short intro.
2. Copy the fenced artifact block: the prompt, the slash command, the CLAUDE.md block, or the MCP list.
3. Paste it into Claude Code. For a slash command, save it at the path the entry names (for example `.claude/commands/outline.md`); for a prompt, paste it straight into the session; for a CLAUDE.md block, add it to your project's `CLAUDE.md`.
4. Fill in the placeholders with your real details, then run it.

Every entry ends with a "How to use" list specific to that artifact.

## Contributing

Want to add an entry or fix one? See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT. See [LICENSE](LICENSE).
