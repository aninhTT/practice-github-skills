# Tide Pool Visit Planner

## What It Does

Turns a stretch of coastline and a few free days into a made-up plan for visiting tide pools. It finds the low-tide windows worth walking, works backward to a departure time, and says plainly when the water will start coming back in. The plan treats the turnaround time as the fixed point and everything else as negotiable, because the tide is the one part of the day that does not care about the schedule.

## When To Use It

Use this skill when someone wants to go looking at tide pools and cannot tell a good window from a bad one. It is most useful for a first visit to an unfamiliar shoreline, a day with only one usable low tide, or a trip where children or a slow walker make the return leg take twice as long as the way out.

## Inputs

- The stretch of coast to visit, described loosely ("the rocky point north of the harbor").
- Which days are available, and any hard limits on start or end time.
- A tide table for those days, or the low-tide times if already known.
- How long the walk out to the pools takes, and whether the return is over the same ground.
- Who is coming, and the slowest walking pace in the group.
- Footwear and gear already owned, so the plan can flag only what is missing.
- Sunrise and sunset times, if the window falls near either end of the day.

## Output

- A ranked list of usable low-tide windows across the available days, with the best one called out and a one-line reason.
- A departure time for the chosen window, worked backward from the turnaround.
- A turnaround time stated as a hard limit, plus what the water will be doing after it.
- A short gear list, split into what is needed and what is only nice to have.
- A list of conditions that should cancel the trip outright, such as a high swell forecast.
- One alternate plan for the day the tide window is missed.

## Example Prompt

```text
I want to see tide pools at the rocky point north of the harbor, either
Saturday or Sunday. Low tide is 7:10am Saturday and 8:40am Sunday. The walk
out is about 25 minutes over loose rock, same way back, and my nephew is 7
so figure double that returning. We have boots but no headlamps. Sunrise is
6:45. Pick the better day, tell me when to leave, and give me a turnaround
time I should not argue with.
```

## Safety Notes

This is a fictional practice skill built for a GitHub exercise. Use invented shorelines, made-up tide tables, and imaginary trips only. Do not include personal files, private notes, location history, company or customer information, internal workflows, credentials, or anything copied from a real workplace document.

The output is casual trip scheduling, not a marine safety tool. A real visit should be planned against an official tide table and local conditions, never against times produced by this skill. Rising water, swell, and slippery rock are genuine hazards, so the plan should always err toward leaving early. Tide pools are living habitat: the plan assumes looking rather than collecting, and that animals stay where they are found.
