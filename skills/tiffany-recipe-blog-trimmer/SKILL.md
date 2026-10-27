# Tiffany Recipe Blog Trimmer

## What It Does

Cuts an overlong fictional recipe blog post down to the part readers actually came for. It flags throat-clearing introductions, redundant adjectives, instructions that could be merged into one step, and background stories that delay the ingredient list. It returns a trimmed draft plus a short list of what was removed and why, so the writer can put anything back.

## When To Use It

Use this skill when a made-up recipe post has buried its ingredients under several paragraphs of preamble, or when a draft needs to hit a word count without losing the actual cooking instructions. It is for practice drafts and invented examples, not for editing a real publication.

## Inputs

- The full text of a fictional recipe blog post.
- A target length, either a word count or a rough reduction goal such as "cut by half."
- Which sections must be preserved, such as the ingredient list or allergy notes.
- Optional: the tone to keep, for example warm and chatty versus plain and quick.

## Output

- A trimmed version of the post.
- A cut list naming each removed passage and the reason, such as redundant, off-topic, or duplicated below.
- A short note on anything the skill chose not to cut because removing it would change the recipe itself.

## Example Prompt

```text
Here is a fictional blog post for lemon olive oil cake. It runs 1,400 words and
the ingredient list does not appear until paragraph nine. Trim it to about 600
words. Keep the full ingredient list and the note about substituting gluten-free
flour. Keep the friendly tone.
```

## Safety Notes

Use invented recipe posts only. Do not paste in text from a real publication, a
real author's blog, or any copyrighted article, and do not use unpublished drafts
from a workplace. Trimming changes emphasis, so always reread the result before
treating it as final. Never cut allergy information, ingredient quantities, or
food-safety steps such as cooking temperatures, even when they push the draft
over the target length.
