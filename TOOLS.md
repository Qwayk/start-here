Last updated: **2026-03-17**

# Tools catalog (Qwayk)

You should be able to see what exists before you sponsor.

These tools let an AI agent do real work through APIs, without the “it changed the wrong thing” problem.

## Public demo tools (free)

These are public repos you can clone and test right now:
- Amazon PA‑API v5 (read-only): https://github.com/Qwayk/amazon-pa-api-tool
- Plausible Analytics: https://github.com/Qwayk/plausible-api-tool

## The safety loop (what makes this different)

Every tool is built around the same loop:

1) The tool shows you a plan first.
2) Nothing changes until you explicitly apply.
3) The tool verifies what happened.
4) You get a receipt you can keep.

You run everything locally. You bring your own API keys. You do not paste secrets into GitHub.

## Tools (quick scan)

Each entry below has plain-English examples so you can quickly tell if it is useful.

### Amazon Product Advertising API v5 (read-only)

Good for: product research workflows.

Examples:
- Turn a list of Amazon URLs into ASINs and clean affiliate links.
- Search for products and export a shortlist with prices and images.

Repo: https://github.com/Qwayk/amazon-pa-api-tool

### Plausible Analytics (Stats API and Events API)

Good for: understanding what content and traffic is working, with optional event writes when you approve.

Examples:
- Pull a weekly report of top pages, sources, and goals.
- Send a test event only after you approve the plan.

Repo: https://github.com/Qwayk/plausible-api-tool

### WordPress (REST API)

Good for: publishing and editing content with preview-first changes.

Examples:
- Find the exact post or page you want to edit and preview the patch.
- Apply a small set of metadata updates, then read-back verify.

### Ghost (Admin API + Content API)

Good for: content workflows for Ghost sites, including safe edits.

Examples:
- Audit posts and SEO fields and export a report.
- Preview and apply small copy fixes with verification.

### Freepik

Good for: searching and downloading assets, where downloads only happen after you approve.

Examples:
- Search and shortlist image styles for a page or post.
- Generate a download plan, then download only when you apply.

### Unsplash

Good for: photo search workflows, with gated download tracking.

Examples:
- Search by keyword, orientation, and color and export a shortlist.
- Track downloads only when you apply.

### Google Ads API (read and write)

Good for: pulling performance data and making changes safely when you choose to.

Examples:
- Export an analysis pack for a date range, then generate an offline optimization report.
- Preview a campaign change plan, then apply only after review.

### Meta Ads API (read-only)

Good for: visibility into Meta ad performance without posting or changing anything.

Examples:
- Export campaign and ad set performance metrics for reporting.
- Pull breakdowns by date range for analysis.

### Microsoft Ads API v13 (read and write)

Good for: keyword research and account reporting, with apply-gated changes.

Examples:
- Estimate keyword volume and suggested bids and export the results.
- Preview bulk name edits from a spreadsheet, then apply with a receipt.

### Cloudflare API (read and write, heavily gated)

Good for: careful infrastructure changes with strict safety gates and file-only output for sensitive data.

Examples:
- Audit DNS records and zones before changing anything.
- Preview and apply a small change, then verify and write a receipt.

### Dynadot API3 (read and write)

Good for: domain inventory and careful bulk registrar operations.

Examples:
- Export your domain inventory and audit nameservers across domains.
- Plan a bulk nameserver update and apply only after review.

### Instantly API v2 (read and write, heavily gated)

Good for: campaign and lead operations with a “review first” workflow.

Examples:
- Add leads in bulk with a dry-run preview before applying.
- Preview an irreversible action plan, then apply using a reviewed plan file.

### Mercury API v1 (read-only)

Good for: finance visibility and exports for bookkeeping.

Examples:
- List accounts and transactions and export to a file.
- Generate a simple snapshot report for a time range.

### Stripe API (read and write, money-moving gates)

Good for: billing and payment operations with “spend money” safety gates.

Examples:
- Preview creating a product or price, then apply with verification.
- Export invoices and subscriptions for reporting.

### Shopify Admin GraphQL API (read and write)

Good for: e‑commerce operations like products, orders, customers, and discounts.

Examples:
- Preview a product creation plan, then apply.
- Export last 30 days of orders to a JSON file.

### Qdrant Cloud API (read and write)

Good for: managing vector database resources safely.

Examples:
- List clusters and collections and export inventory.
- Preview a change plan before applying.

### Zendesk Support API (read and write)

Good for: ticketing workflows with plan-first changes.

Examples:
- Export tickets for analysis.
- Preview bulk updates, then apply with a receipt.

### Pinterest API v1 (read-only)

Good for: pulling Pinterest data without posting.

Examples:
- Export boards and pins for analysis.
- Pull analytics and aggregate it for reporting.

### Statuspage public API (read-only)

Good for: simple “what is down right now” reporting from public status pages.

Examples:
- Fetch current incidents and component status.
- Generate a daily status snapshot report.

### YouTube Data API v3 (read and write, gated)

Good for: channel and video workflows with explicit safety gates for live calls.

Examples:
- Export channel and video metadata for analysis.
- Preview a write-like action plan, then apply only after review.

### X API v2 (read and write, gated)

Good for: safe social workflows where you want explicit “plan first” behavior.

Examples:
- Pull timelines or search results for analysis.
- Preview a post or DM plan, then apply only when you approve.

### Google Analytics (GA4), Google Search Console, and Google Tag Manager

Good for: measurement and tracking work, with plan-first changes and extra gates for destructive actions.

Examples:
- Export reports and audits for a date range.
- Preview tracking changes and apply only after review.

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
- sharing your API keys with us
- an SLA

## What’s next

This list will keep growing.

If there’s a specific API you want next, open an issue in the public repo and tell us:
- what outcome you want
- what the “safe dry-run plan” should look like
