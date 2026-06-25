# Houseplant Watering Scheduler

## What It Does

Turns a list of made-up houseplants into a tidy weekly watering chart. It groups plants by how thirsty they are, spreads waterings across the week so you are not soaking everything on the same day, and adds short reminders for things like rotating a plant toward the light or misting.

## When To Use It

Use this skill when a learner wants to practice describing a simple scheduling workflow with invented plant data, such as planning a watering routine for a pretend apartment full of fictional houseplants.

## Inputs

- A list of fictional houseplants (names can be invented, e.g. "Sir Fronds-a-Lot").
- A rough watering need for each plant ("thirsty", "average", or "low-water").
- Which days of the week the learner is usually home.
- Optional: any plant that needs extra care notes (misting, rotating, low light).

## Output

A Markdown weekly chart that:

- Lists each day of the week with the plants to water that day.
- Balances the workload so no single day is overloaded.
- Marks each plant with its thirst level.
- Adds short care reminders next to plants that need them.

## Example Prompt

```text
Here are five made-up houseplants with invented names and thirst levels. I'm home on Mondays, Wednesdays, and weekends. Build me a weekly watering chart that spreads the work out and adds care reminders.
```

## Safety Notes

Use invented plant names, schedules, and care notes only. Do not include real home addresses, personal location history, private contacts, photos, or any real data tied to a specific person or residence. This is a fictional practice skill.
