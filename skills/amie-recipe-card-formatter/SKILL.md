# Recipe Card Formatter

## What It Does

Turns a loose, free-form recipe (the kind a friend might text you) into a clean, printable recipe card with a consistent layout: title, yield, total time, ingredients list, and numbered steps.

## When To Use It

Use it when you have a recipe written as a paragraph, a screenshot transcription, or a messy bulleted list, and you want a tidy one-page card you can save, share, or stick on the fridge.

## Inputs

- The raw recipe text (paragraph or rough notes).
- Optional: desired yield (e.g. "makes 12 cookies").
- Optional: unit preference ("metric" or "imperial").

## Output

A single Markdown recipe card with these sections:

- **Title**
- **Yield**
- **Total Time**
- **Ingredients** (bulleted, with quantities first)
- **Steps** (numbered, one action per step)
- **Notes** (optional tips or substitutions)

## Example Prompt

```text
Format this into a recipe card. Yield: 4 servings. Units: metric.

"Cook some pasta. While it boils, fry garlic in olive oil until golden, add a splash of pasta water and lemon juice, toss with the drained pasta and a handful of parsley. Salt and pepper to taste."
```

## Safety Notes

- This is a fictional skill for GitHub practice. Do not feed it real personal, company, or customer content.
- Use invented recipes or clearly public examples only. Do not paste copyrighted recipes from cookbooks or paid sites.
- The skill does not check for food allergies, dietary restrictions, or food safety — it only reformats text.
