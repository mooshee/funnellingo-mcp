# FunnelLingo

Translate website pages, review changes, and publish approved wording from your
agent. FunnelLingo preserves page structure and protected names and leaves
visitor-entered form values out of translation.

[Website](https://funnellingo.com) · [Account](https://app.funnellingo.com/account)
· [Support](https://funnellingo.com/support)

## Connect

1. [Open FunnelLingo](https://funnellingo.com/agents) in the business account
   where it is installed. This remote connection requires an active installation
   and administrator access. Review the plan and price before subscribing.
2. Add `https://api.funnellingo.com/agent/mcp` as an OAuth MCP connection in a host
   that supports MCP `2026-07-28` and HTTPS Client ID Metadata Documents.
3. In **Settings → Agent access**, review the requested website and permissions.
   Start with read access when you only need an inspection. Drafting, setup and
   publishing need the corresponding permissions.
4. Ask the agent to inspect the connected website before making changes.

The remote connection uses short-lived authorization. Reconnect when it expires;
do not paste account passwords or access tokens into chat. Compatibility depends
on the host's protocol and callback support. A generated configuration does not
establish that a host has passed a connection test.

Standalone customers can use the separate local account adapter described in
[FunnelLingo's developer guide](https://app.funnellingo.com/developers). It keeps
credentials in the customer's private local store. This package does not
include that adapter.

## Work with translations

The agent can inspect the permissions available to the connection, review source
phrases and translation status, prepare updates, and follow saved operations.
Only tools authorized for that connection appear in its current catalog.

The catalog included with this package was observed with read-only access. To
draft translations, set up a website, or publish an approved plan, reconnect and
explicitly select the permissions needed for that task. Refresh the tool catalog
after reconnecting.

Human-approved wording stays locked. Review a proposed release before approving
its exact plan. A queued job or successful tool response does not prove that the
translated page is publicly available: check the saved delivery evidence and the
actual page. Hosted translations and search indexing have separate requirements;
this plugin does not grant permission to enable indexing.

## Privacy and payment

Use published website text, not visitor entries or contact records. Do not send
payment-card details, mailbox codes, account passwords, or provider credentials
through tool arguments. Paid plans and any optional extra usage are governed by
the terms shown in FunnelLingo. The connection does not approve purchases or
increase a spending limit.

Read the [Privacy Policy](https://funnellingo.com/privacy) and
[Terms](https://funnellingo.com/terms).

## Version

The integration package is version `0.2.0`. Its version is separate from the
hosted product and Marketplace app versions. See [release notes](CHANGELOG.md).

## License

The consumer skills, documentation and connector configurations use the
[MIT-0 license](LICENSE). Brand assets have their
[own notice](https://github.com/mooshee/funnellingo-mcp/blob/v0.2.0/assets/LICENSE).
The private application and existing account adapters are not included or
relicensed by this package.


---

Built and maintained by **[Moosh Works](https://mooshworks.com)** ([https://mooshworks.com](https://mooshworks.com)).
