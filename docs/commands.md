# Command Reference

Only the basic commands students are likely to need.

## opencode

This repo uses a small `opencode.json` config, but it does not include custom opencode agents, skills, or slash commands.

If `opencode.json` changes, quit and restart opencode before testing the change.

Start opencode in the current repository:

```bash
opencode
```

Run a one-off prompt:

```bash
opencode run "Explain this repository in five bullet points"
```

## Inside opencode

Connect a provider:

```text
/connect
```

Choose a model:

```text
/models
```

## Git

Check current changes:

```bash
git status
```

Review a diff:

```bash
git diff
```

## Live Project

The repo intentionally does not include a completed live project. Students create their own project during the workshop using `docs/live-project.md` and `live-project-starter/prompts.md`.

For the default dashboard stack, ask the tool to create a small starter project:

```text
Create a student-dashboard/ starter with app.py, requirements.txt, .gitignore, and README.md. Use Python, pandas, Streamlit, and Plotly. Do not include a Kaggle dataset or credentials.
```

Verify it manually:

1. Download a Kaggle CSV into `student-dashboard/data/`.
2. Run `streamlit run student-dashboard/app.py`.
3. Check that the dashboard loads and the charts are readable.
4. Review the file changes with `git diff`.
