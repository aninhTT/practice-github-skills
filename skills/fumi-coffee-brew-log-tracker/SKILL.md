# Fumi Coffee Brew Log Tracker

## What It Does

Turns a running log of fictional pour-over brews into a readable table and picks the single next variable to change. It normalizes inconsistent notes ("med-fine", "medium fine", "18 clicks") into one grind vocabulary, computes the brew ratio from dose and yield, and flags entries where a taste note and the numbers disagree — like a "sour, weak" cup logged at a long brew time.

## When To Use It

Use it when you have a handful of invented brew entries and want a tidy log plus one concrete experiment for the next cup. Good after a week of casual note-taking, when the notes are too messy to compare and you can't tell which knob actually moved the flavor.

## Inputs

- A list of fictional brews, one per line, in any rough format.
- Per brew, whatever is available: dose in grams, yield in grams, grind setting, water temperature, total brew time, and a short taste note.
- Optional: the brewer being used (e.g. a made-up cone dripper or press).
- Optional: the flavor you are chasing, such as "less sour" or "more body".

## Output

A short Markdown report:

- **Log table** — one row per brew with dose, yield, ratio (e.g. `1:16`), grind, temp, time, and taste note.
- **Patterns** — two or three observations tying the numbers to the taste notes.
- **Next experiment** — exactly one variable to change, the direction to move it, and what to expect if the guess is right.
- **Gaps** — fields missing from the log that would make the next comparison cleaner.

## Example Prompt

```text
Here are five fake brews from my notebook. Tidy them into a log and tell me
what to change next. I want less sourness.

18g in, 290g out, med-fine, 96C, 2:45, "bright but sour, thin"
18g / 300g, medium, 94C, 3:10, "better, still tart"
17g -> 280g, med-coarse, 95C, 2:30, "sour, watery"
18g in 295 out, fine, 93C, 3:40, "muddy, bitter finish"
18/300, med-fine, 96C, 3:05, "balanced, best so far"
```

## Safety Notes

- This is a fictional skill written for GitHub practice. Invent the brew log; do not paste personal files, private notes, company data, customer information, or credentials into it.
- The skill only reasons over numbers and taste notes you provide. It does not measure anything, connect to a scale or kettle, or read from any device or account.
- Its suggestions are guesses from a tiny sample, not calibrated advice — treat the "next experiment" as one thing to try, not a correct answer.
