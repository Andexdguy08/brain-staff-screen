# Brain · Staff · Screen — Starter Kit

From Anderson Ntuk · AI Avengers Lab

This kit is the starting point for the live build on **Wed 11 Nov, 12pm EST**. It has three parts:

| File | What it's for |
|---|---|
| `brain-template/` | A Business Brain for a sample company, Henderson Plumbing. Copy it and swap in your client's details. |
| `dashboard-brief-spec.md` | What goes on the owner's screen and in the 7am / 7pm WhatsApp brief. |
| `owner-pitch-60s.md` | How to explain all of this to a business owner in about a minute. |
| `START.md` | The paste-one-line version: Claude runs the whole kit with you as an interview. |

## The idea in one line

**Brain** knows the business. **Staff** (small AI workers) each do one job. **Screen** shows the owner what happened, on a dashboard or in a text.

None of it works unless the Brain knows the business first. So start there.

## Fastest way: paste one line into Claude

Open a new chat in [Claude](https://claude.ai) (web search on) and paste:

```
Read https://raw.githubusercontent.com/Andexdguy08/brain-staff-screen/main/START.md and run it with me.
```

It interviews you about one client (or runs demo mode with Henderson Plumbing), then builds the Brain, your first AI staff member, the owner's daily brief, and a 60-second pitch. Anything it doesn't know becomes an `[ASK OWNER]` list: your agenda for a paid discovery call.

## Use the files with Claude Code or Pi (5 minutes)

1. Copy `brain-template/` into a new folder for your client, e.g. `~/clients/acme-plumbing/brain/`.
2. Open Claude Code (or Pi) in that client folder.
3. Paste this:

```
Read every file in ./brain. You are the operations assistant for this business.
Only use facts from the brain. If something isn't in there, say so and ask.
Start by listing the open quotes older than 2 days and draft a follow-up for each,
in the voice described in brain/voice.md.
```

4. You now have your first AI staff member: a quote chaser. Read every draft before anything gets sent.

## Use it with the Claude app (no terminal)

Create a Claude Project, upload all the files in `brain-template/` as project knowledge, and paste the same prompt.

## Filling it in for a real client

Run a 45-minute call with the owner and work through `brain-template/business.md` top to bottom. Most owners have never written this down. That call is valuable in its own right, and it's how you justify a paid discovery.

## What's next

- Watch the live build to see the dashboard and the WhatsApp brief wired up.
- The 4-week cohort (starts Mon 23 Nov) covers building every layer, connecting it, and selling it to real clients.

## License

MIT. Free to use, change and share. Henderson Plumbing is fictional.
