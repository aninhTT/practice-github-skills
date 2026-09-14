# ncambasasaki Hydration Plan Builder

## What It Does

Turns a loose description of someone's day into a simple, made-up water-drinking plan. It splits a daily target across the hours the person is actually awake, anchors each serving to something already in their day, and points out the stretches where they will most likely forget to drink.

## When To Use It

Use this skill when someone keeps meaning to drink more water and cannot make it stick. It is most useful for a day with an odd shape, such as a long drive, a stretch of back-to-back errands, or an afternoon outdoors in the heat, where "just drink eight glasses" is not much of a plan.

## Inputs

- A daily water target, in whatever unit the person thinks in (liters, ounces, or "about six bottles").
- Wake-up and wind-down times.
- A rough outline of the day: meals, travel, exercise, and any long gaps away from a tap.
- The container they will actually carry, and how much it holds.
- Anything they want counted toward the total, such as tea or sparkling water.
- Stretches when drinking is inconvenient, such as a two-hour bus ride.

## Output

- An hour-by-hour schedule of servings, each tied to an existing anchor in the day ("with breakfast", "when you park at the trailhead").
- A refill count for the chosen container, so the person knows how many times to top it up.
- A short list of likely gaps, with a nudge for each one.
- A single fallback plan for the days the schedule falls apart, so a missed morning does not turn into a skipped day.

## Example Prompt

```text
I want to drink about 2 liters tomorrow. I am up at 6:30 and in bed by 10.
I carry a 700 ml bottle. Morning is a long drive out to a lake, then a
three-hour walk in the sun with no taps, lunch out of a cooler around 1,
and the drive home. Tea in the evening should count. Build me a plan and
tell me where I am most likely to fall behind.
```

## Safety Notes

This is a fictional practice skill. Use invented schedules and made-up daily routines only. Do not include personal files, private notes, health records, company or customer information, internal workflows, credentials, or anything copied from a real workplace document. The plan is casual everyday scheduling, not medical, clinical, or athletic advice, and it should not be used for anyone with a fluid restriction or a medical condition.
