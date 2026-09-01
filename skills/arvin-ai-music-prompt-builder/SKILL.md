# AI Music Prompt Builder

## What It Does

Turns a plain-English description of a vibe into a structured prompt spec for a fictional text-to-music AI. Instead of generating songs, this skill generates the *instructions* a music model would need: genre tags, tempo, key, instrumentation, an arrangement arc, and a list of things to avoid.

The goal is to replace vague prompts like "make something chill" with a spec that is specific enough to produce a consistent result twice in a row.

## When To Use It

- You have a mood or scene in mind but do not know how to describe it in the tags a music model expects.
- Your generated tracks keep coming out inconsistent, and you want a repeatable prompt to reuse.
- You need background music for a fictional video, game level, or podcast segment and want to spec it before generating.
- You are prototyping a music-generation UI and need realistic-looking prompt payloads as fake data.

## Inputs

- **Vibe description** (required): A short phrase describing the feeling, scene, or use case, e.g. "foggy morning drive, hopeful but tired" or "boss fight in a clockwork factory".
- **Duration** (optional): Target track length in seconds (default: 90). Drives how many arrangement sections are proposed.
- **Reference genre** (optional): A broad style to anchor on, e.g. "synthwave", "bossa nova", "orchestral". Use genres, never real artists.
- **Vocals** (optional): `none`, `wordless`, or `lead` (default: `none`).
- **Must avoid** (optional): Anything the track should not contain, e.g. "no heavy drums", "no brass".

## Output

A Markdown prompt spec with a one-line summary prompt at the top and the parameter breakdown below it:

```
## Foggy Morning Drive — Prompt Spec

**One-line prompt:** hopeful lo-fi synthwave drive at 96 BPM in A minor,
warm analog pads and muted electric bass, tape hiss, no vocals

| Parameter      | Value                                    |
| -------------- | ---------------------------------------- |
| Genre tags     | lo-fi, synthwave, downtempo              |
| Tempo          | 96 BPM                                   |
| Key            | A minor                                  |
| Instrumentation| analog pads, muted electric bass, brushed drums, tape hiss |
| Vocals         | none                                     |
| Duration       | 90s                                      |

**Arrangement arc**

1. 0:00–0:18 — Intro: pads and hiss only, no drums
2. 0:18–0:50 — Body: bass enters, brushed drums, light arpeggio
3. 0:50–1:15 — Lift: add counter-melody, open the filter
4. 1:15–1:30 — Outro: strip back to pads, fade

**Negative tags:** distorted guitar, aggressive drums, spoken word
```

Every value is derived from the vibe description. The skill explains its tempo and key choices in one sentence each so you can override them.

## Example Prompt

```
Build an AI music prompt spec for "boss fight in a clockwork factory",
60 seconds, orchestral, no vocals, must avoid electric guitar.
```

Expected output: a prompt spec with a driving tempo (around 140–160 BPM), a minor key, mechanical percussion and low strings in the instrumentation, a four-section arrangement arc that peaks near the 40-second mark, and `electric guitar` listed under negative tags.

## Safety Notes

- Describe styles with genre and instrumentation words only. Never anchor a prompt on a real artist, band, producer, or specific existing song — "in the style of <real artist>" is out of scope for this skill.
- Do not output lyrics. If vocals are set to `lead`, describe the vocal texture and delivery instead, e.g. "breathy alto, close-mic'd".
- This skill produces text specs only. It does not generate, upload, download, or play audio, and it does not call any music service.
- All example scenes must be fictional. Do not use personal listening history, private files, or any real project, company, or customer information as the vibe input.
