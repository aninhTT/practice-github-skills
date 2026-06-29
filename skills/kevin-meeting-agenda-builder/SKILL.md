# Meeting Agenda Builder

## What It Does

Takes a meeting goal, a list of attendees, and an available time slot, then drafts a timed agenda with labeled discussion blocks and a prompt question for each topic.

## When To Use It

Use it when you need to send a calendar invite with a structured agenda but only have a rough idea of what to cover. Good for recurring syncs, project kickoffs, and cross-functional reviews.

## Inputs

- Meeting goal (one sentence describing the desired outcome).
- Attendee list (names or roles).
- Meeting duration in minutes (e.g. 30, 45, 60).
- Optional: any must-cover topics.

## Output

A Markdown agenda with:

- **Meeting title** and goal statement
- **Attendees**
- **Timed blocks** (start time offset, duration, owner, discussion prompt)
- **Parking lot** section for items that come up but need a separate follow-up

## Example Prompt

```text
Build a 45-minute agenda. Goal: align on Q3 priorities for the Acme widget launch.
Attendees: product lead, eng lead, marketing lead, project manager.
Must cover: timeline review and open blockers.
```

## Safety Notes

- This is a fictional skill for GitHub practice. Do not feed it real company strategy, customer names, internal roadmaps, or sensitive business context.
- Use invented meeting goals and fictional attendee roles only.
- The skill does not send calendar invites or access any scheduling system — it only formats text.
