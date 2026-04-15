# Claude for Delphi

A list of tools, libraries, MCP servers, and resources for using Claude Code with Delphi.

**Focus:** 
Open-source and actively maintained projects. 


---

## Contents

- [MCP Servers](#mcp-servers)
- [IDE Integration](#ide-integration)
- [Anthropic API Wrappers](#anthropic-api-wrappers)
- [AI Frameworks (Delphi-native)](#ai-frameworks-delphi-native)
- [Claude Code Setup for Delphi](#claude-code-setup-for-delphi)
- [Training & Community](#training--community)
- [Commercial Tools](#commercial-tools)



---

## MCP Servers

*MCP (Model Context Protocol) servers let Claude Code and Claude Desktop interact with Delphi tooling directly.*

* [Delphi-MCP-Server](https://github.com/GDKsoftware/Delphi-MCP-Server). `[Delphi]` `[Claude Code]` `[Claude Desktop]` Pure Delphi implementation of an MCP server. Listens on localhost:3000/mcp. Integrates with Claude Desktop, VS Code, Cursor, and Claude Code.

* [Delphi-LSP-MCP-Server](https://github.com/SkybuckFlying/Delphi-LSP-MCP-Server). `[Delphi]` `[MCP]` Routes MCP calls to Embarcadero's `DelphiLSP.exe` for live code intelligence (go-to-definition, find references, symbol search). Requires valid Delphi license.


---

## IDE Integration

*AI assistance built into or plugged into RAD Studio / Delphi IDE.*

* [RAD Studio 13 Smart CodeInsight — Claude Patch](https://blogs.embarcadero.com/rad-studio-13-smart-codeinsight-claude-patch-released/). `[RAD Studio 13]` Official Embarcadero patch adding Claude-powered code completion and suggestions via GetIt package manager. // *Built-in; no extra install beyond GetIt.*


---

## Anthropic API Wrappers

*Libraries for calling the Claude / Anthropic API directly from Delphi code.*

* [DelphiAnthropic](https://github.com/MaxiDonkey/DelphiAnthropic). `[Delphi]` Unofficial but comprehensive Anthropic SDK for Delphi. Supports: all Claude models, vision, prompt caching, batch processing, tool use, MCP connector, streaming. Also available on [Embarcadero GetIt](https://getitnow.embarcadero.com/anthropic-api-wrapper-for-delphi/).


---

## AI Frameworks (Delphi-native)

*Full AI application frameworks written in or targeting Delphi.*

* [MakerAI](https://github.com/gustavoeenriquez/MakerAi). `[Delphi]` `[FPC]` 100% native Delphi AI framework. Features: RAG 2.0, autonomous agents, semantic memory, visual workflow builder. Multi-provider: Claude, OpenAI, Gemini, Ollama, Mistral.



---

## Skills, Agents & Plugins


---

## Community

* [Delphi-PRAXiS — AI & Claude discussions](https://en.delphipraxis.net/). Community forum. Search "Claude" or "AI" for ongoing threads on integrating LLMs into Delphi development.


---

## Commercial Tools

* [TMS AI Studio](https://www.tmssoftware.com/site/tmsaistudio.asp). `[Delphi]` `[FPC]` `[Commercial]` Component suite for building AI-powered Delphi applications. Includes `TTMSMCPServer` class for creating MCP servers in Delphi, plus LLM connectors for Claude, OpenAI, Gemini, Ollama.

* [Claude Code Training for Delphi Developers](https://training.gdksoftware.com/). `[Claude Code]` Dedicated training by GDK Software. Covers CLAUDE.md setup, MCP integration, and Delphi-specific Claude Code workflows.

---

## Contributing

PRs welcome. Criteria:
- Must be Claude / Anthropic AI related AND Delphi/Pascal relevant
- Open-source highly preferred; commercial tools listed if uniquely valuable. Needs to cleary state so!!
- Dead projects (2+ years no updates) excluded unless irreplaceable
