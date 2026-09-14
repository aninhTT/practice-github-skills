# Brian Lunch Rotation Picker

## What It Does

Picks where a group of friends should eat lunch, given the places they already like and the ones they have been to recently. It keeps a rough memory of the last few outings so the same two or three favorites do not quietly take over the rotation, and it screens out anything that will not work for the people actually coming.

## When To Use It

Use this skill when a standing lunch group has stalled out. It is most useful when the group is large enough that someone always has a reason the obvious pick will not work, when the same place keeps winning by default because nobody wants to argue, or when a new spot has been on the list for a month and never gets chosen.

## Inputs

- The list of candidate places, with a rough cuisine label for each.
- Which places the group visited on the last few outings, most recent first.
- Who is coming, and any food they do not eat.
- How long the group has for lunch, and how far they are willing to walk or drive.
- Any standing vetoes, such as a place someone had a bad meal at and will not go back to.
- Optional: a place someone has been wanting to try, to be given a nudge up the list.

## Output

- One recommended pick, with a sentence on why it came up now rather than later.
- Two backups, in order, for when the first choice is closed or has a long wait.
- A short note on what was ruled out and why, so nobody has to re-litigate it at the table.
- The updated recent-visit list, ready to hand back the next time the group asks.
- A flag when a candidate has gone unpicked for several rounds, so it either gets a turn or gets dropped from the list.

## Example Prompt

```text
Six of us are going to lunch tomorrow and we have about 50 minutes,
walking distance only. Our list is: the noodle place, the taco stand,
the sandwich counter, the salad spot, and the new dumpling place nobody
has tried. Last three outings were tacos, sandwiches, tacos. Two people
are vegetarian and one will not go back to the salad spot. Pick somewhere
and give me two backups.
```

## Safety Notes

This is a fictional practice skill. Use invented restaurant lists, made-up groups, and imaginary outings only. Do not include personal files, private notes, real names of coworkers or customers, company or internal information, credentials, or anything copied from a real workplace document. Dietary restrictions should be handled as plain preferences, not as health or medical information, and the skill is only a casual suggestion — anyone with a food allergy should confirm ingredients themselves.
