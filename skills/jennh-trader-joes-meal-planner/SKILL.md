# Jennh Trader Joes Meal Planner

## What It Does

Turns a week of loose dinner ideas into a simple meal plan built around one Trader Joe's run. It picks five or so easy dinners, reuses ingredients across meals so nothing half-used goes bad, writes a shopping list sorted by store section (produce, frozen, refrigerated, pantry), and flags which nights lean on a freezer shortcut so a busy evening still ends with a real dinner.

## When To Use It

Use this skill when the week ahead is busy and you want one grocery trip to cover most dinners. It helps most when you have a rough budget, a couple of picky eaters, or a fridge that always ends up with a forgotten bag of spinach. It is meant for quick weeknight cooking, not elaborate recipes.

## Inputs

- How many dinners to plan and how many people are eating.
- A rough grocery budget for the trip.
- Any dietary needs or dislikes ("no mushrooms", "one vegetarian").
- How much time is available to cook on each night.
- What is already in the fridge, freezer, or pantry.
- A few favorite items or meals to include, if any.

## Output

- A night-by-night dinner plan with a short description and rough cook time for each meal.
- A shopping list grouped by store section, with quantities.
- An estimated total cost, plus one swap to save money if it runs over budget.
- An "ingredient reuse" note showing which items carry across more than one meal.
- One backup "too tired to cook" dinner that uses freezer items.

## Example Prompt

```text
Plan five dinners for two people, Monday through Friday. Budget is about
$90. One of us is vegetarian on weekdays, and neither of us likes olives.
Monday and Thursday we only have 20 minutes to cook. We already have rice,
eggs, and half a bag of frozen peas. Build it around one Trader Joe's trip,
give me a shopping list by section, and tell me what to swap if it is over
budget.
```

## Safety Notes

This is a fictional practice skill for a public learning repository. Use invented households, made-up preferences, and placeholder budgets only. Do not include real names, home addresses, health or medical details, personal files, private notes, company or customer information, internal workflows, credentials, or anything copied from a real workplace document. Prices, product availability, and nutrition details are rough guesses for planning, not live store data, and should not be relied on for allergies or medical diets.
