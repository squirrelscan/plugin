# squirrelscan plugin

The website QA tool for your coding agent, in the cloud.

This plugin connects Claude to the hosted squirrelscan MCP server (`https://mcp.squirrelscan.com/mcp`). Your agent can audit any website for SEO, performance, security, accessibility, content, structured data and agent experience issues (350+ rules), read the report, compare one audit with the last, and fix what it finds in your code. Nothing to install: audits run in squirrelscan's cloud.

## Install

From the Claude plugin directory, or:

```
/plugin marketplace add squirrelscan/plugin
/plugin install squirrelscan@squirrelscan-cloud
```

The first tool call asks you to sign in to squirrelscan (OAuth). Audits spend credits from your squirrelscan organization; the server shows the estimate before a large audit starts.

## What you can ask

- "Audit https://example.com and fix the top issues in this repo"
- "What changed since the last audit of my site?"
- "Why is the accessibility score low, and which pages are affected?"
- "Turn off recurring audits for example.com"

## Tools

The server exposes audits (`run_audit`, `get_audit_status`, `get_report`, `compare_audits`), issues and findings, website settings and schedules, and rule docs. The full list and every parameter: [docs.squirrelscan.com/developers/mcp](https://docs.squirrelscan.com/developers/mcp).

## Using the CLI instead

For local audits with the `squirrel` CLI (localhost, CI, offline), use the agent skills at [squirrelscan/skills](https://github.com/squirrelscan/skills).

## Support

- Docs: [docs.squirrelscan.com](https://docs.squirrelscan.com)
- Support: [squirrelscan.com/support](https://squirrelscan.com/support)
- Privacy: [squirrelscan.com/privacy](https://squirrelscan.com/privacy)
- Terms: [squirrelscan.com/terms](https://squirrelscan.com/terms)

## License

MIT
