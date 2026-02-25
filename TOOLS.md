Last updated: **2026-02-25**

# Tools catalog (Qwayk)

Quick note:
- This page is public so you can see what you’re paying for before you sponsor.
- I’m publishing tools into the `Qwayk` org repo-by-repo. Some are already there, some are “next up”.

## How these tools work (in normal words)

You run everything locally.

The tools don’t “take over your account”.
They just call the same APIs you’d call manually, but with guardrails:

1) Dry-run shows the plan.
2) Apply is a separate step.
3) We verify via read-back.
4) You get a receipt (so you can prove what changed).

## Current lineup (what I’ve built so far)

Content + publishing:
- WordPress — read/update posts, pages, media, and more through the WP REST API (safe-by-default).
- Ghost — safe admin workflows for Ghost sites (dry-run → apply → verify).

Assets:
- Freepik — search and download assets (downloads require explicit apply).
- Unsplash — search photos; optional download tracking (apply required).

Analytics:
- Plausible — read stats; write events only with explicit `--apply --yes`.

Ads + marketing data:
- Google Ads — safe-by-default reads (and carefully gated writes where supported).
- Meta Ads — read-only Marketing API access (GET-only).

Infra + accounts:
- Cloudflare — DNS, Zero Trust, Workers, WAF/rulesets, TLS, and more (writes require explicit apply).
- Statuspage — read status + manage incidents/maintenance safely (gated writes).
- Dynadot — registrar API workflows (domains, DNS, nameservers, transfers) with safety gates.

Sales ops:
- Instantly — campaigns/leads/webhooks + enrichment (destructive changes require a reviewed plan file).

Money ops:
- Mercury — safe-by-default reads and carefully gated workflows.

Affiliate/product data:
- Amazon PA-API v5 — product lookups (read-only).

## What members get (so it’s worth paying)

Members repo: `Qwayk/qwayk-tools` (private)

You get:
- onboarding that’s actually usable (not “read docs for 2 hours”)
- workflow packs (“do this outcome” playbooks)
- release notes and early drops

You don’t get:
- custom setup
- sharing your API keys with me
- an SLA

## What’s next

This list will keep growing.

If there’s a specific API you want next, open an issue in the public repo and tell me:
- what outcome you want
- what the “safe dry-run plan” should look like

