# CTO Events Intake

## What It Does

Mocks up a Slack workflow called **CTO Events Intake**. When someone starts the workflow, it opens a short form that collects the seven answers an events team needs before planning a CTO-hosted event. It then posts a tidy summary to a fictional `#cto-events-intake` channel so the events team can pick it up.

The workflow asks these seven questions, in this order:

| # | Question | Field type | Required |
|---|----------|------------|----------|
| 01 | **Purpose:** Why are we holding this event? | Long text | Yes |
| 02 | **Desired outcomes:** What should attendees leave with or do afterward? | Long text | Yes |
| 03 | **Executive sponsor:** Who is the executive sponsor? | Person picker | Yes |
| 04 | **Planning lead:** Who is the day-to-day planning lead? | Person picker | Yes |
| 05 | **Estimated attendance:** About how many people will attend? | Dropdown: 1–25, 26–75, 76–150, 151+ | Yes |
| 06 | **Preferred dates:** What dates or date ranges work? List backups too. | Short text | Yes |
| 07 | **Location preferences:** Where should it happen? | Dropdown: In person, Virtual, Hybrid, plus a short-text note for city or venue ideas | No |

## When To Use It

Use it when you want to practice designing a Slack intake workflow, or when you need a pretend example of how an events team could collect the basics before an intake conversation. Having these seven answers ready makes the intake conversation much shorter.

## Inputs

- A trigger. In this mockup, that's a Slack shortcut or a link bookmarked in the `#cto-events-intake` channel.
- The requester's answers to the seven form questions above.

## Output

1. **Form:** a Slack form titled "CTO Events Intake" with the seven fields in the table above.
2. **Channel post:** a message posted to `#cto-events-intake`:

   ```text
   :calendar: New CTO Event Request from @{requester}

   01 Purpose: {purpose}
   02 Desired outcomes: {desired_outcomes}
   03 Executive sponsor: @{executive_sponsor}
   04 Planning lead: @{planning_lead}
   05 Estimated attendance: {estimated_attendance}
   06 Preferred dates: {preferred_dates}
   07 Location preferences: {location_format} – {location_notes}

   Next step: the Events team will reply in this thread to schedule intake.
   ```

3. **DM confirmation:** a direct message to the requester: "Thanks! Your CTO event request is in. The Events team will follow up in #cto-events-intake."

### Workflow Steps (Mockup)

```text
Step 1  Trigger        → Shortcut "CTO Events Intake" or channel link
Step 2  Collect info   → Form with questions 01–07
Step 3  Send message   → Post summary to #cto-events-intake
Step 4  Send message   → DM confirmation to the requester
```

## Example Prompt

```text
Run the CTO Events Intake workflow mockup with this fictional request:

Purpose: Host a fall tech talk series on building with robots.
Desired outcomes: Engineers share three demo projects and sign up for a hack week.
Executive sponsor: @pat-example
Planning lead: @river-example
Estimated attendance: 76–150
Preferred dates: Week of March 9, backup the week of March 16
Location preferences: Hybrid, a downtown event space in Sample City

Show me the form and the channel post it would create.
```

## Safety Notes

- This is a fictional skill for GitHub practice. It's a mockup, not a live Slack workflow.
- Don't enter real event plans, real people's names, budgets, or internal company information. Use made-up handles like `@pat-example`.
- The channel name and the people in the example are invented.
