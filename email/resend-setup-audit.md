# Resend Setup Audit

**Type:** Prompt &middot; **Access:** Free &middot; **Live page:** [https://cc4.marketing/library/email/resend-setup-audit/](https://cc4.marketing/library/email/resend-setup-audit/)

_Audit your Resend setup end to end: domain, DMARC, tracking, and broadcast hygiene._

Resend is easy to start and easy to leave half configured: shared click tracking, no DMARC, an audience the signup form never writes to. This prompt runs a fixed seven-point audit of your Resend setup and asks Claude Code to show proof for each item (dashboard state, DNS answers, or API responses) before it changes anything. Run it once after setup, then again before your first real broadcast.

## The prompt

```text
Audit my Resend setup end to end. Work through this checklist and
show me proof for each item (dashboard state, DNS answers, or API
responses). Stop and ask before anything irreversible: sends, DNS
changes, releases.

1. SENDING DOMAIN. Confirm the sending subdomain is verified:
   DKIM and SPF records all green in Resend.
2. AUDIENCE. Confirm the signup flow both sends the welcome email
   AND inserts the contact into an Audience. Report current counts:
   total, subscribed, unsubscribed.
3. CLICK TRACKING. Check whether the domain uses shared click
   tracking. If yes, configure a custom tracking subdomain
   (links.<sending-domain>), add the CNAME (DNS-only, not proxied),
   and verify it.
4. OPEN TRACKING. Confirm it is off unless I explicitly want it.
5. DMARC. Check the _dmarc TXT record on the sending subdomain.
   If missing, add: v=DMARC1; p=none; rua=mailto:dmarc@<root-domain>
   and verify with dig. Remind me to tighten to p=quarantine after
   a month of clean reports.
6. REPORT ROUTING. Confirm dmarc@<root-domain> routes to a real
   inbox (a catch-all rule counts).
7. BROADCAST HYGIENE. Before any send: report the recipient count,
   send me a test email, confirm every image URL in the email
   returns 200, and confirm the unsubscribe link is present.
List anything you could not verify at the end.
```

## How to use

1. Open your project in Claude Code with the Resend API key available (as an environment variable or in your secrets manager, never pasted in plain text).
2. Paste the prompt. Swap `<sending-domain>` and `<root-domain>` for your real domains.
3. Read each item's proof before you approve a fix. If the agent proposes a DNS change or a send, it will pause for your go-ahead.
4. Run it again right before your first broadcast, so the recipient count, test email, and image checks are fresh.
5. For the reasoning behind each step, read the full walkthrough: [Set Up Resend Right: A Marketer's Checklist with an AI Agent](https://cc4.marketing/blog/resend-setup-checklist-for-marketers/).

---

Part of the [Claude Code Marketing Library](https://cc4.marketing/library/). See the live page for the latest version. Browse more [Email & Lifecycle](https://cc4.marketing/library/email/) entries.
