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


---

## MCP Servers

*MCP (Model Context Protocol) servers let Claude Code and Claude Desktop interact with Delphi tooling directly.*

* [Delphi-MCP-Server](https://github.com/GDKsoftware/Delphi-MCP-Server). `[Delphi]` `[Claude Code]` `[Claude Desktop]` Pure Delphi implementation of an MCP server. Listens on localhost:3000/mcp. Integrates with Claude Desktop, VS Code, Cursor, and Claude Code.

* [Delphi-LSP-MCP-Server](https://github.com/SkybuckFlying/Delphi-LSP-MCP-Server). `[Delphi]` `[MCP]` Routes MCP calls to Embarcadero's `DelphiLSP.exe` for live code intelligence (go-to-definition, find references, symbol search). Requires valid Delphi license.


---

## IDE Integration

*AI assistance built into or plugged into RAD Studio / Delphi IDE.*

* [RAD Studio 13 Smart CodeInsight — Claude Patch](https://blogs.embarcadero.com/rad-studio-13-smart-codeinsight-claude-patch-released/). `[RAD Studio 13]` Official Embarcadero patch adding Claude-powered code completion and suggestions via GetIt package manager. // *Built-in; no extra install beyond GetIt.*

* [TMS AI Studio](https://www.tmssoftware.com/site/tmsaistudio.asp). `[Delphi]` `[FPC]` Commercial component suite for building AI-powered Delphi applications. Includes `TTMSMCPServer` class for creating MCP servers in Delphi, plus LLM connectors for Claude, OpenAI, Gemini, Ollama.

---

## Anthropic API Wrappers

*Libraries for calling the Claude / Anthropic API directly from Delphi code.*

* [DelphiAnthropic](https://github.com/MaxiDonkey/DelphiAnthropic). `[Delphi]` Unofficial but comprehensive Anthropic SDK for Delphi. Supports: all Claude models, vision, prompt caching, batch processing, tool use, MCP connector, streaming. Also available on [Embarcadero GetIt](https://getitnow.embarcadero.com/anthropic-api-wrapper-for-delphi/).


---

## AI Frameworks (Delphi-native)

*Full AI application frameworks written in or targeting Delphi.*

* [MakerAI](https://github.com/gustavoeenriquez/MakerAi). `[Delphi]` `[FPC]` 100% native Delphi AI framework. Features: RAG 2.0, autonomous agents, semantic memory, visual workflow builder. Multi-provider: Claude, OpenAI, Gemini, Ollama, Mistral.


---

## Claude Code Setup for Delphi

*Configuration, CLAUDE.md patterns, and workflow guides specifically for Delphi projects.*

* [Using Claude Code with Delphi — Delphi-PRAXiS thread](https://en.delphipraxis.net/topic/14273-using-claude-code-with-delphi/). `[Claude Code]` Active community discussion covering CLAUDE.md setup, custom agents, build integration, and real-world workflows with Delphi projects.

### Recommended CLAUDE.md Conventions for Delphi Projects

Key things to document in your project's `CLAUDE.md`:

- **Build command** — absolute path to `Build.cmd` (bash `cd` doesn't affect `cmd.exe` CWD on Windows)
- **Delphi version target** — e.g., `Delphi 13.1, compat down to Rio`
- **Framework paths** — where LightSaber, VCL/FMX libs, 3rd-party packages live
- **Forbidden patterns** — `with`, `Application.ProcessMessages`, raw pointers, global vars
- **Test runner** — DUnitX + TestInsight, build command for tests
- **Custom agents** — `delphi-compiler` and `delphi-review` agent definitions

### Custom Agent: delphi-compiler

Wire a `delphi-compiler` sub-agent that calls `Build.cmd` and parses Delphi's compiler output. Lets Claude Code verify builds without killing the running process.

### Custom Agent: delphi-review

Wire a `delphi-review` sub-agent for code review of `.pas` files — checks for forbidden patterns, memory leaks, swallowed exceptions, and style compliance.


---

## Training & Community

* [Claude Code Training for Delphi Developers](https://training.gdksoftware.com/). `[Claude Code]` Dedicated training by GDK Software. Covers CLAUDE.md setup, MCP integration, and Delphi-specific Claude Code workflows.

* [Delphi-PRAXiS — AI & Claude discussions](https://en.delphipraxis.net/). Community forum. Search "Claude" or "AI" for ongoing threads on integrating LLMs into Delphi development.

---

## Contributing

PRs welcome. Criteria:
- Must be Claude / Anthropic AI related AND Delphi/Pascal relevant
- Open-source preferred; commercial tools listed if uniquely valuable. Needs to cleary state so!!
- Dead projects (3+ years no updates) excluded unless irreplaceable
