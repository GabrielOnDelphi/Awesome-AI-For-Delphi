# Awesome AI for Delphi

A list of tools, libraries, MCP servers, and resources for using Claude Code with Delphi.

**Focus:** 
Open-source and actively maintained projects. Commercial tools are listed separately and clearly marked.

---

## Contents

- [Apps](#apps)
- [MCP Servers](#mcp-servers)
- [IDE Integration](#ide-integration)
- [Skills, Agents & Plugins](#skills-agents--plugins)
- [Cloud LLM API Wrappers](#cloud-llm-api-wrappers)
  - [Anthropic / Claude](#anthropic--claude)
  - [OpenAI](#openai)
  - [Google Gemini](#google-gemini)
  - [Mistral](#mistral)
  - [Groq](#groq)
  - [DeepSeek](#deepseek)
  - [Hugging Face](#hugging-face)
  - [Stability AI / Image Generation](#stability-ai--image-generation)
- [AI Frameworks (Delphi-native)](#ai-frameworks-delphi-native)
- [Local / Offline LLMs](#local--offline-llms)
- [Machine Learning & Neural Networks](#machine-learning--neural-networks)
- [ONNX & Model Inference](#onnx--model-inference)
- [Image Generation](#image-generation)
- [Community](#community)
- [Commercial Tools](#commercial-tools)


---

## MCP Servers

*MCP (Model Context Protocol) servers let Claude Code and Claude Desktop interact with Delphi tooling directly.*

* [Delphi-MCP-Server](https://github.com/GDKsoftware/Delphi-MCP-Server).  
Pure Delphi implementation. Listens on localhost:3000/mcp. Integrates with Claude Desktop, VS Code, Cursor, and Claude Code.  
`[Claude Code]` `[Claude Desktop]`

* [Delphi-LSP-MCP-Server](https://github.com/SkybuckFlying/Delphi-LSP-MCP-Server).  
Routes MCP calls to Embarcadero's `DelphiLSP.exe` for live code intelligence: go-to-definition, find references, symbol search. Requires valid Delphi license.  

---

## IDE Integration

*AI assistance built into or plugged into RAD Studio / Delphi IDE.*

* [RAD Studio 13 Smart CodeInsight — Claude Patch](https://blogs.embarcadero.com/rad-studio-13-smart-codeinsight-claude-patch-released/).  
Official Embarcadero GetIt patch adding Claude-powered code completion.  
`[RAD Studio 13]`

* [Delphi AI Developer](https://github.com/Code4Delphi/Delphi-AI-Developer).  
Open-source RAD Studio IDE plugin. Chat, code generation, and refactoring directly inside the IDE. Multi-provider: OpenAI, Gemini, Groq, Ollama.  

---

## Skills, Agents & Plugins

*Claude Code skills, agents, and standalone tools that enhance the Delphi + AI workflow.*

* [ClaudeCode TokenVampire](https://github.com/GabrielOnDelphi/ClaudeCode_TokenVampire).  
Real-time token consumption monitor for Claude Code's 5-hour rolling window. Offline tray app: per-hour bar charts (color-coded), cache hit rates, cost estimates, cache-tier expiration countdowns. Zero API calls — reads local usage logs only. Freeware.  
`[Claude Code]`

---

## Apps

*Standalone AI applications built in Delphi.*

* [ChatGPT (HemulGM)](https://github.com/HemulGM/ChatGPT).  
Native ChatGPT client built in Delphi. Cross-platform: Windows, Mac, Android, iOS, Linux.  
`[FMX]`

---

## Cloud LLM API Wrappers

*Libraries for calling cloud AI APIs directly from Delphi. MaxiDonkey maintains a comprehensive family of wrappers covering most major providers.*

### Anthropic / Claude

* [DelphiAnthropic](https://github.com/MaxiDonkey/DelphiAnthropic).  
Full Anthropic SDK. All Claude models, vision, prompt caching, batch processing, tool use, MCP connector, streaming. 

### OpenAI

* [DelphiOpenAI](https://github.com/HemulGM/DelphiOpenAI).  
Most feature-complete OpenAI wrapper. ChatGPT, DALL-E, Whisper, embeddings, functions. Also supports DeepSeek, Azure OpenAI, YandexGPT, Ollama, GigaChat, Qwen via compatible endpoints.  

* [DelphiGenAI](https://github.com/MaxiDonkey/DelphiGenAI).  
MaxiDonkey's OpenAI wrapper. Covers GPT-5 series, vision, audio, SORA video generation, embeddings, and agentic workflows.  

* [openai-delphi](https://github.com/landgraf-dev/openai-delphi).  
OpenAI client for Delphi and Lazarus. Clean API surface, good Lazarus compat.  
`[Lazarus]`

### Google Gemini

* [DelphiGemini](https://github.com/MaxiDonkey/DelphiGemini).  
Google Gemini SDK. Chat, embeddings, code generation, vision, video/audio prompting, fine-tuning, caching.

* [Gemini4Delphi](https://github.com/delmardelima/Gemini4Delphi).  
Lightweight Gemini bridge.  

### Mistral

* [DelphiMistralAI](https://github.com/MaxiDonkey/DelphiMistralAI).  
Mistral text, vision, and audio models. Agentic conversations, embeddings, Codestral code generation, fine-tuning, batching, moderation.  

### Groq

* [DelphiGroqCloud](https://github.com/MaxiDonkey/DelphiGroqCloud).  
Groq LPU cloud API wrapper. Runs Meta, OpenAI, Mistral, and Google models at inference speeds. Chat, image analysis, audio transcription, tool use.  

### DeepSeek

* [DelphiDeepseek](https://github.com/MaxiDonkey/DelphiDeepseek).  
DeepSeek reasoning model wrapper. Also supports local LM Studio server.  

### Hugging Face

* [DelphiHuggingFace](https://github.com/MaxiDonkey/DelphiHuggingFace).  
Hugging Face Inference API. Object detection, text classification, sentiment analysis, image segmentation, speech-to-text, music generation.  

### Stability AI / Image Generation

* [DelphiStabilityAI](https://github.com/MaxiDonkey/DelphiStabilityAI).  
Stability.ai wrapper. Image generation, video generation, 3D generation, editing, and upscaling.  

---

## AI Frameworks (Delphi-native)

*Full AI application frameworks written in or targeting Delphi.*

* [MakerAI](https://github.com/gustavoeenriquez/MakerAi).  
Native Delphi AI framework. RAG 2.0, autonomous agents, semantic memory, visual workflow builder. Multi-provider: Claude, OpenAI, Gemini, Ollama, Mistral. 
`[FPC]`

* [LlamaKit](https://github.com/gustavoeenriquez/LlamaKit).  
Local LLM inference via llama.cpp GGUF models. Compiled Windows DLLs + Delphi wrappers. Zero network, no API keys. By the MakerAI author.  

---

## Local / Offline LLMs

*Run LLMs locally from Delphi — no cloud, no API keys.*

* [llama-cpp-delphi](https://github.com/Embarcadero/llama-cpp-delphi).  
Official Embarcadero llama.cpp binding. Run GGUF models locally.  

* [Dllama](https://github.com/tinyBigGAMES/Dllama).  
LLM inference via llama.cpp. Supports Ollama-compatible GGUF models: Llama, Mistral, Gemma, etc.  

---

## Machine Learning & Neural Networks

*Classical ML, neural networks, and training frameworks — not LLM-based.*

* [TensorFlow.Delphi](https://github.com/Pigrecos/TensorFlow.Delphi).  
Complete TensorFlow API binding. Build, train, and deploy ML models without leaving Pascal.  

* [TONNXRuntime](https://github.com/hshatti/TONNXRuntime).  
Microsoft ONNX Runtime bindings for FreePascal and Delphi. Run pre-trained ONNX models (classification, detection, NLP, etc.).  
`[Lazarus]`

---

## ONNX & Model Inference

*Run trained models locally via ONNX or other runtimes.*

* [Delphi-YOLO-ONNX-RuntimeWrapper](https://github.com/SoftacomCompany/Delphi-YOLO-ONNX-RuntimeWrapper).  
YOLO object detection via ONNX Runtime. Real-time bounding boxes on images and video.   

---

## Image Generation

*Stable Diffusion and generative image tools.*

* [DelphiStabilityAI](https://github.com/MaxiDonkey/DelphiStabilityAI).  
Stability.ai wrapper. Image generation, video generation, 3D generation, editing, and upscaling. (See [Stability AI / Image Generation](#stability-ai--image-generation) above for details.)  

* [DALL-E (HemulGM)](https://github.com/HemulGM/DALL-E).  
DALL-E image generation client for Delphi.  

* [Stable-Diffusion-Desktop-Client](https://github.com/FMXExpress/Stable-Diffusion-Desktop-Client).  
Cross-platform FMX desktop client for Stable Diffusion (Windows, macOS, Linux). Calls SD via REST API.  
`[FMX]`

---

## Community

* [Delphi-PRAXiS — AI & LLM discussions](https://en.delphipraxis.net/forum/43-ai-assisted-coding/).  
Community forum. Search "Claude", "AI", or "LLM" for ongoing threads on integrating AI into Delphi development.  

* [awesome-chatgpt (HemulGM)](https://github.com/HemulGM/awesome-chatgpt).  
General (non-Delphi) curated list of ChatGPT resources, tools, and projects. Useful background reading.  


---

## Commercial Tools

*Paid or source-available products. Clearly marked.*



* [Claude Code Training for Delphi Developers](https://training.gdksoftware.com/).  
Dedicated training by GDK Software. CLAUDE.md setup, MCP integration, Delphi-specific Claude Code workflows.  
`[Commercial]` `[Claude Code]`

---

## Contributing

PRs welcome. Criteria:
- Must be AI-related AND Delphi/Pascal relevant
- Open-source highly preferred; commercial tools listed if uniquely valuable. Needs to clearly state so!!
- Dead projects (2+ years no updates) excluded unless irreplaceable
