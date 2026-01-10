# Hipp AI Development Guide

## 1. Local Development (Website)
To work on the website (`hipp-ai-website`):

### Start the Local Server
Run this command in your terminal:
```bash
python3 -m http.server 8000
```
Then open: [http://localhost:8000](http://localhost:8000)

### Making Changes
1.  Edit `index.html`, `styles.css`, or `script.js`.
2.  Refresh the browser to see changes.

## 2. Deployment (Vercel)
To push your changes to the live internet:

### Option A: Automatic (Recommended)
Simply commit and push to GitHub. Vercel will automatically deploy.
```bash
git add .
git commit -m "Describe your change"
git push
```

### Option B: Manual CLI (Advanced)
*Note: You encountered SSL errors with this. We recommend Option A.*
If you need to use the CLI, try running:
```bash
NODE_TLS_REJECT_UNAUTHORIZED=0 vercel login
```
But for day-to-day work, just use **git push**.

## 3. n8n & MCP Tools
Your n8n tools are configured in `~/Projects`.

- **hipp-ai-n8n**: Your workflow backups.
- **n8n-skills**: The "brain" for building workflows.
- **Config**: `.mcp.json` is located in `~/Projects/hipp-ai-website/.mcp.json`.

### How to use n8n Skills
When you want to build a workflow, you can ask for help like:
> "Help me build a lead qualification workflow using the n8n skills."

### Security
- **API Key**: If you ever need to change your n8n key, edit `.mcp.json`.
