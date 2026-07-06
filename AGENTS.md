# AGENTS.md

This repository is a minimal beginner-friendly workshop kit for AI coding tools such as opencode, Claude Code, and Codex.

## Project Goals

- Help students try practical AI coding workflows.
- Keep docs short and student-facing.
- Demonstrate opencode basics with OpenRouter when setup is available.
- Provide copyable commands, prompts, and starter instructions.
- Keep the live project prompt-driven, tiny, and focused on a beginner data dashboard.

## Important Constraints

- Do not commit API keys, provider credentials, screenshots containing secrets, or local auth files.
- Prefer small, reviewable documentation changes.
- Keep student-facing language direct, practical, and low-hype.
- Verify opencode config changes with `opencode debug config` when config is edited.

## Repo Structure

- `docs/` contains only setup, command, prompt, and live-project references.
- `opencode.json` contains a small project-local opencode configuration.
- `live-project-starter/` contains prompt-only materials for the live dashboard project.

## Documentation Style

- Use Markdown.
- Prefer short sections and concrete examples.
- Use numbered steps for workflows.
- Use fenced code blocks for commands and prompts.
- Avoid overpromising what AI tools can do.
- Include verification steps when documenting commands.

## Live Project Policy

The live project should be generated during the workshop in a separate folder such as `student-dashboard/`. This repo should not include that completed app, downloaded Kaggle datasets, API keys, or local credential files.
