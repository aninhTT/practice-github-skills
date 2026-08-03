# Kyle Trail Run Route Planner

## What It Does

Suggests a fictional trail-running route based on how far you want to go, how much
climbing you're in the mood for, and how much time you have. It returns a simple
route sketch with an out-and-back or loop shape, estimated distance, rough elevation
gain, and a suggested pace band so the run fits the time available.

## When To Use It

Use it when you want a quick, low-effort trail-run idea and don't feel like planning
the route yourself. Good for deciding a weekend long run, fitting a short recovery jog
into a lunch break, or picking something with more (or less) climbing than usual.

## Inputs

- Target distance (miles or kilometers)
- Elevation preference (flat, rolling, or hilly)
- Time available (minutes)
- Optional: route shape preference (loop or out-and-back)

## Output

A short route plan containing:

- A route name and shape (loop or out-and-back)
- Estimated total distance
- Rough elevation gain
- A suggested pace band to fit the available time
- One or two notes (for example, "save energy for the climb in the back half")

## Example Prompt

> Plan me a trail run: about 6 miles, rolling hills, I have 75 minutes. Prefer a loop.

Example response shape:

> **Cedar Ridge Loop** (loop) - ~6.1 mi, ~650 ft gain. Target pace 11:30-12:30/mi to
> finish near 72 min. Note: the middle third is the hilliest, so ease into the first
> mile.

## Safety Notes

- Everything produced is fictional and for practice only. Route names, distances, and
  trails are invented and should not be treated as real navigation.
- Do not rely on this for actual wayfinding, emergency planning, or safety decisions.
- No personal, company, customer, or sensitive data is used or required.
