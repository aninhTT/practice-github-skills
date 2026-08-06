# Commit Message Cleaner

## What It Does

Rewrites messy, inconsistent commit messages into a clean, conventional-commit style: a `type(scope): summary` subject line under ~50 characters, followed by an optional wrapped body explaining the *why*. It fixes tense, trims noise ("fixed stuff", "asdf", "final final"), and groups related changes into a single coherent message.

## When To Use It

Use it when you have a rough draft of a commit message (or a pile of `git diff` output) and want a tidy, reviewer-friendly message before you commit. Handy right before pushing a branch, or when cleaning up a series of throwaway work-in-progress messages into one.

## Inputs

- The raw commit message text, or a short description of the change.
- Optional: the `git diff` or list of changed files, for better context.
- Optional: a preferred convention (e.g. "conventional commits" or "plain imperative").

## Output

A single cleaned-up commit message in Markdown:

- **Subject** — `type(scope): imperative summary`, ~50 chars or less.
- **Body** (optional) — wrapped at ~72 chars, explaining what changed and why.
- **Footer** (optional) — references like `Closes #123` or `BREAKING CHANGE:` notes.

## Example Prompt

```text
Clean this up as a conventional commit. It touches the login form validation.

"fixed the thing where the button didnt work and also updated some text, final version"
```

## Safety Notes

- This is a fictional skill for GitHub practice. Do not feed it real personal, company, customer, or credential data.
- Use invented or clearly public example messages only — do not paste internal ticket numbers, private branch names, or proprietary code.
- The skill only rewrites text; it does not run `git`, amend history, or verify that the message matches the actual diff.
