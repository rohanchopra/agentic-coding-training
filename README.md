# AI Coding Tools Workshop

A beginner-friendly workshop on using AI coding tools such as **opencode**, **Claude Code**, and **Codex**.

The goal is simple: show novices how to ask clear questions, inspect changes, and stay responsible for the result. This repo is intentionally documentation-first.

## What Students Need To Know

- Make one small change at a time.
- Review the diff before trusting the result.
- Never paste API keys or secrets into prompts or files.

## Files To Use

- `docs/windows-setup.md` - Windows + WSL setup checklist.
- `live-project-starter/` - optional prompts and instructions for the dashboard project.

## Quick Start For Students

1. Install VS Code, Git, Node.js, and opencode if students will follow along locally. Windows students should use `docs/windows-setup.md`.
2. Clone this repo and open it in VS Code.
3. Create an OpenRouter API key from <https://openrouter.ai/settings/keys>.
4. Start opencode from the terminal with `opencode`.
5. Run `/connect`, choose OpenRouter, and paste your API key.
6. Run `/models` and choose a free or low-cost model.
7. Ask opencode to explain the repo before making changes.

## Recommended First Prompt

```text
Read this repository and explain it to a beginner. Do not edit files yet.
```

## Basic Workflow

1. Ask the tool to explain the files.
2. Ask for one small change.
3. Review the diff.
4. Run a simple check.
5. Keep, fix, or undo the change.


## Live Project Policy

This repo should not contain a finished live project, downloaded Kaggle datasets, or credential files. Students create their own `student-dashboard/` folder during the workshop.
