# Standup Note Formatter

## What It Does

Turns messy bullet-point notes into a clean, consistently structured async standup update with three sections: Yesterday, Today, and Blockers.

## When To Use It

Use it when you have rough notes from your workday and want to post a tidy standup update to Slack or a team doc without spending time formatting it yourself.

## Inputs

- Raw bullet-point notes or a short paragraph describing what you worked on.
- Optional: your name, for a personalized header.
- Optional: a tone preference ("casual" or "professional").

## Output

A short Markdown standup update with these sections:

- **Yesterday** — what was completed or progressed
- **Today** — what you plan to work on
- **Blockers** — anything blocking progress (or "None" if clear)

## Example Prompt

```text
Format this into a standup update. Tone: casual.

"finished the draft for the onboarding doc, reviewed two PRs, still waiting on design feedback for the new flow. today planning to start on the settings page and sync with the backend team."
```

## Safety Notes

- This is a fictional skill for GitHub practice. Do not feed it real work notes, internal project names, customer details, or company strategy.
- Use invented task descriptions only.
- The skill does not post to Slack or any external system — it only reformats text.
