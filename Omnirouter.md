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

## Step 5 — Configure Claude Code

1. Open your **User Folder**.
2. Go to the **.claude** folder.
3. Open the **settings.json** file in **Visual Studio Code**.
4. Replace the values below with your **OmniRoute API Key** and **Model Name**, then save the file.

> **Note:**
> - `ANTHROPIC_AUTH_TOKEN` = Your OmniRoute API Key
> - `ANTHROPIC_MODEL` = Your selected model (e.g. `oc/deepseek-v4-flash-free`)

```json
{
  "env": {
    "ANTHROPIC_BASE_URL": "http://localhost:20128",
    "ANTHROPIC_AUTH_TOKEN": "Your_Key",
    "ANTHROPIC_API_KEY": "",
    "ANTHROPIC_MODEL":"Model_name"
  }
}
```

5. Save the file.
6. Restart **Claude Code**.

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
