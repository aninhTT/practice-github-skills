# Dinner Party Seating Planner

## What It Does

Takes a made-up guest list and a few simple preferences and turns them into a seating chart for a dinner party. It spreads out the big talkers, puts quieter guests next to someone easy to chat with, keeps couples together or apart based on what the host wants, and explains each choice in one line.

## When To Use It

Use this skill when you are hosting a fictional dinner for 6 to 16 people and can't decide who sits where. It helps most when the guests are a mix of people who know each other and people who don't, or when a couple of guests are known not to get along.

## Inputs

- The table shape and number of seats (round, rectangle, or two small tables).
- A list of invented guest names, each with a short note ("loves gardening", "new in town", "very chatty").
- Pairs that should sit together, and pairs that should not.
- Whether couples should sit side by side or be split up.
- Optional: seats the host wants for themselves, such as near the kitchen.

## Output

- A simple text diagram of the table with each guest's name in their seat.
- A one-line reason for each placement ("Pip sits next to Juniper because they both love gardening").
- A short list of conversation starters for each side of the table.
- One backup swap in case a guest cancels at the last minute.

## Example Prompt

```text
I'm hosting a made-up dinner for 8 at a rectangle table. Guests: Pip (loves
gardening), Juniper (new in town, a bit shy), Marco (tells long stories),
Delphine (Marco's partner), Otis (board game fan), Wren (just ran a
marathon), Bea (very chatty), and me. Keep Marco and Delphine apart, keep
Otis and Bea apart, and seat me closest to the kitchen. Show me the chart
and explain each seat.
```

## Safety Notes

This is a fictional practice skill for learning GitHub. Use invented guest names and made-up details only. Do not include real people's names, personal relationships, private notes, company or customer information, internal workflows, credentials, or anything copied from a real document. The skill only suggests seating; it does not know about real dietary needs, accessibility needs, or personal conflicts, so the host should always use their own judgment.
