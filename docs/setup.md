# Setup Guide

Use this before the workshop if possible.

If you are using Windows, start with `docs/windows-setup.md`.

## Required

- VS Code
- Git
- Node.js 20 or newer
- opencode
- OpenRouter account and API key

Optional for later projects:

- uv
- Docker Desktop

## Windows Students

Use `docs/windows-setup.md` for a full Windows + WSL setup checklist. It covers Windows Terminal, Ubuntu on WSL, VS Code, Git, Node.js, uv, Docker Desktop, opencode, and OpenRouter.

## Recommended VS Code Setup

- Open the repository root in VS Code.
- Keep one terminal for opencode.
- Keep one terminal for simple checks, such as opening a file or running a command the instructor gives you.
- Use the Source Control panel or `git diff` to review AI changes.

## Install Checks

Run these commands before the workshop:

```bash
git --version
node --version
npm --version
opencode --version
```

## OpenRouter Setup

1. Go to <https://openrouter.ai/settings/keys>.
2. Create an API key.
3. Start opencode with `opencode`.
4. Run `/connect`.
5. Select OpenRouter.
6. Paste the key.
7. Run `/models` and choose a model.

Free model availability changes. Pick a model the instructor recommends.

## If Setup Fails

- Pair with another student.
- Watch the instructor demo and run the prompts later.
- Use the docs in this repo after fixing setup.

## Security Reminder

Do not paste API keys into GitHub, committed files, screenshots, or public chat logs.
