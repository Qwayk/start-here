Last updated: **2026-03-19**

# Proof — how Qwayk keeps agent work safer

A lot of people now want AI agents to do real work.
That part makes sense.

The hard part is safety.

If an agent can touch real APIs, one bad action can mean:
- the wrong page gets changed
- the wrong record gets updated
- the wrong setting gets pushed live
- nobody can prove what happened after

Qwayk is built to reduce that risk.

## The simple rule

Skills tell the agent what to do.
Qwayk tools make sure the work goes through safety gates.

That means:
1) plan first
2) apply only when you approve
3) verify the result
4) keep a receipt

## What that looks like in practice

A safe run should answer four questions clearly:
- what is going to change
- what will not change yet
- what happened after apply
- what proof do I have now

If a tool cannot answer those questions clearly, it is not good enough.

## What this is not

This is not:
- blind automation
- a bot that holds your secrets for you
- "just trust the agent"

## Public proof repos

Start with these:
- Amazon PA-API v5: `https://github.com/Qwayk/amazon-pa-api-tool`
- Plausible Analytics: `https://github.com/Qwayk/plausible-api-tool`

And the front door:
- `https://github.com/Qwayk/start-here`

## If you want the full library

Support Qwayk here:
- `https://github.com/sponsors/Qwayk`
