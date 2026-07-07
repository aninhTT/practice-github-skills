# Meeting Mood Summarizer

## What It Does

Reads a meeting transcript and returns a one-line vibe read — a plain-English description of the room's energy (e.g. "energized and aligned" or "polite but stuck") — plus the top 3 unresolved questions left open at the end.

## When To Use It

Use it after a meeting when you want a fast gut-check on how it actually went before writing up your notes, or when you missed a meeting and want more than just action items — you want to know how the room felt.

## Inputs

- The meeting transcript (plain text or copy-pasted from a notes tool).
- Optional: the stated goal of the meeting (e.g. "align on Q3 priorities").

## Output

A short summary with two parts:

- **Vibe** — one sentence describing the overall mood and energy of the meeting.
- **Open Questions** — a numbered list of up to 3 questions that came up but were not resolved by the end.

## Example Prompt

```text
Summarize the mood of this meeting and list the top 3 unresolved questions.
Goal: decide on the launch date for the new onboarding flow.

[Transcript]
Sara: I think we're close but I'm not sure the eng timeline is realistic.
Dev: We said two weeks but that assumed no bugs from the last sprint.
Sara: Right, so do we push to the 15th or hold for testing?
Dev: I'd feel better with more testing time honestly.
Sara: Let's see what Marcus thinks. Marcus, are you good with a two-week delay?
Marcus: I need to check with the vendor first. Can we decide Friday?
Sara: Works for me. Okay, I think we're aligned on waiting — let's reconnect Friday.
```

Expected output:
- **Vibe:** Cautiously aligned — the team wanted to move forward but kept deferring to missing information.
- **Open Questions:**
  1. Is the two-week engineering timeline realistic given the last sprint?
  2. What does the vendor timeline allow?
  3. Will the Friday check-in actually produce a final decision?

## Safety Notes

- This is a fictional skill for GitHub practice. Do not feed it real meeting transcripts, customer names, internal strategy, or confidential business information.
- Use invented or clearly fictional transcripts only.
- The skill reads tone and open questions — it does not assign blame, evaluate individual performance, or make decisions.
