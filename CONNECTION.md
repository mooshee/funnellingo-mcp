# Connect to FunnelLingo

Start at [FunnelLingo](https://funnellingo.com) and add `https://api.funnellingo.com/agent/mcp` as a remote Streamable HTTP MCP server.

The server requires MCP `2026-07-28`. Check that your host supports this revision before connecting. A generated configuration does not verify host compatibility.

This revision uses `server/discover` and per-request protocol and client-capability metadata. It has no `initialize` handshake. The host must send matching protocol and method headers for HTTP requests.

Sign in through the server's OAuth connection flow and review the permissions requested by your host. The protected resource is `https://api.funnellingo.com`. Advertised scopes are `read`, `setup`, `draft`, `publish`. Request only the permissions needed for your task; tool availability follows the approved account and grant.

Use the server's live OAuth discovery metadata. Do not paste passwords, tokens, or authorization links into a prompt or commit them to configuration. Reconnect when the server requires new authorization. Publication and other consequential actions retain their separate product approvals.

Discover the current tools after connecting. A saved catalog describes the observed connection and may not include every tool available under another grant. Successful packaging does not establish a working host connection or a published listing.
