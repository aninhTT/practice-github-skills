# Bookshelf Swap Tracker

## What It Does

Turns a messy pile of notes about a neighborhood book swap into a single, readable lending table. It figures out which book went to which person, when it was lent, and when it is due back, then flags anything that is overdue or missing a return date.

## When To Use It

Use it when a casual book swap has outgrown a group chat — you have scattered notes like "gave Marisol the sci-fi one, maybe two weeks?" and you want one tidy table you can post or print. It is also handy right before a swap meetup, when you want a quick list of what should be coming back.

## Inputs

- The raw lending notes (chat snippets, scribbled lines, or a rough list).
- Optional: default loan length in days (defaults to 21).
- Optional: today's date, so overdue items can be flagged.
- Optional: sort preference — `due-date`, `borrower`, or `title`.

## Output

A single Markdown table with these columns:

- **Title**
- **Borrower**
- **Date Lent**
- **Due Back** (calculated from the default loan length when not stated)
- **Status** — `Out`, `Due soon`, `Overdue`, or `Returned`

Followed by two short lists:

- **Needs Follow-Up** — overdue books and who has them.
- **Missing Details** — entries where the title, borrower, or lend date could not be determined.

## Example Prompt

```text
Tidy these book swap notes into a tracker. Default loan length: 21 days. Today is March 14. Sort by due date.

"Lent The Salt Road to Marisol on Feb 20. Priya took the little green poetry book, I think Mar 1. Devon still has Winter Orchard from January — need that back. Kwame returned Tidepools last week."
```

## Safety Notes

- This is a fictional skill written for GitHub practice. The people and book titles above are invented.
- Do not feed it real personal, company, or customer information — no addresses, phone numbers, or contact details for actual neighbors.
- It only reorganizes text. It does not send reminders, contact anyone, or store data anywhere.
- Dates it calculates are estimates based on the difference between the lend date and the default loan length, so confirm anything important with the borrower.
