# PatentReply

**The USPTO prosecution record for your AI.**

PatentReply compiles a U.S. patent application's public file wrapper into a
working record your AI assistant can use: every claim version on the legal
date it took effect, each office action with its rejections and objections,
the cited references, and the specification. Ask it to review the pending
office action and it sets each rejection against the exact passage the
examiner relied on, with a verification address into the stored record for
every quote. Current law comes from the MPEP live, never recited from memory.

The response is built in stages the attorney controls. Drafting stays locked
until a registered practitioner approves the response plan on the PatentReply
approval page; a confirmation inside the chat is never sign-off. After
approval, PatentReply generates the 37 CFR 1.121 claim listing and the
filing-ready response document on the server.

## Connect

One hosted MCP server, OAuth sign-in, no API keys:

```
https://mcp.patentreply.ai/mcp/v2
```

- **Claude** (web, desktop, mobile): Settings → Connectors → Add custom connector
- **Claude Code**: `claude mcp add --transport http patentreply https://mcp.patentreply.ai/mcp/v2`
- **Cursor, ChatGPT, any MCP client**: see [patentreply/patentreply-mcp](https://github.com/patentreply/patentreply-mcp)

Full guide: [patentreply.ai/connect](https://www.patentreply.ai/connect)

## Repositories

- [patentreply-mcp](https://github.com/patentreply/patentreply-mcp): the connector card, registry metadata, and the Claude plugin with the office-action methodology and `/oa`, `/respond`, `/interview`, `/status` commands.

The PatentReply service is hosted by Patent Agentic LLC and is not open
source. Public USPTO records and current MPEP text are ingested server-side
for the applications you name; PatentReply receives only the arguments of
the tools your AI calls and never reads conversation history, memory, or
files on your machine.

## Links

[Website](https://www.patentreply.ai) · [Documentation](https://www.patentreply.ai/documentation) · [Pricing](https://www.patentreply.ai/pricing) · [Privacy](https://www.patentreply.ai/privacy) · [Security](https://www.patentreply.ai/security) · [Terms](https://www.patentreply.ai/terms)

Support: info@patentreply.ai

*PatentReply is software, not a law firm. The registered practitioner remains responsible for every filing.*
