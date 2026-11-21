# Naffes for Claude

[Naffes](https://naffes.net) is a CRM: deals, contacts, companies, tasks, inbox and
reports. This connector lets Claude work in your Naffes workspace as you — it sees
what you may see, and nothing more.

- Connector URL: `https://api.naffes.net/api/mcp`
- Sign-in: OAuth. No key to copy.
- Support: hello@naffes.net · [Privacy](https://naffes.net/privacy) · [Terms](https://naffes.net/terms)

## Connect

**Claude (web, desktop, mobile)** — Settings → Connectors → Add custom connector,
paste `https://api.naffes.net/api/mcp`, then Connect.

**Claude Code** — install the plugin, which adds the connector and three skills:

```
/plugin marketplace add I3mal-Team/naffes-claude-plugin
/plugin install naffes@naffes
```

Then run `/mcp`, choose `naffes` and sign in.

Either way you land on one Naffes screen that names who is asking and which
workspace it is for. You choose there:

- **Read only** (the default) — Claude can look things up and report. It cannot
  change anything.
- **Read and change** — Claude can also create and edit records, tasks and
  settings, within your own permissions.

## What Claude can do

| Area | Examples |
| --- | --- |
| Find and read | Search contacts, companies and deals; open any record; read its history |
| Your day | Tasks due and overdue, meetings, deals closing this week |
| Pipeline | Totals by stage, stuck and at-risk deals, win/loss numbers |
| Team (managers) | Workload and activity per person |
| Change (if you allow it) | Create and update records, log notes, complete tasks, move a deal's stage, schedule meetings |
| Set up (admins, if you allow it) | Pipelines, fields, roles, reports, dashboards, workflows |

Every record Claude mentions comes with a link that opens it in Naffes.

## Try

- "What is on my plate today in Naffes?"
- "Which deals are at risk this week, and what should I do about each?"
- "Prepare me for my call with Acme — who are they, what is open, what did we last say?"
- "Add a task to call Nada Ali tomorrow at 10." (needs Read and change)
- "Move the Acme renewal to Negotiation and log a note that they asked for a discount." (needs Read and change)

With the plugin you also get `/naffes:brief`, `/naffes:pipeline-review` and
`/naffes:meeting-prep <name>`.

## Permissions and privacy

- Claude acts as the person who connected it, in the one workspace they approved.
  Their role and record-level permissions apply to every call.
- The connection opens the connector only. It cannot be used on the rest of the
  Naffes API.
- A read-only connection is refused every tool that changes data.
- Naffes does not receive your conversation — only the tool calls Claude makes.
- Disconnect any time in Naffes: Settings → API tokens → Connected agents. It
  stops at once.

## Troubleshooting

- **"Not available"** on a tool — your Naffes role does not allow it, or the
  connection is read only. Reconnect and choose Read and change.
- **Asked to sign in again** — the connection was disconnected in Naffes, or
  unused for a long time. Connect again.
- Anything else: hello@naffes.net
