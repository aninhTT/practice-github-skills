# Playlist Mood Matcher

## What It Does

Generates a fictional playlist of 8–12 song titles and artists that match a described mood, vibe, or activity. All artists and tracks are invented; no real music catalog is required.

## When To Use It

- You want a quick set of themed song suggestions for a fictional scenario (study session, road trip, dinner party, workout).
- You are writing a story or script and need plausible-sounding background music cues.
- You want to prototype a music-recommendation UI with realistic-looking fake data.

## Inputs

- **Mood or activity** (required): A short phrase describing the feeling or setting, e.g. "rainy afternoon focus session" or "upbeat morning run".
- **Genre hint** (optional): A broad style preference, e.g. "lo-fi", "pop", "jazz", "synthwave".
- **Length** (optional): How many tracks to generate (default: 10).

## Output

A numbered playlist in Markdown format:

```
## Rainy Afternoon Focus — 10 Tracks

1. "Still Water" — The Harbour Lights
2. "Grey Pane" — Nora Velt
3. "Drip Clock" — Ambient Module
...
```

Each entry is a fictional song title in quotes followed by a fictional artist name.

## Example Prompt

```
Create a 10-track playlist for a rainy afternoon focus session, lo-fi style.
```

Expected output: a numbered Markdown list of 10 fictional song titles and artist names fitting a calm, drizzly, concentration-friendly mood.

## Safety Notes

- All song titles and artist names must be entirely fictional. Do not name real bands, labels, or songs.
- Do not include lyrics, album art, streaming links, or any real intellectual property.
- Do not infer or use personal music history, listening data, or private preferences.
