# Weekly To-Do Builder

## What It Does

Runs every Friday at end of day. Scans the week's Slack messages and meeting notes,
extracts action items, follow-ups, and unresolved threads, and produces a prioritized
to-do list to tackle the following week.

## When To Use It

Use this skill on Friday afternoons when you want a clean, consolidated list of
next-week priorities without having to manually re-read every conversation and note
from the week.

## Inputs

- Slack messages from the current week (DMs, group DMs, and relevant channels)
- Meeting notes from the current week (e.g. from a note-taking tool like Granola)
- Optional: a list of channels or people to focus on

## Output

A prioritized weekly to-do list grouped by category (e.g. Follow-ups, Decisions
Needed, In Progress, FYI / No Action). Each item includes a one-line description
and the source it came from (meeting or Slack thread).

Example output:

**Follow-ups**
- [ ] Send budget estimate to fictional-manager@example.com (from: Friday team sync)
- [ ] Confirm timeline with the vendor on the Q3 project (from: Slack DM)

**Decisions Needed**
- [ ] Decide on rollout approach for the new onboarding flow (from: Wednesday planning call)

**In Progress**
- [ ] Finish draft of the fictional project proposal (from: Tuesday standup)

## Example Prompt

```text
It's Friday EOD. Please review my Slack messages and meeting notes from this week
and give me a prioritized to-do list for next week. Group items by: Follow-ups,
Decisions Needed, In Progress, and FYI / No Action.
```

## Safety Notes

This skill accesses Slack and meeting notes. Only run it on accounts and workspaces
you are authorized to access. Do not include customer names, credentials, confidential
business data, or any sensitive information in the output. All example content above
is fictional.
