# Divya Book Club Pick Ranker

## What It Does

Takes a short list of invented book nominations for a fictional book club and turns them into a ranked shortlist. For each pick it gives a one-line rationale, flags how it fits the group's stated preferences, and notes a rough reading commitment so the club can pick realistically.

## When To Use It

Use this skill when a made-up book club has more nominations than it can read and wants a friendly, explainable ranking instead of a coin flip. It also works for practicing how to turn loose group preferences into a clear, ordered recommendation.

## Inputs

- A fictional list of nominated titles, with optional made-up authors.
- The group's stated preferences, such as preferred genres or themes to avoid.
- The meeting cadence, for example monthly or every six weeks.
- An optional page-count or length limit.
- Any invented notes about what the club read recently, so picks do not repeat a theme.

## Output

A ranked shortlist of the nominations, where each entry includes:

- The rank and title.
- A one-line rationale for the placement.
- Which stated preference it satisfies.
- A rough reading commitment relative to the meeting cadence.

Followed by a short "runner-up" note on any nomination worth revisiting next cycle.

## Example Prompt

```text
My fictional book club nominated four made-up titles: "The Lantern Keeper's Atlas",
"Salt and Other Small Mercies", "Nine Doors to Nowhere", and "A Field Guide to
Quiet Towns". The group prefers character-driven stories, wants to avoid horror,
meets monthly, and would rather stay under 400 pages. We just finished something
very plot-heavy. Rank these and tell me why.
```

## Safety Notes

Use invented book titles, fictional authors, and made-up club members only. Do not use real reading lists, private group chats, personal notes, company book clubs, employee names, customer data, or anything copied from a real workplace document. Rankings produced by this skill are a fictional practice exercise and are not recommendations about real published books.
