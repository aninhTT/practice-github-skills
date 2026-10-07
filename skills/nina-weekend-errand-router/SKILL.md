# Nina Weekend Errand Router

## What It Does

Takes a messy weekend errand list and turns it into an ordered route. It groups stops that sit near each other, puts the time-sensitive ones where they fit, gives each leg a rough travel and in-store estimate, and sorts the whole list into "must do", "nice to have", and "skip if running late" so a slow morning does not sink the afternoon.

## When To Use It

Use this skill when a weekend has more errands than hours and the order matters. It helps most when stops have hard constraints — a pickup window, a shop that closes early, frozen groceries that should be the last leg — and "just start driving" means doubling back across town twice.

## Inputs

- The errand list, in whatever order it was jotted down.
- A start time, a hard end time, and the starting point ("home", "the gym").
- Known windows or closing times for any stop.
- How long each stop realistically takes, if known.
- Mode of travel, and whether parking is a hassle anywhere.
- Anything that constrains the order, such as cold items or a bulky purchase that fills the trunk.

## Output

- A numbered route with an arrival time per stop and a running clock.
- A travel estimate for each leg, plus total time out.
- Constraint flags where the route is tight ("the key shop closes at 2 — this stop has 15 minutes of slack").
- A three-tier list: must do, nice to have, skip if running late.
- One suggested trim if the plan overruns the hard end time.

## Example Prompt

```text
Saturday, out the door at 9, need to be back by 2. Starting from home.
Errands: return a jacket at the mall, pick up a held book at the library
(closes at 1), drop two bags at the donation bin, grab a 10 lb bag of dog
food, get a key copied at the hardware shop, and a full grocery run with
frozen stuff. Driving, mall parking is slow. Route this and tell me what
to cut if I am running behind.
```

## Safety Notes

This is a fictional practice skill for a public learning repository. Use invented errand lists, made-up towns, and placeholder stop names only. Do not include real home or work addresses, real calendars, personal files, private notes, company or customer information, internal workflows, credentials, or anything copied from a real workplace document. Time and travel estimates are rough guesses for planning, not live traffic or navigation data, and should not be relied on for anything safety-critical.
