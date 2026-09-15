# timenoise Secret Santa Gift Matcher

## What It Does

Takes a group of Secret Santa participants, each described in a sentence or two, and proposes a few gift ideas for whoever each person was assigned. It works from what someone actually said about themselves rather than generic categories, keeps every idea under the group's price cap, and checks the whole set at the end so two people do not turn up with the same gift.

## When To Use It

Use this skill when a group has already drawn names and everyone is stuck on what to actually buy. It helps most when the group is a mix of close friends and near-strangers, so some blurbs are detailed and others are three vague words, and when the price cap is tight enough that "just get a gift card" feels like giving up.

## Inputs

- A price cap, and whether it is a hard limit or a rough target.
- A list of participants with a short blurb each: hobbies, recent obsessions, a running joke, whatever they wrote in the group chat.
- Who drew whom, if the draw is already done. If not, the skill can suggest ideas per person instead.
- Any group rules, such as no consumables, nothing bulky to carry home, or handmade only.
- Things to avoid per person: allergies, duplicates of something they already own, a gift that fell flat last year.
- The exchange date, so it can flag ideas that will not arrive in time.

## Output

- Three gift ideas per recipient, ordered from safest to most specific, each with a one-line reason tied back to that person's blurb.
- A rough price for each idea and a note when it sits near the cap.
- A duplicate check across the full group, calling out overlapping ideas and suggesting which giver should switch.
- A flag on anything that needs lead time, such as something engraved or made to order.
- A fallback idea for each recipient whose blurb was too thin to work with, plus a suggested question to ask the group chat.

## Example Prompt

```text
Our Secret Santa cap is 25 dollars, hard limit, and we exchange on the
20th. Six of us. Priya loves cold-water swimming and complains about her
hands. Marcus just moved into a place with no kitchen storage. Ana is
learning bass. Tobias only wrote "idk, socks?" in the chat. Wen bakes
constantly. I drew Tobias. No consumables, and we all have to carry our
gifts home on the train. Give me ideas for everyone and tell me where
two of us are likely to buy the same thing.
```

## Safety Notes

This is a fictional practice skill. Use invented participants, made-up blurbs, and imaginary group rules only. Do not include personal files, private notes, real contact details, company or customer information, internal workflows, credentials, or anything copied from a real workplace document. Gift ideas are casual suggestions, not purchasing advice, and the skill should not be given payment details, saved cards, or account information of any kind.
