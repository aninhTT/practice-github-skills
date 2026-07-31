# Board Game Shelf Sorter

## What It Does

Takes a messy, unordered list of board games and turns it into a tidy, browsable shelf guide. It groups games into sensible categories and produces a clean Markdown table so you can find the right game for the night at a glance.

## When To Use It

Use it when you have a pile of games (or a random list jotted in your notes) and want an organized overview — for example, when tidying a game shelf, planning a game night, or deciding what fits the group you have over.

## Inputs

- A list of board games (one per line, or comma-separated).
- Optional: player count you are planning for (e.g. "4 players").
- Optional: how you want them grouped ("by play time", "by complexity", or "by player count"). Defaults to grouping by player count.

## Output

A Markdown shelf guide containing:

- **A grouped table** with columns: Game, Best Player Count, Play Time, Complexity (Light / Medium / Heavy).
- **Section headings** for each group (e.g. "Quick Fillers", "Main Events").
- **A "Tonight's Pick" note** — one suggested game based on the optional player count, if provided.

## Example Prompt

```text
Sort these into a shelf guide, grouped by play time. I'm planning for 4 players.

"Meadow Kingdoms, Rocket Rally, Whispering Woods, Taco Tower, Star Freighter Nine, Garden Gnomes Deluxe"
```

## Safety Notes

- This is a fictional skill for GitHub practice. The game titles above are invented examples.
- Do not feed it real personal, company, or customer content.
- Complexity and play-time labels are rough, opinion-based estimates for organizing a shelf — they are not official ratings and should not be treated as authoritative.
