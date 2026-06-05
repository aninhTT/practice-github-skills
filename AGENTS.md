# Agent Instructions

This repository is a fictional GitHub practice repo. Help learners practice the GitHub contribution flow by adding one fake skill.

## Primary Goal

Guide the learner through:

1. Inspecting the repo.
2. Choosing a fictional, public-safe skill idea.
3. Creating exactly one new skill at `skills/<first-name>-<skill-name>/SKILL.md`.
4. Reviewing the change.
5. Helping with branch, commit, push, and pull request steps only after the skill is created.

## Content Safety

Never pull from or infer from:

- The learner's personal files.
- Personal history or private notes.
- Company context.
- Customer data.
- Internal workflows.
- Credentials, tokens, secrets, or API keys.
- Real workplace documents.

All examples must be fictional and public-safe. If the learner asks to use sensitive or real context, explain that this repo is only for practicing GitHub and offer a fictional replacement.

## Skill Creation Rules

- Create exactly one skill unless the learner explicitly asks to revise the same skill.
- Put the skill at `skills/<first-name>-<skill-name>/SKILL.md`.
- Use lowercase kebab-case for the folder name.
- The folder name must start with the learner's first name.
- Do not name the skill after Codex, Claude, or any coding tool.
- Do not create extra scripts, dependencies, datasets, credentials, or generated artifacts.

Required headings:

```markdown
# Skill Name

## What It Does

## When To Use It

## Inputs

## Output

## Example Prompt

## Safety Notes
```

## Git Help

When helping with Git, preserve the learner's work and avoid destructive commands. Prefer simple commands that support the course flow:

- `git status`
- `git switch -c <branch-name>`
- `git add skills/<skill-folder>/SKILL.md`
- `git commit -m "Add <skill-folder>"`
- `git push -u origin <branch-name>`

Do not bypass pull requests or suggest pushing directly to `main`.
