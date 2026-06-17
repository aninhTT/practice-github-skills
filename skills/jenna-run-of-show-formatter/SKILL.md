# Run of Show Formatter

## What It Does

Converts a rough event schedule — bullet points, a messy notes doc, or a stream-of-consciousness list — into a clean, timed run-of-show table with columns for time, segment name, owner, and notes.

## When To Use It

Use it when you have a draft event agenda that needs to be turned into a structured run-of-show document you can share with a venue, AV team, or event staff.

## Inputs

- The raw schedule or agenda (bullet points, paragraph, or rough list).
- Event start time.
- Optional: owner names or roles to assign to each segment.
- Optional: any hard stops or fixed time anchors (e.g. "lunch must start at noon").

## Output

A Markdown table with these columns:

| Time | Segment | Owner | Notes |
|------|---------|-------|-------|

Each row represents one segment in chronological order. Fixed anchors are respected and gaps are flagged with a note.

## Example Prompt

```text
Format this into a run-of-show. Start time: 9:00 AM. Lunch is fixed at 12:00 PM.

- Welcome and intros (15 min)
- Keynote from the CEO (30 min)
- Breakout groups (45 min)
- Debrief (20 min)
- Lunch
- Afternoon workshops, two tracks (60 min)
- Closing remarks (10 min)
```

## Safety Notes

- This is a fictional skill for GitHub practice. Do not feed it real event details, internal schedules, attendee names, or confidential company information.
- Use invented event scenarios or clearly generic examples only.
- The skill does not validate venue logistics, AV requirements, or staffing — it only reformats schedule text.
