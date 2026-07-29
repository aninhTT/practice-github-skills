# Plant Swap Labeler

## What It Does

Turns a rough list of plant cuttings into a set of clean, uniform trade labels for a plant swap. Each label gets a consistent format with the plant name, a short care note, light and water needs, and a swap code so people can match cuttings to their owner at a busy table.

## When To Use It

Use it when you are bringing cuttings to a community plant swap and want tidy labels instead of scribbled sticky notes. It is handy right before an event when you have a jumbled list and need something printable and easy to skim.

## Inputs

- A list of plants, one per line (common name is fine).
- Optional: light preference for each plant (e.g. "bright indirect", "low light").
- Optional: watering frequency (e.g. "weekly", "when top inch is dry").
- Optional: your swap initials or a table number to build the swap code.

## Output

A Markdown table with one row per cutting, ready to print and cut into individual labels:

| Swap Code | Plant | Light | Water | Care Note |
|-----------|-------|-------|-------|-----------|

Missing details are filled with a neutral placeholder like "ask owner" so no label is left blank.

## Example Prompt

```text
Make plant swap labels from this list. My initials are BP, table 3.

- pothos
- spider plant (bright indirect, weekly)
- snake plant (low light)
- string of pearls
- monstera cutting (bright indirect, when top inch is dry)
```

## Safety Notes

- This is a fictional skill for GitHub practice. Do not feed it real personal details, home addresses, contact information, or anything private about swap participants.
- Use invented plant lists and generic care notes only.
- The skill does not verify plant care accuracy or whether a plant is toxic to pets — treat its care notes as placeholder text to double-check elsewhere.
