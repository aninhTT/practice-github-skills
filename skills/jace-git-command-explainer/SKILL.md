# Jace Git Command Explainer

## What It Does

Explains a single git command in plain language before the learner runs it. It says what the command does, which of the four places it touches (working tree, staging area, local branch, remote), whether the effect can be undone, and what the learner should expect to see afterward. When a command is risky, it names the specific work that could be lost and offers a safer command that reaches the same goal.

## When To Use It

Use this skill when someone new to git has a command in front of them — copied from a tutorial, a teammate, or a coding tool — and does not want to run it blind. It is most useful for the commands that sound harmless but are not, such as `git reset --hard`, `git checkout .`, `git push --force`, and `git clean -fd`, and for the ones that are genuinely safe but feel frightening, such as `git switch -c` or `git fetch`.

## Inputs

- The git command, pasted exactly as the learner has it.
- Whether the learner has uncommitted work right now.
- Whether the branch has already been pushed to a remote.
- How confident the learner feels about running it, in their own words.
- Optionally, what they are actually trying to accomplish, so the skill can suggest a better-fitting command.

## Output

- A one-sentence plain-language summary of the command.
- A short list of what changes, labeled by which of the four places it touches.
- A reversibility verdict: safe, recoverable, or destructive — with the recovery command when one exists.
- What the learner should see in the terminal if it worked.
- A safer alternative when the command is riskier than what they are trying to do needs.

## Example Prompt

```text
I'm about to run `git reset --hard HEAD~1` because I want to undo my last
commit. I have some edits I haven't committed yet, and I already pushed the
branch. Explain what this will do before I run it, and tell me if there's a
safer way.
```

## Safety Notes

This is a fictional practice skill. Use invented repositories, made-up branch names, and sample commands only. Do not include personal files, private notes, company information, customer data, internal workflows, credentials, tokens, or anything copied from a real workplace document. The skill explains git commands and never runs them — the learner always decides whether to execute anything, and should confirm destructive commands against the official git documentation before relying on this explanation.
