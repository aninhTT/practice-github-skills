# practice-github-skills

This is a practice repository for learning the GitHub contribution flow.

You will use Codex, Claude Code, or another coding assistant to explore this repo, create a fake skill, push your work on a branch, open a pull request, receive instructor approval, and merge.

Everything in this repo is fictional. Do not use personal context, private files, customer data, credentials, company information, internal workflows, or anything sensitive. The goal is to practice GitHub, not to build a real production skill.

## What You Will Practice

- Requesting temporary write access to a repo.
- Cloning a shared repository.
- Asking a coding tool to explain an unfamiliar repo.
- Creating a branch.
- Authoring a small Markdown-based skill.
- Committing and pushing changes.
- Opening a pull request.
- Responding to instructor review.
- Merging after approval.

## Learner Flow

1. Request write access by opening a "Request write access" issue in this repo.
2. Wait for the instructor to invite your personal GitHub account as a temporary collaborator.
3. Accept the GitHub collaborator invitation.
4. Clone the shared repo:

   ```bash
   git clone https://github.com/aninhTT/practice-github-skills.git
   cd practice-github-skills
   ```

5. Open the repo in Codex or Claude Code.
6. Ask your coding tool to explain the repo:

   ```text
   What is in this repo? Explain the folder structure and tell me what kind of fake skill I should add for this GitHub practice exercise.
   ```

7. Create a branch. Use your first name and a short skill idea:

   ```bash
   git switch -c add-amie-spreadsheet-cleaner
   ```

8. Ask your coding tool to create one fake skill:

   ```text
   Create one fake, public-safe skill for this practice repo. My first name is Amie. The skill should be about cleaning spreadsheet data. Follow the README, AGENTS.md, and CLAUDE.md instructions. Do not use personal, company, customer, or real private context.
   ```

9. Review the change locally.
10. Commit and push your branch:

    ```bash
    git add skills/<your-skill-folder>/SKILL.md
    git commit -m "Add <your-skill-folder>"
    git push -u origin <your-branch-name>
    ```

11. Open a pull request into `main`.
12. Wait for instructor approval.
13. After approval and passing checks, merge the pull request.

## Skill Naming Rules

Each skill must live at:

```text
skills/<first-name>-<skill-name>/SKILL.md
```

Folder names must follow these rules:

- Use lowercase kebab-case.
- Start with your first name.
- Use 2-4 short words after your first name.
- Describe the job the skill performs, not the coding tool used to write it.
- Keep it fictional and public-safe.

Good examples:

- `amie-spreadsheet-cleaner`
- `chris-meeting-notes-drafter`
- `maya-candidate-email-helper`
- `jordan-policy-summary-writer`

Avoid:

- `my-skill`
- `test-skill`
- `codex-helper`
- `claude-skill`
- `real-customer-analysis`
- `company-roadmap-summarizer`
- anything using private, personal, company, customer, or sensitive context

## Skill Structure

Create exactly one `SKILL.md` file in your skill folder:

```text
skills/<first-name>-<skill-name>/
  SKILL.md
```

Your `SKILL.md` must use this structure:

```markdown
# Skill Name

## What It Does

## When To Use It

## Inputs

## Output

## Example Prompt

## Safety Notes
```

## Public-Safe Content Rules

Use fictional examples only.

Do not include:

- Personal files or personal history.
- Private notes.
- Company data.
- Customer names or customer data.
- Internal tools, systems, strategy, or workflows.
- Credentials, tokens, API keys, or secrets.
- Anything copied from a real workplace document.

If your coding tool suggests using real context, stop and redirect it:

```text
This is a fake public practice repo. Do not use personal, company, customer, or private context. Please invent a fictional example instead.
```

## Example Coding Tool Prompts

Use these prompts inside Codex or Claude Code.

Explore the repo:

```text
Please inspect this repo and explain what it is for. Summarize the files that matter for this GitHub practice exercise.
```

Pick a fake skill:

```text
Suggest three fake, public-safe skills I could add. Each skill name must start with my first name and use lowercase kebab-case.
```

Create the skill:

```text
Create one fake skill under skills/<first-name>-<skill-name>/SKILL.md. Follow the required headings in README.md. Do not use personal context, company data, customer data, secrets, or real workflows.
```

Prepare the pull request:

```text
Review my changes, confirm they follow the repo rules, then help me commit, push my branch, and open a pull request.
```

## Instructor Notes

For the intended course flow:

- Add learners as temporary collaborators with write access after they request it.
- Protect `main`.
- Require a pull request before merge.
- Require one approving review.
- Require the validation workflow to pass.
- Allow squash merge only.
- Remove learner write access after the course or exercise is complete.
