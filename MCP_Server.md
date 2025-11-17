# Part 2: Connect GitHub MCP Server with Gemini CLI (Remote Server)

Learn how to securely connect the GitHub MCP Server to your Google Gemini CLI using a remote (hosted) server—no Docker required. This method is simple, quick, and designed for modern workflows.

---

## 🚀 Prerequisites

- Google Gemini CLI installed and configured  
- GitHub Personal Access Token (PAT)  
  - [Generate a new PAT here](https://github.com/settings/personal-access-tokens/new)  
  - Recommended scopes: `repo`, `read:packages` (optional for package access)

> **Security tip:** Never expose your PAT in screenshots or source code!

---

## 🔒 Step 1: Store Your PAT Securely

Create (or open) your user `.env` file:

```bash
mkdir -p ~/.gemini
nano ~/.gemini/.env
```

Add your token:

```env
GITHUB_MCP_PAT=your_token_here
```

This way, Gemini CLI will automatically load it from environment variables and your token remains secure.

---

## ⚙️ Step 2: Configure GitHub MCP Server

Edit (or create if missing) your settings file:

```bash
nano ~/.gemini/settings.json
```

Add the following configuration block (**do not hardcode your token directly!**):
```
{
  "mcpServers": {
    "github": {
      "httpUrl": "https://api.githubcopilot.com/mcp/",
      "headers": {
        "Authorization": "Bearer $GITHUB_MCP_PAT"
      }
    }
  }
}
```

**How this works:**

- **httpUrl** tells Gemini CLI where to reach the hosted GitHub MCP server.  
- **headers.Authorization** pulls your PAT securely from the env variable.

---

## 🔄 Step 3: Restart Gemini CLI

Apply your configuration:

```bash
gemini
```

---

## ✅ Step 4: Verify the Connection

List the available MCP servers:

```bash
/mcp list
```

You should see:

```
🟢 github - Ready (90+ tools)
```

If you see this, congratulations—your MCP server is ready!

---

## 🧪 Step 5: Test the MCP Server

Try a natural language command, e.g.:

```bash
List my GitHub repositories
```

If your repos appear, everything is working perfectly. Enjoy multi-tool integration!

---
**Need advanced automation, code reviews, or multi-repo queries?**  
Stay tuned for **Day 3: Harnessing MCP Tools for Real-World Projects!**
