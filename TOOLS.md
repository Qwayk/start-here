Last updated: **2026-02-25**

# Tools catalog (Qwayk)

This page is public so you can see what you’re paying for before you sponsor.

My goal is simple: let AI agents do real work for you, without the “oops it changed the wrong thing” problem.

## How these tools work

You run everything locally.

The tools don’t “take over your account”.
They just call the same APIs you’d call manually, but with guardrails.

You’ll usually see this flow:
1) Dry-run shows the plan
2) Apply is a separate step
3) The tool verifies what happened
4) You get a receipt you can keep

Two important notes:
- Some tools are read-only. Some can do writes.
- Anything that writes is gated. Dry-run first. Apply only when it looks right.

## Quick scan

| Tool | Best for | Writes |
|---|---|---|
| WordPress | publishing and editing content | yes, gated |
| Ghost | Ghost admin workflows | yes, gated |
| Freepik | finding and downloading assets | downloads gated |
| Unsplash | photo search | tracking gated |
| Plausible Analytics | website analytics | events gated |
| Google Ads | ads performance reads | depends |
| Meta Ads | ads performance reads | no, read-only |
| Cloudflare | DNS and zone changes | yes, gated |
| Atlassian Statuspage | incidents and components | yes, gated |
| Dynadot | domain inventory and registrar ops | yes, gated |
| Instantly | campaigns and lead ops | yes, gated |
| Mercury | money ops reads | depends |
| Amazon Product Advertising API v5 | product lookups | no, read-only |
| Pinterest | read-only data pulls | no, read-only |
| YouTube | read-only data pulls | depends |

## The lineup

### WordPress

Uses the WordPress REST API.

Best for: publishing and editing content safely.

Examples:
- list posts/pages and find the exact one you want to touch
- update a draft title/excerpt/SEO fields with a dry-run preview first
- bulk operations with a small scope, then verify via read-back

Writes: yes, but gated.

### Ghost

Uses the Ghost Admin API.

Best for: Ghost site admin workflows without guessing.

Examples:
- audit posts/pages and metadata
- patch small copy changes safely
- export, update, and verify what actually changed

Writes: yes, but gated.

### Freepik

Best for: finding assets fast, downloading only when you confirm.

Examples:
- search for an image style and shortlist results
- download only after a dry-run plan

Writes: downloads are gated.

### Unsplash

Best for: simple photo search workflows.

Examples:
- find a set of photos by keywords and orientation
- track downloads only when you explicitly apply

Writes: download tracking is gated.

### Plausible Analytics

Best for: understanding what pages/content are actually working.

Examples:
- pull top pages for the last 7/30 days
- check referrers and campaign tags
- write events only when you explicitly apply and confirm

Writes: events are gated.

### Google Ads

Uses the Google Ads API.

Best for: pulling performance data safely.

Examples:
- campaign performance by date range
- ad group and keyword performance reads

Writes: depends on the command. Assume reads first.

### Meta Ads

Read-only access to the Meta Marketing API.

Best for: read-only visibility into Meta ad performance.

Examples:
- pull campaign/ad set/ad performance metrics
- export data for reporting

Writes: no. Read-only.

### Cloudflare

Best for: careful DNS and zone changes with guardrails.

Examples:
- audit DNS records before changing anything
- apply a small DNS change, then read-back verify
- review security/zero-trust settings before touching them

Writes: yes, but gated.

### Atlassian Statuspage

Uses the Statuspage API.

Best for: status and incident workflows that are explicit and auditable.

Examples:
- read current incidents and component status
- create or update an incident only after a dry-run plan

Writes: yes, but gated.

### Dynadot

Uses Dynadot API3.

Best for: domain inventory and careful bulk registrar changes.

Examples:
- export domain inventory
- audit nameservers across many domains
- bulk set nameservers with a plan + verification

Writes: yes, but gated.

### Instantly

Best for: campaign and lead ops with a “review the plan first” workflow.

Examples:
- add leads to a campaign from a CSV
- run safe enrichment/search workflows
- anything destructive requires a reviewed plan file

Writes: yes, but gated.

### Mercury

Best for: money ops reads and careful workflows.

Examples:
- list accounts/transactions
- generate exports for bookkeeping

Writes: depends on the command. Assume reads first.

### Amazon Product Advertising API v5

Best for: product lookups and structured product data.

Examples:
- lookup products by ASIN
- pull prices and attributes for a shortlist

Writes: no. Read-only.

### Pinterest

Read-only v1.

Best for: reading Pinterest data without posting.

Examples:
- list boards and pins for analysis
- export data for planning

Writes: no. Read-only.

### YouTube

Best for: safe data pulls and workflow patterns where supported.

Examples:
- fetch channel/video info for analysis
- export data for reporting

Writes: depends on the workflow. Assume reads first.

## What members get

Members repo: `Qwayk/qwayk-tools` (private)

You get:
- onboarding that’s actually usable
- workflow packs that focus on outcomes
- release notes and early drops

Also:
- you get the update first when a tool ships as a polished workflow pack

You don’t get:
- custom setup
- sharing your API keys with me
- an SLA

## What’s next

This list will keep growing.

If there’s a specific API you want next, open an issue in the public repo and tell me:
- what outcome you want
- what the “safe dry-run plan” should look like
