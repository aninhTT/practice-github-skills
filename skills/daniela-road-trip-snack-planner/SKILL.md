# Daniela Road Trip Snack Planner

## What It Does

Takes the rough shape of a long drive and turns it into a made-up plan for when to stop and what to eat. It spaces the stops so nobody hits hour four on an empty stomach, splits the food between a cooler that has to stay cold and a bag that can ride up front, and says which stops are worth getting out of the car for.

## When To Use It

Use this skill when a drive is long enough that snacks stop being an afterthought — a full day on the highway, a run to a campsite with nothing open along the way, or any trip where the passengers have very different ideas about what counts as lunch. It is less useful for a short hop where one gas station will do.

## Inputs

- Total drive time, and roughly when you plan to leave.
- Who is in the car, including anyone who cannot go long between meals.
- Foods to avoid, invented for this exercise — say, one passenger who will not touch anything with peanuts.
- Cooler size, and whether there is ice or a plug for it.
- Long stretches with no services, such as a two-hour gap through open desert.
- Whether stops should be quick fuel-ups or real breaks with a walk.
- Anything that has to be eaten early because it will not survive the afternoon heat.

## Output

- A stop-by-stop timeline with a target hour for each one, and how long to plan on being parked.
- A snack assigned to each stop, sorted into cooler items and front-seat items.
- A packing list grouped by container, so the cooler gets loaded in the order things will come out of it.
- A note on the longest gap between stops, and a snack to keep within arm's reach for it.
- One fallback for the stretch where the plan is most likely to slip, such as arriving at a closed rest area.

## Example Prompt

```text
We are driving about nine hours tomorrow, leaving at 7am. Two adults and a
seven-year-old who needs to eat every couple of hours. One of us will not eat
anything with peanuts. We have a small cooler with one ice pack and no plug.
There is a long empty stretch in the middle with nothing for about two hours,
and the afternoon is going to be hot. Plan our stops and tell me what to pack
in the cooler versus the bag up front.
```

## Safety Notes

This is a fictional practice skill written for a public GitHub exercise. Use invented routes, made-up passengers, and imaginary food preferences only. Do not include personal files, private notes, real travel plans, health records, company or customer information, internal workflows, credentials, or anything copied from a real workplace document. The plan is casual trip planning, not dietary, medical, or food-safety guidance, and it should not be relied on for allergy decisions or for judging whether food has stayed cold enough to eat.
