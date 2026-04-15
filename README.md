# Claude for Delphi

A list of tools, libraries, MCP servers, and resources for using Claude Code with Delphi.

**Focus:** 
Open-source and actively maintained projects. 


---

## Contents

- [MCP Servers](#mcp-servers)
- [IDE Integration](#ide-integration)
- [Skills, Agents & Plugins](#skills-agents--plugins)
- [Anthropic / Claude API Wrappers](#anthropic--claude-api-wrappers)
- [OpenAI API Wrappers](#openai-api-wrappers)
- [Google Gemini API Wrappers](#google-gemini-api-wrappers)
- [AI Frameworks (Delphi-native)](#ai-frameworks-delphi-native)
- [Local / Offline LLMs](#local--offline-llms)
- [Community](#community)
- [Commercial Tools](#commercial-tools)



---

## MCP Servers

*MCP (Model Context Protocol) servers let Claude Code and Claude Desktop interact with Delphi tooling directly.*

* [Delphi-MCP-Server](https://github.com/GDKsoftware/Delphi-MCP-Server). 
`[Delphi]` `[Claude Code]` `[Claude Desktop]` Pure Delphi implementation of an MCP server. Listens on localhost:3000/mcp. Integrates with Claude Desktop, VS Code, Cursor, and Claude Code.

* [Delphi-LSP-MCP-Server](https://github.com/SkybuckFlying/Delphi-LSP-MCP-Server). 
`[Delphi]` `[MCP]` Routes MCP calls to Embarcadero's `DelphiLSP.exe` for live code intelligence (go-to-definition, find references, symbol search). Requires valid Delphi license.


---

## IDE Integration

*AI assistance built into or plugged into RAD Studio / Delphi IDE.*

* [RAD Studio 13 Smart CodeInsight — Claude Patch](https://blogs.embarcadero.com/rad-studio-13-smart-codeinsight-claude-patch-released/). `[RAD Studio 13]` Official Embarcadero patch adding Claude-powered code completion and suggestions via GetIt package manager. // *Built-in; no extra install beyond GetIt.*

* [Delphi AI Developer](https://github.com/Code4Delphi/Delphi-AI-Developer). `[Delphi]` Open-source RAD Studio IDE plugin. Chat, code generation, and refactoring directly inside the IDE. Supports OpenAI, Gemini, Groq, Ollama.


---

## Skills, Agents & Plugins

*Claude Code skills, agents, and standalone tools that enhance the Delphi + Claude workflow.*

* [ClaudeCode TokenVampire](https://github.com/GabrielOnDelphi/ClaudeCode_TokenVampire). `[Claude Code]` `[Windows]` Real-time token consumption monitor for Claude Code's 5-hour rolling window. Offline tray app showing per-hour bar charts (color-coded), cache hit rates, cost estimates, and cache-tier expiration countdowns. Zero API calls — reads local usage logs only. License: MPL-2.0.


---

## Anthropic / Claude API Wrappers

*Libraries for calling the Claude / Anthropic API directly from Delphi code.*

* [DelphiAnthropic](https://github.com/MaxiDonkey/DelphiAnthropic). `[Delphi]` Comprehensive Anthropic SDK for Delphi. Supports: all Claude models, vision, prompt caching, batch processing, tool use, MCP connector, streaming. Also on [Embarcadero GetIt](https://getitnow.embarcadero.com/anthropic-api-wrapper-for-delphi/).


---

## OpenAI API Wrappers

*Libraries for calling OpenAI-compatible APIs from Delphi.*

* [DelphiOpenAI](https://github.com/HemulGM/DelphiOpenAI). `[Delphi]` Most feature-complete OpenAI wrapper for Delphi. ChatGPT, DALL-E, Whisper, embeddings, functions. Also supports DeepSeek, Azure OpenAI, YandexGPT, Ollama, GigaChat, Qwen via compatible endpoints.

* [openai-delphi](https://github.com/landgraf-dev/openai-delphi). `[Delphi]` `[FPC]` OpenAI client for Delphi and Lazarus. ChatGPT, DALL-E. Cleaner API surface, good Lazarus compat.


---

## Google Gemini API Wrappers

*Libraries for calling the Google Gemini API from Delphi.*

* [DelphiGemini](https://github.com/MaxiDonkey/DelphiGemini). `[Delphi]` Google Gemini SDK for Delphi by MaxiDonkey. Supports chat, embeddings, code generation, vision, video/audio prompting, fine-tuning, caching. Also on [Embarcadero GetIt](https://getitnow.embarcadero.com/gemini-api-wrapper-for-delphi/).

* [Gemini4Delphi](https://github.com/delmardelima/Gemini4Delphi). `[Delphi]` Lightweight Gemini bridge for Delphi.


---

## AI Frameworks (Delphi-native)

*Full AI application frameworks written in or targeting Delphi.*

* [MakerAI](https://github.com/gustavoeenriquez/MakerAi). `[Delphi]` `[FPC]` 100% native Delphi AI framework. Features: RAG 2.0, autonomous agents, semantic memory, visual workflow builder. Multi-provider: Claude, OpenAI, Gemini, Ollama, Mistral. Also on [Embarcadero GetIt](https://getitnow.embarcadero.com/makerai-universal-llm-connector-for-delphi/).

* [LlamaKit](https://github.com/gustavoeenriquez/LlamaKit). `[Delphi]` Local LLM inference via llama.cpp GGUF models. Compiled Windows DLLs + Delphi wrappers. Zero network, no API keys. By the MakerAI author.


---

## Local / Offline LLMs

*Run LLMs locally from Delphi — no cloud, no API keys.*

* [Dllama](https://github.com/tinyBigGAMES/Dllama). `[Delphi]` LLM inference in Delphi via llama.cpp. Supports Ollama-compatible GGUF models (Llama, Mistral, Gemma, etc.).


---

## Community

* [Delphi-PRAXiS — AI & Claude discussions](https://en.delphipraxis.net/). Community forum. Search "Claude" or "AI" for ongoing threads on integrating LLMs into Delphi development.


---

## Commercial Tools

*Paid or source-available products. Clearly marked.*

* [TMS AI Studio](https://www.tmssoftware.com/site/tmsaistudio.asp). `[Delphi]` `[FPC]` `[Commercial]` Component suite for building AI-powered Delphi applications. Includes `TTMSMCPServer` class for creating MCP servers in Delphi, plus LLM connectors for Claude, OpenAI, Gemini, Ollama.

* [Claude Code Training for Delphi Developers](https://training.gdksoftware.com/). `[Claude Code]` `[Commercial]` Dedicated training by GDK Software. Covers CLAUDE.md setup, MCP integration, and Delphi-specific Claude Code workflows.

---

## Contributing

PRs welcome. Criteria:
- Must be AI-related AND Delphi/Pascal relevant
- Open-source highly preferred; commercial tools listed if uniquely valuable. Needs to clearly state so!!
- Dead projects (2+ years no updates) excluded unless irreplaceable
