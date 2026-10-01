# Danny Sourdough Schedule Planner

## What It Does

Works backward from the time someone wants a loaf of sourdough out of the oven and builds a timed, step-by-step baking plan. It lays out when to feed the starter, mix, stretch and fold, shape, proof, and bake, and flags any step that would land in the middle of the night or during a busy part of the day.

## When To Use It

Use this skill when someone wants fresh bread at a specific time, such as for a weekend dinner or a picnic, and does not want to do the timing math in their head. It is most useful when the day has fixed commitments the dough has to work around, or when the kitchen is warmer or cooler than usual.

## Inputs

- The target time the bread should be ready.
- Roughly how warm the kitchen is (cool, average, or warm).
- When the starter was last fed, and how lively it usually is.
- Whether an overnight cold proof in the fridge is an option.
- Blocks of time when the baker is unavailable, such as a morning errand or sleep.
- The number of loaves.

## Output

- A schedule with a clock time for each step, from starter feed to bake.
- A short note on how temperature shifts the timing, with an earlier and a later fallback.
- A warning for any step that conflicts with an unavailable block, plus a suggested fix.
- A one-line checklist of what to have on hand before starting.

## Example Prompt

```text
I want one sourdough loaf out of the oven by 6pm on Saturday for a
backyard dinner. My kitchen runs warm, my starter is usually ready about
5 hours after feeding, and I'm happy to proof it in the fridge overnight.
I'm out from 10am to 1pm on Saturday. Build me a schedule and tell me
if anything lands at a bad time.
```

## Safety Notes

This is a fictional practice skill. Use invented schedules, kitchens, and baking scenarios only. Do not include personal files, private notes, company or customer information, internal workflows, credentials, or anything copied from a real workplace document. The timings are casual home-baking estimates, not food-safety guidance.
