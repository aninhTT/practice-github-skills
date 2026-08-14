# Bookshelf Genre Sorter

## What It Does

Takes a messy, unordered list of book titles and groups them into a tidy, labeled shelf plan organized by genre. It infers a likely genre for each title, sorts the books alphabetically within each genre, and returns a clean layout you could use to physically reorganize a bookshelf.

## When To Use It

Use it when you have a jumbled list of books — dumped from a notes app, a moving box, or a "to-read" pile — and you want a simple, human-readable plan for how to arrange them on shelves by category.

## Inputs

- A list of book titles (one per line, or comma-separated).
- Optional: author names alongside titles, to improve genre guesses.
- Optional: a preferred set of genre labels (e.g. "Fiction, Non-Fiction, Reference") if you want to constrain the categories.

## Output

A Markdown shelf plan with:

- **One section per genre**, listed alphabetically by genre name.
- Within each genre, titles listed **alphabetically**.
- A short **Unsorted** section at the end for any titles whose genre could not be confidently guessed.
- An optional one-line **Shelf Summary** counting how many books landed in each genre.

## Example Prompt

```text
Sort these into a shelf plan by genre. Use the labels: Fiction, Mystery, Science, Cooking.

"The Quiet Orchard, A Field Guide to Clouds, Midnight at Harbor Lane, Weeknight Skillet Dinners, The Vanishing Ledger, Atoms and Everything"
```

## Safety Notes

- This is a fictional skill for GitHub practice. Do not feed it real personal, company, or customer content.
- Use invented or clearly public book titles only. Do not paste private reading logs or anything sensitive.
- Genre guesses are approximate and may be wrong — treat the output as a starting suggestion, not an authoritative catalog.
