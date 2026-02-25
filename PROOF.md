Last updated: **2026-02-25**

# Proof — what “safe-by-default” means here

Ok so… a lot of agent stuff online is “look, it did the thing”.

That’s cool, but it’s also how you end up with:
- the wrong DNS record
- a deleted campaign
- a broken post/page
- a mess you can’t undo

So I built everything around one rule:
**you see the plan first, and nothing writes unless you explicitly apply.**

## The safety flow

1) **Dry-run**: the tool prints a plan of what it *would* do.
2) **You review**: if the plan looks wrong, you stop.
3) **Apply**: you run the same command with `--apply` (and sometimes `--yes`).
4) **Verify**: the tool reads back the API and confirms the new state.
5) **Receipt**: you get a small artifact you can save for auditing.

## A tiny example

Dry-run might say:
- “I’m going to update `example.com` DNS A record from `1.2.3.4` to `5.6.7.8`.”

Apply is explicit:
- same command + `--apply`

Verify might say:
- “Read-back confirms A record is now `5.6.7.8`.”

Receipt might include:
- timestamp
- what you changed
- what was verified

## What this is / isn’t

This is:
- tools + workflow packs for safe automation through APIs
- self-serve by default

This isn’t:
- a bot that holds your credentials
- a done-for-you service
- “trust me bro” automation

## Get access

- Sponsors: `https://github.com/sponsors/Qwayk`
- Public start here: `https://github.com/Qwayk/start-here`
