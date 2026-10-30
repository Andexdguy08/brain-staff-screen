# The Screen — Dashboard + Daily Brief Spec

The owner sees the business two ways: **a dashboard** (when he wants to look) and **a text** (which comes to him). Build the text first. Most owners never open dashboards, but they all read their messages.

## The 4 tiles

| Tile | Shows | Comes from | Why the owner cares |
|---|---|---|---|
| **Calls caught** | Missed calls the AI texted back · how many became leads | missed-call log | "I didn't lose those jobs" |
| **Quotes chased** | Open quotes · follow-ups sent · quotes won this week | `open-quotes.md` + log | "Money stopped leaking from my inbox" |
| **Reviews earned** | Review requests sent · new reviews · current rating | review log + Google | "My reputation grows on its own" |
| **$ recovered (est.)** | Value of jobs won from caught calls + chased quotes | the three tiles above | **The reason he keeps paying** |

Rules:
- Four tiles at most. If it needs explaining, it doesn't belong on the screen.
- Each tile shows **this week vs last week**.
- Under the tiles, add a short **"Needs you"** list: items the AI escalated, oldest first.
- Label "$ recovered" honestly as an estimate (the job value from the quote or price list).

## The 7am brief (WhatsApp / SMS)

```
Morning Mike ☕ Here's Henderson Plumbing today:

📞 Yesterday: 4 missed calls caught → 3 leads, 1 booked
💬 Quotes: chased 3 · Linda Park said YES ($1,690)
⭐ 1 new 5-star review (Tom Becker)

Needs you (2):
1. The Grill House wants a quarterly contract. Call Andre?
2. James Ortiz asked about financing on the tankless.

Reply 1 or 2 to deal with it, or "chase Ortiz" and I'll handle it.
```

## The 7pm brief

```
Evening Mike. Today: 6 jobs done, 2 new quotes out ($2,330),
1 review request sent. Tomorrow starts at 7:30 with Linda Park (water heater).
Nothing urgent. 👍
```

Brief rules:
- Under 10 lines. Numbers first, then "Needs you".
- **Two-way:** the owner can reply in plain words and the AI acts on it, within the rules in `brain/sops/`.
- If nothing needs him, say so. That's the best message he'll get all day.

## Channels
- **SMS:** US default. Business sending needs A2P 10DLC registration (takes a few days).
- **WhatsApp:** official Business API through Meta or Twilio. Use the Twilio Sandbox for demos.
- **Telegram:** easiest to build, rarely used by US trades.
- **iMessage:** no official API. Don't promise it.

## Weekly (Monday 7am)
Same format, covering the whole week, plus one line: *"Your AI staff recovered about $X this week."*
