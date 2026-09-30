# Leftovers Remix Planner

## What It Does

Takes an honest inventory of what is actually sitting in the fridge and proposes two or three made-up meals that use it up. It works backward from what is about to turn, so the ingredient with the shortest life gets spent first, and it tells you plainly when a combination is not worth attempting.

## When To Use It

Use this skill at the end of a week, when the fridge holds half a roast chicken, a lonely bunch of herbs, and two portions of rice from a meal you have already eaten twice. It is for the moment when you want a plan rather than a recipe — something that uses what you have instead of sending you back to the store for three more things.

## Inputs

- A list of what is in the fridge, freezer, or on the counter, with rough quantities ("about two cups of rice", "half a bunch of cilantro").
- Anything you know is close to turning, and roughly how close.
- Pantry staples you can reliably assume are on hand, such as oil, rice, pasta, or tinned tomatoes.
- How many meals you need and for how many people.
- Effort you are willing to spend, from "assemble cold in five minutes" to "happy to cook for an hour".
- Things to leave out — ingredients you are tired of, or anything you would rather not eat again this week.

## Output

- Two or three meal ideas, each with a one-line description, the leftovers it consumes, and a short list of steps.
- An order to cook them in, driven by which ingredient expires soonest.
- A short "still unclaimed" list of anything the plan does not use, with a note on whether it freezes.
- At most one or two items to pick up, flagged separately so the plan still works without them.
- A plain warning for anything that looks past its prime and should simply be thrown out rather than cooked into a meal.

## Example Prompt

```text
Help me use up what is in the fridge. I have about half a roasted chicken,
two cups of cooked jasmine rice from Tuesday, a bunch of cilantro that is
going limp, three eggs, half a jar of salsa, and a wedge of cheddar. I have
oil, onions, garlic, and tinned black beans in the pantry. I need two dinners
for two people. One should be quick on a weeknight, the other can take longer
on Saturday. Please do not make me eat plain rice again.
```

## Safety Notes

- This is a fictional practice skill written for a public GitHub exercise. Use invented fridge contents and made-up meals only.
- Do not include personal files, private notes, household records, company or customer information, internal workflows, credentials, or anything copied from a real workplace document.
- The skill does not judge food safety. It cannot tell whether something has actually spoiled, how long an item has really been refrigerated, or whether a reheating step is sufficient. Trust your own eyes and nose, and throw out anything questionable.
- The skill does not account for allergies, dietary restrictions, or nutritional needs. Check any suggestion against your own before cooking it.
