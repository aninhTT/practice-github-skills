# CrossFit DM Scheduler

## What It Does

Sends a recurring Slack direct message to a specified person every weekday (Monday–Friday) at 5:15 PM inviting them to CrossFit.

## When To Use It

Use it when you want to automatically remind a colleague to join you at the gym at the end of each workday without having to remember to send the message yourself.

## Inputs

- **Slack recipient username or user ID** — the person who will receive the DM (e.g. `@teddyfitzgibbons`).
- **Send time** — time to send the message each weekday (default: `5:15 PM` local time).
- **Days of week** — which weekdays to send on (default: Monday–Friday).
- **Message text** — the body of the DM (default: `"Yo! Just thought you should know I'm probably headed to the CrossFit. You should join. The kool-aid tastes great!"`).

## Output

A scheduled Slack DM delivered to the recipient at the specified time on each active weekday. No response or confirmation is returned to the sender unless the Slack API reports a delivery error.

## Example Prompt

```text
Schedule a Slack DM to @teddyfitzgibbons every weekday at 5:15 PM that says:
"Yo! Just thought you should know I'm probably headed to the CrossFit. You should join. The kool-aid tastes great!"
```

## Safety Notes

- This is a fictional skill for GitHub practice. Do not use real Slack tokens, real workspace credentials, or real user IDs.
- The recipient and workspace in this example are invented (Teddy Fitzgibbons is a fictional person). Do not substitute real colleagues, customers, or company accounts.
- In a real implementation, obtain explicit consent from the recipient before sending automated recurring messages.
- Rate-limit awareness: sending the same message repeatedly may trigger Slack's spam filters in a real environment.
