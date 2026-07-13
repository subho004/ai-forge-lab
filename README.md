# 🛠️ AI Forge Lab

![AI Forge Lab Header](assets/header2.png)

<div align="center">

**A monorepo of cutting-edge AI research, autonomous agents, and experimental LLM demos.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Projects](https://img.shields.io/badge/projects-19-blue.svg)](#-featured-projects)
[![Git Submodules](https://img.shields.io/badge/git-submodules-orange.svg)](#%EF%B8%8F-getting-started)
[![Python](https://img.shields.io/badge/python-3.10%2B-3776AB.svg?logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688.svg?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#-contributing)
[![GitHub stars](https://img.shields.io/github/stars/subho004/ai-forge-lab?style=social)](https://github.com/subho004/ai-forge-lab/stargazers)

</div>

---

Welcome to the **AI Forge Lab** — a centralized hub for projects exploring the boundaries of LLM reasoning, autonomous workflows, and innovative RAG architectures. Each project lives in its own GitHub repository and is wired into this lab as a **git submodule**, so you can clone everything at once or pick a single project to dive into.

## 📚 Table of Contents

- [Featured Projects](#-featured-projects)
- [Getting Started](#%EF%B8%8F-getting-started)
- [Working with Individual Submodules](#-working-with-individual-submodules)
- [Research Themes](#-research-themes)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🚀 Featured Projects

Project names below match their upstream GitHub repository names. Click any project to open its dedicated repo.

| Project | Description | Key Tech |
| :------ | :---------- | :------- |
| [`openevolve-guide`](https://github.com/subho004/openevolve-guide) | Framework for building self-evolving AI agents that improve their own code. | Python, LLMs, Process Isolation |
| [`auto-research-guide`](https://github.com/subho004/auto-research-guide) | Automated technical and scientific research workflows powered by AI. | LangChain, Research APIs |
| [`finetuning-guide`](https://github.com/subho004/finetuning-guide) | Comprehensive reference for fine-tuning LLMs (LoRA, QLoRA, DPO, RLHF). | PEFT, bitsandbytes, TRL |
| [`mcp-chatbot`](https://github.com/subho004/mcp-chatbot) | A modular chatbot implementation using the Model Context Protocol (MCP). | LangChain, MCP, Groq |
| [`podcast-automate`](https://github.com/subho004/podcast-automate) | End-to-end automation for podcast production, from script to speech. | Maya1, TTS, LLMs |
| [`a2a-guide`](https://github.com/subho004/a2a-guide) | Action-to-Action guide: practical patterns for chaining agent actions. | Examples, Guides |
| [`vectorless-llm-evals`](https://github.com/subho004/vectorless-llm-evals) | Evaluating RAG systems using PageIndex for hierarchical, vectorless retrieval. | PageIndex, LangSmith |
| [`graph-llms`](https://github.com/subho004/graph-llms) | Integrating Knowledge Graphs (Neo4j) with LLM reasoning for complex queries. | Neo4j, Cypher, Groq |
| [`attention-to-gpt-scratch`](https://github.com/subho004/attention-to-gpt-scratch) | Build, deconstruct, and train decoder-only Generative Pre-trained Transformers. | PyTorch, tiktoken, GPT-2 |
| [`agentic-deep-reader`](https://github.com/subho004/agentic-deep-reader) | Multi-agent, multi-pass pipeline for extracting compliance evidence from long PDFs. | FastAPI, Groq, Datalab OCR, BM25 |
| [`bm25-rlm-agent`](https://github.com/subho004/bm25-rlm-agent) | In-memory deep-research agent over a local markdown corpus using recursive decomposition. | FastAPI, LangChain, LangGraph, OpenAI |
| [`llm-rpg-world-simulator`](https://github.com/subho004/llm-rpg-world-simulator) | Interactive RPG sandbox with Gemini world-transition engine, memory reflection, and emergent economy. | FastAPI, Gemini, NetworkX, Cytoscape.js |
| [`mem-git-agent`](https://github.com/subho004/mem-git-agent) | Self-contained MemGPT agent with tiered memory and versioned "memory git". | FastAPI, SQLite, NumPy, OpenAI, MarkItDown |
| [`turboquant-personal-ai`](https://github.com/subho004/turboquant-personal-ai) | Folder-based personal AI with perfect memory via TurboVec quantization and hybrid retrieval. | FastAPI, SQLite, TurboVec, FAISS, OpenAI |
| [`okf-knowledge-graph-wiki`](https://github.com/subho004/okf-knowledge-graph-wiki) | Ingests heterogeneous files, analyzes dependencies, and builds an AI-queryable OKF wiki. | Python 3.14, FastAPI, Gemini 3, SQLite, sqlite-vec, NetworkX |
| [`omni-agent`](https://github.com/subho004/omni-agent) | Agentic research harness executing parallel sub-agents with planning and self-correction. | Python 3.14, FastAPI, Gemini, SQLAlchemy, NetworkX, MarkItDown |
| [`llm-distillation-guide`](https://github.com/subho004/llm-distillation-guide) | A hands-on guide to LLM knowledge distillation: using Llama-3 (via Groq) to label synthetic data and fine-tuning a 1000x smaller RoBERTa student. | Llama-3, Groq, RoBERTa, PyTorch, Hugging Face |
| [`rlm-due-diligence-agents`](https://github.com/subho004/rlm-due-diligence-agents) | Autonomous investment analyst leveraging LangChain Deep Agents & RLM-style dynamic workflows to run end-to-end technical, market, and financial due diligence with human-in-the-loop validation. | LangChain, Deep Agents, RLM, Python |
| [`omni-video-agent`](https://github.com/subho004/omni-video-agent) | End-to-end automated video generation: researches the web, writes a storyboard, generates clips (Veo 3.1) and music (Lyria 3), and compiles the final video. | LangChain Deep Agents, Gemini (Veo 3.1, Lyria 3, Nano Banana 2), crawl4ai, MarkItDown, FastAPI, SQLite, ffmpeg |

> **Local paths:** each repo is mounted in this monorepo at a submodule path. See the mapping in [Working with Individual Submodules](#-working-with-individual-submodules).

---

## 🛠️ Getting Started

This repository uses **Git Submodules** to manage individual projects.

### 1. Clone with all submodules

```bash
git clone --recursive https://github.com/subho004/ai-forge-lab.git
cd ai-forge-lab
```

### 2. Already cloned? Initialize submodules

```bash
git submodule update --init --recursive
```

### 3. Explore projects

Each project resides in its own directory and has a dedicated `README.md` with installation and usage instructions.

---

## 📦 Working with Individual Submodules

Each project's **display name = its GitHub repo name**. The table below maps that repo (and URL) to the local submodule path inside this monorepo.

| GitHub Repository | URL | Local Path |
| :---------------- | :-- | :--------- |
| `openevolve-guide` | https://github.com/subho004/openevolve-guide | `openevolve-guide` |
| `auto-research-guide` | https://github.com/subho004/auto-research-guide | `auto-research-guide` |
| `finetuning-guide` | https://github.com/subho004/finetuning-guide | `finetuning-guide` |
| `mcp-chatbot` | https://github.com/subho004/mcp-chatbot | `mcp-chatbot` |
| `podcast-automate` | https://github.com/subho004/podcast-automate | `podcast-automate` |
| `a2a-guide` | https://github.com/subho004/a2a-guide | `a2a-guide` |
| `vectorless-llm-evals` | https://github.com/subho004/vectorless-llm-evals | `vectorless-llm-evals` |
| `graph-llms` | https://github.com/subho004/graph-llms | `graph-llms` |
| `attention-to-gpt-scratch` | https://github.com/subho004/attention-to-gpt-scratch | `gpt-scratch` |
| `agentic-deep-reader` | https://github.com/subho004/agentic-deep-reader | `long-document-context` |
| `bm25-rlm-agent` | https://github.com/subho004/bm25-rlm-agent | `rlm-test` |
| `llm-rpg-world-simulator` | https://github.com/subho004/llm-rpg-world-simulator | `world-simulator` |
| `mem-git-agent` | https://github.com/subho004/mem-git-agent | `memgpt-test` |
| `turboquant-personal-ai` | https://github.com/subho004/turboquant-personal-ai | `turboquant-test` |
| `okf-knowledge-graph-wiki` | https://github.com/subho004/okf-knowledge-graph-wiki | `okf+llm wiki` |
| `omni-agent` | https://github.com/subho004/omni-agent | `harness-ultimate` |
| `llm-distillation-guide` | https://github.com/subho004/llm-distillation-guide | `LLM-distillation-guide` |
| `rlm-due-diligence-agents` | https://github.com/subho004/rlm-due-diligence-agents | `deep-agents-due-diligence` |
| `omni-video-agent` | https://github.com/subho004/omni-video-agent | `agentic-video-generator` |

To initialize or update a single submodule after cloning:

```bash
# Example: agentic-deep-reader lives at ./long-document-context
git submodule update --init long-document-context
cd long-document-context
git pull origin main
cd ..
```

> Paths containing special characters (e.g. `okf+llm wiki`) must be quoted:
> `git submodule update --init "okf+llm wiki"`

### Project deep-dives

<details>
<summary><b>openevolve-guide</b> — Self-evolving AI agents (<code>openevolve-guide</code>)</summary>

Framework for building self-evolving AI agents that improve their own code.

**Key tech:** Python, LLMs, Process Isolation.
</details>

<details>
<summary><b>auto-research-guide</b> — Automated research workflows (<code>auto-research-guide</code>)</summary>

Automated technical and scientific research workflows powered by AI.

**Key tech:** LangChain, Research APIs.
</details>

<details>
<summary><b>finetuning-guide</b> — LLM fine-tuning reference (<code>finetuning-guide</code>)</summary>

Comprehensive reference for fine-tuning LLMs (LoRA, QLoRA, DPO, RLHF).

**Key tech:** PEFT, bitsandbytes, TRL.
</details>

<details>
<summary><b>mcp-chatbot</b> — Modular MCP chatbot (<code>mcp-chatbot</code>)</summary>

A modular chatbot implementation using the Model Context Protocol (MCP).

**Key tech:** LangChain, MCP, Groq.
</details>

<details>
<summary><b>podcast-automate</b> — Podcast production automation (<code>podcast-automate</code>)</summary>

End-to-end automation for podcast production, from script to speech.

**Key tech:** Maya1, TTS, LLMs.
</details>

<details>
<summary><b>a2a-guide</b> — Action-to-Action agent patterns (<code>a2a-guide</code>)</summary>

Action-to-Action guide: practical examples and patterns for chaining agent actions.

**Key tech:** Examples, Guides.
</details>

<details>
<summary><b>vectorless-llm-evals</b> — Vectorless RAG evaluation (<code>vectorless-llm-evals</code>)</summary>

Evaluating RAG systems using PageIndex for hierarchical, vectorless retrieval.

**Key tech:** PageIndex, LangSmith.
</details>

<details>
<summary><b>graph-llms</b> — Knowledge-graph reasoning (<code>graph-llms</code>)</summary>

Integrating Knowledge Graphs (Neo4j) with LLM reasoning for complex queries.

**Key tech:** Neo4j, Cypher, Groq.
</details>

<details>
<summary><b>attention-to-gpt-scratch</b> — GPT from scratch (<code>gpt-scratch</code>)</summary>

Build, deconstruct, and train decoder-only Generative Pre-trained Transformers.

**Key tech:** PyTorch, tiktoken, GPT-2.
</details>

<details>
<summary><b>agentic-deep-reader</b> — Long-context compliance pipeline (<code>long-document-context</code>)</summary>

Multi-agent, multi-pass pipeline for extracting and synthesizing compliance evidence from long PDFs.

**Key tech:** FastAPI, Groq, Datalab OCR, BM25.
</details>

<details>
<summary><b>bm25-rlm-agent</b> — Recursive research agent (<code>rlm-test</code>)</summary>

In-memory deep-research agent over a local markdown corpus using recursive decomposition.

**Key tech:** FastAPI, LangChain, LangGraph, OpenAI.
</details>

<details>
<summary><b>llm-rpg-world-simulator</b> — Generative RPG sandbox (<code>world-simulator</code>)</summary>

Interactive RPG sandbox with Gemini world-transition engine, memory reflection, and emergent economy.


- **World Transition Engine:** LLM parses player intent and NPC actions to output structured state diffs, processed via a validation choke point (`DiffApplier`).
- **Emergent Quests:** short supply triggers fetch quests; completing them pays rewards, resolves shortages, and spawns rumors.
- **Cognitive Agent Memory:** episodic memories are periodically reflected upon and consolidated into abstract insights.
- **Social Cliques & Rumor Decay:** community detection groups NPCs, while rumors decay in truth value as they propagate through the locations graph.
- **Interactive Sandbox UI:** visual Cytoscape.js map, command parser, detail logs, and save/load state.

Companion docs inside the submodule: `docs/GAME_GUIDE.md`, `docs/MANUAL.md`, `docs/future_notes.md`.
</details>

<details>
<summary><b>mem-git-agent</b> — MemGPT tiered-memory agent (<code>memgpt-test</code>)</summary>

Self-contained MemGPT agent with tiered memory (persona, human, document catalog, recall, archival) and versioned "memory git".

- **Tiered Memory Hierarchy:** maps OS memory concepts to LLMs — editable core memory (`persona`/`human`) always in context (RAM), a message FIFO queue, a document catalog, with full transcripts (recall) and embedded passages (archival) on disk.
- **Control Loop & Heartbeats:** decouples thinking/acting from speaking via an inner monologue and automated heartbeats, chaining multiple search/edit calls before replying via `send_message`.
- **Document Catalog Tier:** always-in-context single-line metadata per document so the agent knows its whole library at a glance.
- **Versioned "Memory Git":** tracks all core-memory changes in a queryable, revertible database.
- **Context Eviction & Summarization:** manages token limits by prompting under memory pressure and recursively folding evicted history into a running summary.
- **Hybrid Retrieval & Reranking:** in-process NumPy similarity search fused with SQLite FTS5 BM25, then a cheap LLM rerank.

Companion docs: `docs/notes.md`.
</details>

<details>
<summary><b>turboquant-personal-ai</b> — Ultra-low-bit vector memory (<code>turboquant-test</code>)</summary>

Folder-based personal AI assistant with perfect memory powered by TurboVec quantization and hybrid retrieval.

- **TurboVec Vector Index:** Rust implementation of Google Research's TurboQuant for 2-bit/4-bit quantization with AVX-512/NEON SIMD flat search — no index training or codebooks, high recall.
- **Folder-Based Knowledge Management:** uploads trigger MarkItDown parsing (or Whisper for audio), token-aware chunking, OpenAI embeddings, and multi-index updates.
- **Follow-up Aware Conversation:** rewrites multi-turn queries into standalone search queries.
- **Persistent Conversation Memory:** summarizes turns into a separate TurboVec memory index for cross-session recall.
- **Cost & Token Tracker** and **Benchmark Dashboard** (TurboVec vs. FAISS IndexPQ/IndexFlat).

Companion docs: `docs/notes.md`.
</details>

<details>
<summary><b>okf-knowledge-graph-wiki</b> — Company Knowledge Builder (<code>okf+llm wiki</code>)</summary>

Ingests heterogeneous files, analyzes dependencies, and builds an AI-queryable OKF wiki.

- **Universal Ingestion & Structure Analysis:** heuristically analyzes project files (ZIP, PDF, DOCX, OpenAPI, SQL DDL) into a typed NetworkX dependency graph.
- **Concept Page Extraction:** structures key concepts with Gemini into Open Knowledge Format (OKF) markdown pages.
- **Auto Wiki-Linking:** resolves relative links between concepts, turning dangling references into stub pages.
- **Hybrid Search & SSE Streaming:** `sqlite-vec` semantic search + BM25 fused with RRF, streaming RAG chat and pipeline status over SSE.

Companion docs: `docs/Company_Knowledge_Builder_OKF_Project_Idea.txt`, `docs/implementation_plan.md`, `docs/notes.md`.
</details>

<details>
<summary><b>omni-agent</b> — Multi-agent DAG research harness (<code>harness-ultimate</code>)</summary>

Agentic research harness executing parallel sub-agents with planning and self-correction.

- **Multi-Agent DAG Planning:** a NetworkX DAG executes tasks in parallel via specialized sub-agents.
- **Self-Correction & Evaluation:** critiques performance and dynamically reshapes/re-plans steps mid-flight.
- **Recursive Sub-Agent Fan-Out:** spawns nested sub-agents to delegate granular tasks in parallel.
- **Grounding & Headless Browser Tools:** ~16 real-world tools — Google Search grounding, browser-use/crawl4ai automation, sandboxed command execution, hybrid vector/BM25 retrieval.

Companion docs: `docs/idea.md`, `docs/implementation-plan.md`.
</details>

<details>
<summary><b>llm-distillation-guide</b> — LLM knowledge distillation (<code>LLM-distillation-guide</code>)</summary>

Hands-on guide to LLM knowledge distillation: using Llama-3 (via Groq) to label synthetic data and fine-tuning a 1000x smaller RoBERTa student.

**Key tech:** Llama-3, Groq, RoBERTa, PyTorch, Hugging Face.
</details>

<details>
<summary><b>rlm-due-diligence-agents</b> — Autonomous due diligence (<code>deep-agents-due-diligence</code>)</summary>

Autonomous investment analyst leveraging LangChain Deep Agents & RLM-style dynamic workflows to run end-to-end technical, market, and financial due diligence with human-in-the-loop validation.

**Key tech:** LangChain, Deep Agents, RLM, Python.
</details>

<details>
<summary><b>omni-video-agent</b> — Automated video generation (<code>agentic-video-generator</code>)</summary>

End-to-end automated video generation from a single query: researches the web, storyboards scenes, generates video clips and music, and compiles the final video.

- **Web Research & Synthesis:** uses LangChain Deep Agents with crawl4ai (scraping) and MarkItDown (document parsing) to research a topic and build a structured knowledge wiki.
- **Storyboard Generation:** uses Gemini structured output to translate the research wiki into a shot-by-shot storyboard with Veo prompts, Lyria music briefs, and thumbnail prompts.
- **Media Generation & Continuity:** generates 30–60s video clips via Veo 3.1 (with native audio/dialogue and scene extensions) and composes a custom background music bed via Lyria 3.
- **Assembly & UI:** mixes and compiles video clips, narration, and background music using ffmpeg into a final `.mp4` and creates a poster thumbnail with Nano Banana 2, served via a vanilla HTML/CSS/JS frontend.

Companion docs: `docs/implementation-plan.md`.
</details>

---

## 🧪 Research Themes

### 🧠 Autonomous Evolution
LLMs iteratively improving their own logic and tools through self-correction and performance-based evolution — see [`openevolve-guide`](https://github.com/subho004/openevolve-guide).

### 📖 Model Fine-Tuning, Alignment & Distillation
Advanced alignment strategies including SFT, LoRA/QLoRA, preference optimization (DPO), and knowledge distillation to smaller student models — see [`finetuning-guide`](https://github.com/subho004/finetuning-guide) and [`llm-distillation-guide`](https://github.com/subho004/llm-distillation-guide).

### 🕸️ Graph-Based Reasoning
Moving beyond flat vector embeddings toward structured knowledge graphs for accurate, traceable RAG — see [`graph-llms`](https://github.com/subho004/graph-llms) and [`okf-knowledge-graph-wiki`](https://github.com/subho004/okf-knowledge-graph-wiki).

### 🎙️ AI Content Pipelines
Streamlining the path from raw ideas to polished media like podcasts and videos — see [`podcast-automate`](https://github.com/subho004/podcast-automate) and [`omni-video-agent`](https://github.com/subho004/omni-video-agent).

### 📚 Recursive Research & Long-Context Compliance
Multi-agent pipelines synthesizing structured evidence from massive (1000+ page) corpora via iterative refinement, BM25 dependency resolution, and LangGraph self-correction — see [`agentic-deep-reader`](https://github.com/subho004/agentic-deep-reader) and [`bm25-rlm-agent`](https://github.com/subho004/bm25-rlm-agent).

### 🗺️ Generative World Simulations & RPGs
LLM-driven role-playing simulations with structured intent parsing, episodic memory reflection, emergent trade economies, and rumor propagation — see [`llm-rpg-world-simulator`](https://github.com/subho004/llm-rpg-world-simulator).

### 💾 Stateful Memory & OS-Style Agent Architectures
LLMs as operating systems: tiered memory hierarchies (RAM vs. disk), tool-driven memory paging, context eviction/summarization, and versioned memory histories — see [`mem-git-agent`](https://github.com/subho004/mem-git-agent).

### ⚡ High-Efficiency Vector Quantization & Semantic Search
Ultra-low-bit quantization à la Google Research's TurboQuant (1536-dim → 2–4 bits, no training/codebooks) benchmarked against FAISS — see [`turboquant-personal-ai`](https://github.com/subho004/turboquant-personal-ai).

### 🤖 Multi-Agent Planning & Self-Correction
Decomposing complex queries into parallelized DAG execution plans or dynamic workflows with self-reflection, browser automation, sandboxed runtimes, hybrid retrieval, and human-in-the-loop verification — see [`omni-agent`](https://github.com/subho004/omni-agent) and [`rlm-due-diligence-agents`](https://github.com/subho004/rlm-due-diligence-agents).

---

## 🤝 Contributing

Contributions are welcome across all sub-projects! Since each project is an independent repository:

1. Open issues and pull requests **on the individual project's GitHub repo** (linked in the tables above).
2. Refer to each project directory's own `README.md` for project-specific contribution guidelines.
3. For monorepo-level changes (this README, submodule wiring), open a PR against [`ai-forge-lab`](https://github.com/subho004/ai-forge-lab).

---

## 📜 License

This lab is released under the **MIT License** — see [LICENSE](./LICENSE) for details. Individual submodules may carry their own licenses; check each repository.

---

<div align="center">

Created with ❤️ by [**subho004**](https://github.com/subho004)

</div>
