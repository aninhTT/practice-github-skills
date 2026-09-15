# Pun Title Brainstormer

## What It Does

Takes a flat, literal title for a document, talk, or presentation and returns a short list of punny alternatives. Each suggestion comes with a groan rating from 1 to 5, so you can tell the mild wordplay apart from the jokes that will make a room audibly sigh.

## When To Use It

Use it when you have a working title that is accurate but forgettable, and you want a few playful options before you commit. It is most useful for internal talk titles, workshop names, newsletter subject lines, and chapter headings — anywhere a little wordplay earns attention.

Skip it when the title needs to stay strictly literal, such as legal documents, safety instructions, or anything that will be translated.

## Inputs

- The original title (required).
- Optional: the subject or one-line summary, which gives the puns something to work with.
- Optional: a tone preference — `subtle`, `playful`, or `maximum groan`.
- Optional: a maximum length in words, for slides or subject lines that have to fit.

## Output

A Markdown list of five to eight alternative titles. Each entry includes:

- **The title** itself.
- **Groan rating** — 1 (barely a pun) through 5 (unforgivable).
- **The pivot** — the word or phrase the pun turns on, so you can judge whether it will land.

Followed by a short **Top Pick** line recommending one option and saying why.

## Example Prompt

```text
Brainstorm pun titles for this. Tone: playful. Max 8 words.

Original title: "Quarterly Update on Our Sourdough Starter Program"
Subject: a fictional office club that keeps a shared sourdough starter alive
and reports on how it is doing every three months.
```

Example of the kind of output this produces:

- **A Rising Concern: Our Starter, One Quarter On** — groan 3 — pivots on "rising" (dough / worry)
- **Loaf at First Sight** — groan 5 — pivots on "love / loaf"
- **The Proof Is in the Proofing** — groan 4 — pivots on "proof" (evidence / dough stage)

## Safety Notes

- This is a fictional skill written for GitHub practice. It is not a real tool and does nothing on its own.
- Do not feed it real personal, company, or customer content. Invent a subject if you need an example.
- Puns travel badly. Wordplay that works in one language or region often means nothing in another, so treat every suggestion as a draft rather than a final choice.
- The skill has no sense of audience or occasion. It will happily suggest a joke title for a solemn topic, so a human should always make the final call.
