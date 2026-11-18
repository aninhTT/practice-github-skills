# CTO Events Intake

## What It Does

Mocks up a Slack workflow called **CTO Events Intake**. When someone starts the workflow, it opens a short form that collects the nine answers an events team needs before planning a CTO-hosted event. It then posts a tidy summary to a fictional `#cto-events-intake` channel so the events team can pick it up.

The workflow asks these nine questions, in this order:

| # | Question | Field type | Required |
|---|----------|------------|----------|
| 01 | **Event name:** What is the event called? | Short text | Yes |
| 02 | **Preferred dates:** What dates or date ranges work? List backups too. | Short text | Yes |
| 03 | **Estimated attendance:** About how many people will attend? | Short text | Yes |
| 04 | **Location preferences:** Where should it happen? Add 2 to 3 location preferences in order of preference. | Short text | No |
| 05 | **Location considerations:** Add details that give more weight to your location preferences. Example: "We want Seattle because half of the team is located in Seattle." | Long text | No |
| 06 | **Purpose:** Why are we holding this event? | Long text | Yes |
| 07 | **Desired outcomes:** What should attendees leave with or do afterward? | Long text | Yes |
| 08 | **Executive sponsor:** Who is the executive sponsor? | Person picker | Yes |
| 09 | **Planning lead:** Who is the day-to-day planning lead? | Person picker | Yes |

## When To Use It

Use it when you want to practice designing a Slack intake workflow, or when you need a pretend example of how an events team could collect the basics before an intake conversation. Having these nine answers ready makes the intake conversation much shorter.

## Inputs

- A trigger. In this mockup, that's a Slack shortcut or a link bookmarked in the `#cto-events-intake` channel.
- The requester's answers to the nine form questions above.

## Output

1. **Form:** a Slack form titled "CTO Events Intake" with the nine fields in the table above.
2. **Channel post:** a message posted to `#cto-events-intake`:

   ```text
   :calendar: New CTO Event Request from @{requester}

   01 Event name: {event_name}
   02 Preferred dates: {preferred_dates}
   03 Estimated attendance: {estimated_attendance}
   04 Location preferences: {location_preferences}
   05 Location considerations: {location_considerations}
   06 Purpose: {purpose}
   07 Desired outcomes: {desired_outcomes}
   08 Executive sponsor: @{executive_sponsor}
   09 Planning lead: @{planning_lead}

   Next step: the Events team will reply in this thread to schedule intake.
   ```

3. **DM confirmation:** a direct message to the requester: "Thanks! Your CTO event request is in. The Events team will follow up in #cto-events-intake."

### Workflow Steps (Mockup)

```text
Step 1  Trigger        → Shortcut "CTO Events Intake" or channel link
Step 2  Collect info   → Form with questions 01–09
Step 3  Send message   → Post summary to #cto-events-intake
Step 4  Send message   → DM confirmation to the requester
```

## Example Prompt

```text
Run the CTO Events Intake workflow mockup with this fictional request:

Event name: Robot Builders Tech Talk Series
Preferred dates: Week of March 9, backup the week of March 16
Estimated attendance: About 120
Location preferences: 1) Sample City, 2) Example Town, 3) Virtual
Location considerations: We want Sample City because most of the speakers already live there.
Purpose: Host a fall tech talk series on building with robots.
Desired outcomes: Engineers share three demo projects and sign up for a hack week.
Executive sponsor: @pat-example
Planning lead: @river-example

Show me the form and the channel post it would create.
```

## Safety Notes

- This is a fictional skill for GitHub practice. It's a mockup, not a live Slack workflow.
- Don't enter real event plans, real people's names, budgets, or internal company information. Use made-up handles like `@pat-example`.
- The channel name and the people in the example are invented.
