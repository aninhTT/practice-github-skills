# Contributing

Thanks for practicing the GitHub flow in `practice-github-skills`.

This repo is public and fictional. Your contribution should be a fake skill that helps you practice branching, committing, pushing, opening a pull request, receiving review, and merging.

## Before You Start

1. Open a "Request write access" issue.
2. Wait for the instructor to invite your GitHub account.
3. Accept the collaborator invitation.
4. Clone the repo.

## Contribution Steps

Create a branch:

```bash
git switch -c add-<first-name>-<skill-name>
```

Add one skill:

```text
skills/<first-name>-<skill-name>/SKILL.md
```

Commit and push:

```bash
git add skills/<first-name>-<skill-name>/SKILL.md
git commit -m "Add <first-name>-<skill-name>"
git push -u origin add-<first-name>-<skill-name>
```

Open a pull request into `main`, then wait for instructor approval.

## Review Checklist

Before opening your PR, confirm:

- Your folder name starts with your first name.
- Your folder name uses lowercase kebab-case.
- You added exactly one `SKILL.md`.
- Your skill uses all required headings from the README.
- Your examples are fictional.
- You did not include personal, company, customer, or sensitive information.
- You did not push directly to `main`.

## After Approval

After your PR is approved and checks pass, merge the PR using the option provided by GitHub.
