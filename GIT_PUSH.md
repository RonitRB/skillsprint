Git push / GH CLI instructions

Option A — Create & push with GitHub CLI (recommended if `gh` installed):

```bash
# from project root
gh repo create RonitRB/skillsprint --public --source=. --remote=origin --push
```

If `gh` prompts to authenticate, follow the prompts.

Fallback if remote already has commits (merge histories):

```bash
# merge remote main into local allowing unrelated histories
git pull origin main --allow-unrelated-histories
# resolve conflicts if any, then:
git add -A
git commit -m "chore: merge remote"
git push -u origin main
```

Local commit steps I ran/that you can re-run:

```bash
git add -A
git commit -m "chore: rebrand to SkillSprint, add env templates and docs"
git push -u origin main
```

If push fails due to authentication, open a browser and authenticate `gh` or set up an SSH key and add it to GitHub.
