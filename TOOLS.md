Last updated: **2026-02-25**

# Tools catalog (Qwayk)

Quick note:
- This page is public so you can see what you’re paying for before you sponsor.
- Some tools are already published as repos under the `Qwayk` org. Some are still being migrated.
- Either way, this page tells you what exists in the library.

## How these tools work

You run everything locally.

The tools don’t “take over your account”.
They just call the same APIs you’d call manually, but with guardrails.

You’ll usually see this flow:
1) Dry-run shows the plan
2) Apply is a separate step
3) The tool verifies what happened
4) You get a receipt you can keep

## Current lineup

I built these around “real outcomes”, not just endpoints.
So I group them by what you’re trying to do.

Content and publishing:
- WordPress: read and update posts, pages, and media through the WordPress REST API.
- Ghost: safe admin workflows for Ghost sites.

Assets:
- Freepik: search and download assets. Downloads require explicit apply.
- Unsplash: search photos. Download tracking requires apply.

Analytics:
- Plausible: read stats. Writing events requires explicit apply and confirmation.

Ads + marketing data:
- Google Ads: safe-by-default reads and carefully gated changes where supported.
- Meta Ads: read-only access.

Infra + accounts:
- Cloudflare: DNS, Zero Trust, Workers, WAF rules, TLS, and more. Writes require explicit apply.
- Statuspage: read status and manage incidents and maintenance with safety gates.
- Dynadot: registrar workflows for domains, DNS, nameservers, and transfers with safety gates.

Sales ops:
- Instantly: campaigns, leads, webhooks, enrichment. Destructive changes require a reviewed plan file.

Money ops:
- Mercury: safe-by-default reads and carefully gated workflows.

Affiliate/product data:
- Amazon PA-API v5: product lookups, read-only.

Social:
- Pinterest: read-only browsing, no posting.

Video:
- YouTube: safe CLI patterns for YouTube-related workflows where supported.

## What members get

Members repo: `Qwayk/qwayk-tools` (private)

You get:
- onboarding that’s actually usable (not “read docs for 2 hours”)
- workflow packs (“do this outcome” playbooks)
- release notes and early drops

Also:
- when a tool is published as its own repo under the Qwayk org, members get the update first (and the workflow pack stays consistent).

You don’t get:
- custom setup
- sharing your API keys with me
- an SLA

## What’s next

This list will keep growing.

If there’s a specific API you want next, open an issue in the public repo and tell me:
- what outcome you want
- what the “safe dry-run plan” should look like
