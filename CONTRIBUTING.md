# Contributing

Thanks for practicing the GitHub flow in `practice-github-skills`.

This repo is public and fictional. Your contribution should be a fake skill that helps you practice branching, committing, pushing, opening a pull request, receiving review, and merging.

## Before You Start

You don't need write access. The repo owner is on leave through the end of Q1 2027, so contributions come from forks.

1. Fork the repo: click **Fork** near the top right of the repo page, then **Create fork**.
2. Clone your fork: `git clone https://github.com/<your-username>/practice-github-skills.git`

## Contribution Steps

Create a branch:

```bash
git switch -c add-<first-name>-<skill-name>
```

Add one skill:

```text
skills/<first-name>-<skill-name>/SKILL.md
```

Commit and push to your fork:

```bash
git add skills/<first-name>-<skill-name>/SKILL.md
git commit -m "Add <first-name>-<skill-name>"
git push -u origin add-<first-name>-<skill-name>
```

Open a pull request from your fork into `main` on `aninhTT/practice-github-skills`. It will stay open until review resumes after Q1 2027, and that's expected.

## Review Checklist

Before opening your PR, confirm:

- Your folder name starts with your first name.
- Your folder name uses lowercase kebab-case.
- You added exactly one `SKILL.md`.
- Your skill uses all required headings from the README.
- Your examples are fictional.
- You did not include personal, company, customer, or sensitive information.
- You did not push directly to `main`.

## After You Open Your PR

You can't merge into this repo yourself. Your PR will be reviewed after the owner is back.

Optional: to practice merging, open a second pull request inside your fork (your branch into your fork's own `main`) and merge it there.
