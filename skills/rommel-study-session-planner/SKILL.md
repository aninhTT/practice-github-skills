# Study Session Planner

## What It Does

Takes a reading list and an exam date and lays out study sessions across the days in between. It splits long chapters into sittings of a workable length, spaces repeat passes over the same material a few days apart instead of stacking them, and stops filling a day once it hits the daily limit you set.

It hands back a plain day-by-day schedule. It does not connect to a calendar, send reminders, or track whether you actually studied.

## When To Use It

Reach for it when you have three weeks until an exam, a stack of chapters, and no plan — the point is to turn "study more" into a specific list of sittings with topics attached.

Good fits:

- A fixed deadline and a known, finite pile of material.
- Material that rewards revisiting, where a second pass days later beats one long cram.
- Uneven daily availability, where a flat "two hours every evening" plan would fall apart by Wednesday.

Poor fits:

- Open-ended learning with no deadline — there's nothing to work backward from.
- A reading list so short you can just sort it by hand.
- Deciding what's worth studying. This takes your list as given; it won't judge which chapters matter or predict what the exam will cover.

## Inputs

- **Reading list** (required) — the items to cover. Each needs a label and a rough size (page count, chapter count, or a time estimate). Size drives the split, so a guess is fine but a blank is not.
- **Exam date** (required) — the hard stop. Nothing gets scheduled on or after it.
- **Available days and hours** (required) — which days you can study and how long on each. Uneven is expected: 30 minutes on weekdays, three hours on Sunday.
- **Maximum session length** (optional) — longest single sitting before a break is forced in. Defaults to 50 minutes.
- **Passes per item** (optional) — how many times to revisit each item. Defaults to 2: a first read, then one review pass.
- **Priority items** (optional) — anything to schedule early rather than letting the natural order decide.

## Output

A Markdown schedule with four parts:

1. **Day-by-day plan** — each study day as a heading, with its sessions listed underneath: item, which pass this is, and how long. Days you marked unavailable are skipped, not padded with filler.
2. **Coverage table** — one row per reading-list item, showing which days its passes landed on. This is the quick check that nothing got silently dropped.
3. **Didn't fit** — items or passes with no room left before the exam date. Listed explicitly, with how much time would have been needed. Never quietly trimmed, and never pushed past the exam to force a fit.
4. **Crowding warnings** — days packed to the limit, and any item whose review pass ended up adjacent to its first pass because spacing wasn't possible. Both are signs the input was too ambitious for the time available.

## Example Prompt

```text
Plan my study sessions. The exam is in 12 days. Max 45-minute sittings, two passes
per chapter. I can study 1 hour on weekdays and 3 hours on Saturday; Sundays are out.

Chapter 1 - Cell Structure        18 pages
Chapter 2 - Membrane Transport    32 pages   (priority, I keep forgetting this one)
Chapter 3 - Photosynthesis        24 pages
Chapter 4 - Cell Division         40 pages
Lab Review Packet                 10 pages
```

Expected shape of the answer: Chapter 2 pulled to the front as a priority item and split across multiple sittings since 32 pages won't fit in 45 minutes; Chapter 4 split the most; the Lab Review Packet landing in a single sitting; every chapter's second pass placed at least a few days after its first; Saturday carrying three or four sessions while weekdays carry one; and an honest note if the 164 total pages across two passes simply don't fit in 12 days at that pace.

## Safety Notes

- This is a fictional skill written for a GitHub practice exercise. The chapters, page counts, and exam above are invented.
- Keep any real use to your own study material. Don't paste in personal, company, customer, or credential data — it has no use here, and this repo is public.
- The skill only produces text. It doesn't write to a calendar, set reminders, or modify anything, so a bad plan costs you nothing but a re-run with different inputs.
- Session lengths come from page counts, which are a crude proxy for effort — a dense 10-page proof and 10 pages of diagrams are not the same work. Treat the durations as a starting point and adjust once you know your real pace.
- Spacing between passes is best-effort. When the time available is too short, the schedule will place passes close together rather than drop them, and flag it under crowding warnings. Read those warnings as "this plan is too tight," not as a detail.
