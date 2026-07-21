# ⭐ Subscribe My Channel: **CodeVerse Soban**

------------------------------------------------------------------------

# OmniRoute + Claude Code Installation Guide

## Step 1 --- Install Node.js

Download and install the **LTS** version:

https://nodejs.org

Check that Node.js is installed:

``` bash
node -v
```

------------------------------------------------------------------------

## Step 2 --- Install OmniRoute

``` bash
npm install -g omniroute
omniroute
```

Now open your browser:

http://localhost:20128

------------------------------------------------------------------------

## Step 3 --- Connect a Free Provider

1.  Open the OmniRoute Dashboard.
2.  Go to **Providers**.
3.  Turn **ON** any available **Free Provider**.

------------------------------------------------------------------------

## Step 4 --- Install Claude Code

``` bash
npm install -g @anthropic-ai/claude-code
```

------------------------------------------------------------------------

# Step 5 --- Run Claude Code

## 🪟 Windows (PowerShell)

``` powershell
$env:CLAUDE_CONFIG_DIR="$HOME\.claude-omniroute"
$env:ANTHROPIC_BASE_URL="http://localhost:20128"
$env:ANTHROPIC_AUTH_TOKEN="PASTE-YOUR-OMNIROUTE-KEY-HERE"
$env:ANTHROPIC_API_KEY=""
$env:ANTHROPIC_MODEL="PASTE-YOUR-MODEL-NAME-HERE"

claude
```

------------------------------------------------------------------------

## 🍎 macOS / 🐧 Linux

``` bash
export CLAUDE_CONFIG_DIR="$HOME/.claude-omniroute"
export ANTHROPIC_BASE_URL="http://localhost:20128"
export ANTHROPIC_AUTH_TOKEN="PASTE-YOUR-OMNIROUTE-KEY-HERE"
export ANTHROPIC_API_KEY=""
export ANTHROPIC_MODEL="PASTE-YOUR-MODEL-NAME-HERE"

claude
```
