Last updated: **2026-02-25**

# Safe-by-default API tools for AI agents

This repo is the public **start here** for a library of safe-by-default API tools designed for AI agents and automation.

## Safety model (why this is different)

- **Dry-run by default** (you see the plan first)
- Writes require explicit **apply**
- We use **read-back verification**
- We produce **receipts/audit logs** so changes are verifiable

Proof/demo:
- `https://github.com/Qwayk/start-here/blob/main/PROOF.md`

Tools source (monorepo):
- `https://github.com/shai347/api-tools-for-ai-agents`

## What you can do with these tools

Examples:
- publish/update content safely (CMS APIs)
- run marketing/analytics reads safely (ad + analytics APIs)
- manage infra/vendor accounts safely (cloud + status + registrar APIs)

## Membership (how to get the private members repo)

We sell membership via GitHub Sponsors:
- Sponsors page: `https://github.com/sponsors/Qwayk`
- Members get access to the private members repo: `Qwayk/qwayk-tools` (private)

If the Sponsors page isn’t live yet, we’re likely in the approval/onboarding flow.

Members repo includes:
- self-serve onboarding (`START_HERE.md`)
- workflow packs
- updates/releases
- strict support boundaries (docs-first; no custom setup by default)

## Support boundary (important)

This is built to be self-serve:
- No custom setup
- No SLAs
- Don’t paste secrets into Issues/Discussions

## Where to start

1) Read the proof/demo link above.
2) If you sponsor, accept the GitHub invite to the members repo.
3) Start at `START_HERE.md` inside the members repo.
