# Windows Setup Guide

Use this if you will follow the workshop on a Windows laptop.

Recommended setup: use **Windows Terminal**, **WSL Ubuntu**, and **VS Code**. Run coding commands inside the Ubuntu terminal unless a step says Windows.

Before you start, make sure you have:

- Admin access on the laptop.
- A stable internet connection.
- Enough free disk space for WSL, VS Code, and Docker Desktop.

## What To Install/Setup

- Windows Terminal
- WSL with Ubuntu
- VS Code
- VS Code WSL extension
- Git
- Node.js and npm
- uv
- Docker Desktop
- opencode
- OpenRouter account and API key
- GitHub account
- A modern browser such as Edge, Chrome, or Firefox

## 1. Install Windows Terminal

Windows Terminal is the easiest way to use PowerShell and Ubuntu side by side.

1. Open Microsoft Store.
2. Search for `Windows Terminal`.
3. Install it.
4. Open Windows Terminal.

## 2. Install WSL Ubuntu

In Windows Terminal, open a PowerShell tab and run:

```powershell
wsl --install -d Ubuntu
```

Restart if Windows asks you to.

Then open `Ubuntu` from Windows Terminal and create your Linux username and password.

Check WSL:

```bash
lsb_release -a
```

## 3. Update Ubuntu Packages

In the Ubuntu terminal, run:

```bash
sudo apt update
sudo apt upgrade -y
sudo apt install -y curl
```

## 4. Install Git

In the Ubuntu terminal, run:

```bash
sudo apt install -y git
git --version
```

Set your Git name and email if you have them:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Use the same email you use for GitHub if you have a GitHub account.

## 5. Install VS Code

Install VS Code on Windows:

1. Go to <https://code.visualstudio.com/>.
2. Download the Windows installer.
3. Install VS Code.

Then install the WSL extension:

1. Open VS Code.
2. Go to Extensions.
3. Search for `WSL`.
4. Install the Microsoft `WSL` extension.

## 6. Install Node.js and npm

opencode needs Node.js. Install Node.js inside Ubuntu.

Use the latest instructions from the official Node.js download page:

1. Go to <https://nodejs.org/en/download>.
2. Select the recommended LTS version.
3. Select `Linux`.
4. Select the install method shown for your Ubuntu setup.
5. Copy the command from the page and run it in the Ubuntu terminal.

Then check:

```bash
node --version
npm --version
```

Use Node.js 20 or newer.

## 7. Install uv

`uv` is a fast Python package and project tool. Install it inside Ubuntu:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Close and reopen the Ubuntu terminal, then check:

```bash
uv --version
```

## 8. Install Docker Desktop

Docker is useful for some coding projects. It may not be required for the first workshop exercises, but installing it now avoids delays later.

1. Go to <https://www.docker.com/products/docker-desktop/>.
2. Download Docker Desktop for Windows.
3. Install it.
4. Open Docker Desktop.
5. In Settings, enable WSL integration for Ubuntu.

Check from the Ubuntu terminal:

```bash
docker --version
docker run hello-world
```

If this fails, make sure Docker Desktop is running.

## 9. Install opencode

In the Ubuntu terminal, run:

```bash
npm install -g opencode-ai
opencode --version
```

## 10. Create An OpenRouter API Key

1. Go to <https://openrouter.ai/settings/keys>.
2. Create an account if needed.
3. Create an API key.
4. Keep the key private.

Do not commit the key, screenshot it, or paste it into public chat logs.

## 11. Clone This Workshop Repo

In the Ubuntu terminal, choose a folder and clone the repo:

```bash
mkdir -p ~/workshops
cd ~/workshops
git clone <repo-url>
cd agentic-coding-training
code .
```

Replace `<repo-url>` with the URL your instructor gives you.

VS Code should open in WSL mode. Look for `WSL: Ubuntu` in the bottom-left corner.

## 12. Connect opencode To OpenRouter

In the VS Code terminal, run:

```bash
opencode
```

Then inside opencode:

```text
/connect
```

Choose OpenRouter and paste your API key.

Then choose a model:

```text
/models
```

Free model availability changes. Use the model your instructor recommends.

## Final Check

Run these in the Ubuntu terminal before the workshop:

```bash
git --version
node --version
npm --version
uv --version
docker --version
opencode --version
code --version
```

Then start opencode in the repo:

```bash
opencode
```

Try this first prompt:

```text
Read this repository and explain it to a beginner. Do not edit files yet.
```
