# Norma WFM Report Analyzer

## What It Does

Turns a week of invented workforce management figures from a make-believe contact center into a short written report. It compares how staffing actually tracked against the forecast, calls out the time blocks where coverage slipped, looks for patterns across the week, and closes with a handful of plain-language recommendations for the week ahead.

The report is written to be read aloud in a fifteen-minute stand-up, so it leads with the summary and keeps the tables small.

## When To Use It

Use this skill when someone has a pile of made-up scheduling and volume numbers and wants a readable recap instead of a raw spreadsheet. It is most useful when the question is not "what happened" but "so what should we change next week," which is the part a table never answers on its own.

It is also handy for practicing how to explain a staffing miss without blaming anyone: the fictional numbers make it safe to rehearse the wording.

## Inputs

- Invented contact volume for the week, broken into whatever time blocks the person has: hourly, half-hourly, or just morning and afternoon.
- The made-up forecast those numbers were supposed to match.
- A fictional roster: how many agents were scheduled in each block.
- Invented adherence and shrinkage percentages, if known. Rough guesses are fine.
- The pretend service level target, such as "answer 80 percent of chats within 30 seconds."
- Any imaginary one-off events worth explaining a bad day: a fake tooling outage, a made-up holiday promotion, a fictional training session that pulled half the floor offline.

Anything missing gets treated as unknown rather than filled in silently.

## Output

- A one-paragraph summary of the week in ordinary language, no jargon.
- A short table of the time blocks that missed target, with the size of the gap.
- Three to five recommendations, ordered by how much difference they would make, each with a sentence on the tradeoff.
- A watch list of trends that are not problems yet but are heading that way.
- An assumptions note listing which figures were given and which were inferred, so nothing looks more certain than it is.

## Example Prompt

```text
Meridian Support Co. is a make-believe 40-agent chat team. Last week we forecast
1,200 chats a day and actually got about 1,450 on Tuesday and Wednesday, then a
quiet Friday around 900. We schedule 12 agents in the morning block, 18 midday,
and 8 in the evening. Adherence was roughly 88 percent, shrinkage around 30
percent. Our made-up target is answering 80 percent of chats within 30 seconds.
Tuesday afternoon we also had a pretend outage in the routing tool that lasted
about two hours. Write me the weekly report and tell me what to change.
```

## Safety Notes

This is a fictional practice skill built for a public GitHub learning exercise. Use invented companies, invented staffing numbers, and made-up targets only.

Do not paste in real staffing data, real contact or customer records, real dashboard exports, real internal tooling names, actual team member names, or genuine performance targets. Workforce data touches both customer contacts and individual employee performance, so it is exactly the kind of material that does not belong in a public repository.

The recommendations this skill produces are illustrative writing practice, not real staffing, scheduling, or employment advice. Decisions that affect real people's hours should come from a person with the real numbers in front of them.
