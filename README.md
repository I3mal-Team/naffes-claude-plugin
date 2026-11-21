# Naffes for Claude

Work in your Naffes CRM from Claude: your day, your pipeline, your customers.

## Install (Claude Code)

```
/plugin marketplace add I3mal-Team/naffes-claude-plugin
/plugin install naffes@naffes
```

Then run `/mcp`, choose `naffes` and sign in. You approve one screen in Naffes; the
connection reads your CRM as you, and changes nothing unless you switch that on.

In the Claude app: Customize → Plugins → add this repository, then connect Naffes
from the plugin's Connectors tab.

## What you get

| Command | What it does |
| --- | --- |
| `/naffes:brief` | Your day: overdue, due today, closing this week, at risk |
| `/naffes:pipeline-review` | The pipeline by stage, what is stuck, what to do next |
| `/naffes:meeting-prep <name>` | One page on a customer before you meet them |

You can also just ask — "what is on my plate today?", "prepare me for my call with …".

Disconnect any time in Naffes: Settings → API tokens → Connected agents.
