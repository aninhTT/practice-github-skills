# Armie Farmers Market Haul Planner

## What It Does

Turns a budget and a short list of meals someone wants to cook into a made-up plan for a single trip to a farmers market. It works out roughly how much of each thing to buy, groups the list by the kind of stall that sells it, and suggests an order to walk the market in so the fragile and the frozen get picked up last.

## When To Use It

Use this skill when someone is heading to a market with a vague intention to "get vegetables" and comes home with four bunches of radishes and nothing for dinner. It is most useful when the trip has real constraints: a fixed budget, a set number of meals to cover, only two hands to carry things, or a market that is mostly sold out by mid-morning.

## Inputs

- A budget, and whether it is firm or a rough ceiling.
- The meals to cover, and how many people each one feeds.
- Which day and roughly what time the trip happens.
- How the haul gets home: on foot, by bike, by car, and whether there is a cooler.
- Any stalls or growers the person already plans to visit.
- Things to skip, such as an allergy, a dislike, or something already in the fridge.

## Output

- A shopping list grouped by stall type (produce, bread, dairy, eggs, flowers), with a quantity and a rough price for each line.
- A running budget total, plus a short list of what to cut first if the total comes in high.
- A walking order through those stall types, with the delicate and cold items placed at the end.
- A few swaps to fall back on when something is sold out or looks past its best.
- A note on what will not keep, so the most perishable items get cooked in the first day or two.

## Example Prompt

```text
I have about $60 for Saturday morning and I want to cook three dinners for
two people this week. One should be a soup, one a pasta, and one something
on the grill. I am walking there and back with two tote bags and no cooler,
and the trip takes twenty minutes each way. I already have olive oil, pasta,
and a block of parmesan. No mushrooms. Build me a list and tell me what
order to walk the market in.
```

## Safety Notes

This is a fictional practice skill written for a public GitHub exercise. Use invented markets, made-up stalls, and imaginary prices only. Do not include personal files, private notes, real budgets or financial details, company or customer information, internal workflows, credentials, or anything copied from a real workplace document. Prices and availability are rough guesses for planning, not quotes, and the skill offers no food-safety, nutrition, or allergy guidance — anyone with an allergy should check ingredients with the seller directly.
