<p align="center">
  <img src="assets/logo-full.png" alt="TeliTask" width="280" />
</p>

<p align="center">AI-powered phone calls, task management, and contact organization</p>

<p align="center">
  <a href="https://telitask.io">Website</a> ·
  <a href="#mcp-server">MCP Server</a> ·
  <a href="https://github.com/Telitask/telitask-ai/issues">Report Bug</a> ·
  <a href="https://github.com/Telitask/telitask-ai/discussions">Discussions</a>
</p>

---

## Features

- **AI Voice Calls** — Make and receive phone calls with AI-generated transcripts and summaries
- **Contact Management** — Organize and manage your contacts
- **Task Tracking** — Create, assign, and track tasks
- **MCP Server** — Integrate with Claude Desktop, Claude Code, and Cursor

## MCP Server

The [`@telitask/mcp-server`](https://www.npmjs.com/package/@telitask/mcp-server) package lets you manage contacts, tasks, and calls directly from your AI assistant.

### Quick Start

1. **Authenticate:**

   ```bash
   npx @telitask/mcp-server login
   ```

2. **Add to your MCP config** (Claude Desktop, Claude Code, or Cursor):

   ```json
   {
     "mcpServers": {
       "telitask": {
         "command": "npx",
         "args": ["-y", "@telitask/mcp-server"]
       }
     }
   }
   ```

### Available Tools

| Tool | Description |
|------|-------------|
| `call_me` | Request a call to your phone |
| `make_call` | Make a call to a contact |
| `schedule_call` | Schedule a call for later |
| `cancel_call` | Cancel a scheduled call |
| `list_calls` | List call history |
| `get_call` | Get call details with transcript |
| `list_contacts` | List your contacts |
| `create_contact` | Create a new contact |
| `list_tasks` | List your tasks |
| `create_task` | Create a new task |
| `update_task` | Update an existing task |

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for release history.

## License

© 2026 Telitask. All rights reserved.
