---
name: funnellingo
displayName: FunnelLingo
version: 0.2.0
author: Moosh Works LLC
description: Translate website pages
keywords:
  - website
  - translation
  - localization
  - mcp
mcpServers:
  funnellingo:
    type: streamable-http
    url: https://api.funnellingo.com/agent/mcp
---

# FunnelLingo Power (AWS Kiro)

Author: Moosh Works LLC

Translate website pages

## Quick start

1. Visit [FunnelLingo](https://funnellingo.com) or connect Kiro to `https://api.funnellingo.com/agent/mcp`.

## MCP Server Configuration

```json
{
  "mcpServers": {
    "funnellingo": {
      "type": "streamable-http",
      "url": "https://api.funnellingo.com/agent/mcp"
    }
  }
}
```

## Tools Available

- `agent_capabilities`
- `agent_create_operation`
- `agent_get_operation`
- `agent_list_events`
- `agent_resume_operation`
- `agent_cancel_operation`
- `agent_get_plan`
- `agent_release_evidence`
