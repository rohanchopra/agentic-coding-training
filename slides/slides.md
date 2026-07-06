---
theme: default
title: AI Coding Workshop
info: |
  Introduction to AI coding tools with opencode
class: text-center
drawings:
  persist: false
transition: slide-left
mdc: true
---

# AI Coding Workshop

Use AI tools to code faster while staying in control.

---
layout: center
class: text-left
---

<div class="max-w-5xl mx-auto">

<div class="grid grid-cols-2 gap-8 items-start">

<div>

<h1 class="!text-5xl !leading-tight mb-3">Rohan Chopra</h1>

<p class="text-2xl opacity-75 mb-6">Machine Learning Engineer</p>

<p class="text-xl leading-relaxed">
I build end-to-end ML and AI systems that help business users make better decisions with data.
</p>

</div>

<div class="space-y-4">

<div class="rounded-xl bg-blue-50 p-4">
<p class="font-bold text-blue-700">ML/AI since 2018</p>
<p class="text-sm opacity-70">From data problems to production systems.</p>
</div>

<div class="rounded-xl bg-blue-50 p-4">
<p class="font-bold text-blue-700">MSc Computer Science, 2024</p>
<p class="text-sm opacity-70">Concordia University.</p>
</div>

<div class="rounded-xl bg-slate-900 text-white p-4">
<p class="text-sm uppercase tracking-widest text-blue-200 mb-2">Example Project</p>
<p class="font-bold">AI email automation for loan commitments</p>
<p class="text-sm opacity-80 mt-2">Helped convert millions of dollars in loans that may have otherwise been lost.</p>
</div>

</div>

</div>

</div>

---

# Agenda

<div class="mt-8 grid gap-5">

<div class="rounded-xl border border-blue-100 bg-blue-50 p-5">
<p class="text-sm font-bold uppercase tracking-widest text-blue-700">Part 1</p>
<p class="mt-2 text-2xl font-bold">Install the prerequisite tools</p>
<p class="mt-2 text-lg opacity-75">Understand what each tool is used for before we start coding.</p>
</div>

<div class="rounded-xl border border-slate-200 bg-slate-900 p-5 text-white">
<p class="text-sm font-bold uppercase tracking-widest text-blue-200">Part 2</p>
<p class="mt-2 text-2xl font-bold">Build a data analysis dashboard</p>
<p class="mt-2 text-lg opacity-80">Use opencode to inspect data, write code, create charts, and verify changes.</p>
</div>

</div>

---

# Prerequisite Tools

Before we build anything, we need a reliable coding environment.

<div class="mt-6 grid grid-cols-2 gap-x-8 gap-y-3 text-left text-lg">

<div><strong>Windows Terminal</strong><br><span class="opacity-70">Run command-line tools.</span></div>
<div><strong>WSL with Ubuntu</strong><br><span class="opacity-70">Use Linux on Windows.</span></div>

<div><strong>VS Code</strong><br><span class="opacity-70">Edit and review code.</span></div>
<div><strong>VS Code WSL extension</strong><br><span class="opacity-70">Connect VS Code to Ubuntu.</span></div>

<div><strong>Git</strong><br><span class="opacity-70">Track project changes.</span></div>
<div><strong>Node.js and npm</strong><br><span class="opacity-70">Install JavaScript tools.</span></div>

<div><strong>uv</strong><br><span class="opacity-70">Manage Python packages.</span></div>
<div><strong>Docker Desktop</strong><br><span class="opacity-70">Run containerized software.</span></div>

<div><strong>opencode</strong><br><span class="opacity-70">Use an AI coding assistant.</span></div>
<div><strong>OpenRouter</strong><br><span class="opacity-70">Connect opencode to AI models.</span></div>

<div><strong>GitHub</strong><br><span class="opacity-70">Store and share repositories.</span></div>

</div>

---

# Windows Terminal

Windows Terminal is the command center for the workshop.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">It lets you open PowerShell and Ubuntu tabs in one clean app.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">We will run setup commands and open the Ubuntu terminal from here.</p>
</div>

</div>

---

# WSL With Ubuntu

WSL gives Windows a Linux development environment.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">Most coding tutorials, AI tools, and data tools work smoothly in Linux.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">Run workshop commands inside Ubuntu unless the guide says Windows.</p>
</div>

</div>

---

# VS Code

VS Code is where we read, edit, and review code.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">It makes project files, terminal output, and code changes visible in one place.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">We will inspect files, run commands, and review AI-generated changes.</p>
</div>

</div>

---

# VS Code WSL Extension

The WSL extension connects VS Code to Ubuntu.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">It prevents confusion between Windows files and Linux files.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">Look for <code class="rounded bg-blue-100 px-2 py-1 text-blue-900">WSL: Ubuntu</code> in VS Code before coding.</p>
</div>

</div>

---

# Git

Git tracks changes in a project.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">It helps you see what changed and recover when an edit goes wrong.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">We will clone the workshop repo and review diffs after AI edits.</p>
</div>

</div>

---

# Node.js And npm

Node.js runs JavaScript tools. npm installs them.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">Many developer tools are distributed through npm.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">We use npm to install opencode and check that it runs.</p>
</div>

</div>

---

# uv

uv is a fast Python package and project tool.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">It makes Python setup faster and more repeatable.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">It can manage the Python tools for our data dashboard project.</p>
</div>

</div>

---

# Docker Desktop

Docker runs software in containers.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">It helps projects run the same way on different machines.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">It may not be needed for the first dashboard, but it is common in real projects.</p>
</div>

</div>

---

# opencode

opencode is the AI coding assistant we will use from the terminal.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">It can inspect files, answer questions, and make code changes with your approval.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">We will ask it to build a small dashboard one step at a time.</p>
</div>

</div>

---

# OpenRouter Account And API Key

OpenRouter connects opencode to AI models.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">It gives opencode access to models from different providers.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">Create an API key, connect it in opencode, and keep the key private.</p>
</div>

</div>

---

# GitHub Account

GitHub stores Git repositories online.

<div class="mt-8 grid grid-cols-2 gap-5 text-left">

<div class="rounded-xl bg-blue-50 p-5">
<p class="font-bold text-blue-700">Why it matters</p>
<p class="mt-2">It lets you save projects, share code, and collaborate with others.</p>
</div>

<div class="rounded-xl bg-slate-900 p-5 text-white">
<p class="font-bold text-blue-200">How we use it</p>
<p class="mt-2 opacity-80">Use it to clone repositories and connect your local work to remote projects.</p>
</div>

</div>

---

# Next: Windows Setup Guide

We will now walk through <code>docs/windows-setup.md</code> quickly.

<div class="mt-8 rounded-xl bg-blue-50 p-6 text-left">

<p class="font-bold text-blue-700">Focus on the final checks:</p>

<pre class="mt-4 rounded-lg bg-slate-900 p-4 text-white"><code>git --version
node --version
npm --version
uv --version
docker --version
opencode --version
code --version</code></pre>

</div>
