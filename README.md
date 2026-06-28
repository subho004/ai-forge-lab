# 🛠️ AI Forge Lab

![AI Forge Lab Header](assets/header.png)

Welcome to the **AI Forge Lab**, a premier collection of cutting-edge AI research, autonomous agents, and experimental demos. This repository serves as a centralized hub for projects exploring the boundaries of LLM reasoning, autonomous workflows, and innovative RAG architectures.

---

## 🚀 Featured Projects

| Project                                      | Description                                                                         | Key Tech                        |
| :------------------------------------------- | :---------------------------------------------------------------------------------- | :------------------------------ |
| [**OpenEvolve**](./openevolve-guide)         | Framework for building self-evolving AI agents that improve their own code.         | Python, LLMs, Process Isolation |
| [**Auto-Research**](./auto-research-guide)   | Automated technical and scientific research workflows powered by AI.                | LangChain, Research APIs        |
| [**Fine-Tuning Guide**](./finetuning-guide)  | Comprehensive reference for fine-tuning LLMs (LoRA, QLoRA, DPO, RLHF).              | PEFT, bitsandbytes, TRL         |
| [**MCP Chatbot**](./mcp-chatbot)             | A modular chatbot implementation using the Model Context Protocol (MCP).            | LangChain, MCP, Groq            |
| [**Podcast Automate**](./podcast-automate)   | End-to-end automation for podcast production, from script to speech.                | Maya1, TTS, LLMs                |
| [**A2A Guide**](./a2a-guide)                 | Action-to-Action guide: practical examples and patterns for chaining agent actions. | Examples, Guides                |
| [**Vectorless RAG**](./vectorless-llm-evals) | Evaluating RAG systems using PageIndex for hierarchical, vectorless retrieval.      | PageIndex, LangSmith            |
| [**Graph LLMs**](./graph-llms)               | Integrating Knowledge Graphs (Neo4j) with LLM reasoning for complex queries.        | Neo4j, Cypher, Groq             |
| [**GPT-Scratch**](./gpt-scratch)             | Build, deconstruct, and train decoder-only Generative Pre-trained Transformers.     | PyTorch, tiktoken, GPT-2        |
| [**Long-Context Compliance**](./long-document-context) | Multi-agent, multi-pass pipeline for extracting and synthesizing compliance evidence from long PDFs. | FastAPI, Groq, Datalab OCR, BM25 |
| [**RLM Research Agent**](./rlm-test)         | In-memory deep-research agent over a local markdown corpus using recursive decomposition. | FastAPI, LangChain, LangGraph, OpenAI |
| [**RPG World Simulator**](./world-simulator) | Interactive RPG sandbox with Gemini world transition engine, memory reflection, and emergent economy. | FastAPI, Gemini, NetworkX, Cytoscape.js |

---

## 🛠️ Getting Started

This repository uses **Git Submodules** to manage individual projects. To get everything up and running:

### 1. Clone the Repository

```bash
git clone --recursive https://github.com/subho004/ai-forge-lab.git
cd ai-forge-lab
```

### 2. Initialize Submodules (if already cloned)

```bash
git submodule update --init --recursive
```

### A2A Guide submodule

This repository includes the A2A Guide as a git submodule. It's located at `a2a-guide` and sourced from https://github.com/subho004/a2a-guide.

To initialize or update only this submodule after cloning:

```bash
git submodule update --init a2a-guide
cd a2a-guide
git pull origin main
cd ..
```

You can inspect the submodule contents in `a2a-guide` and follow its README for usage examples.

### GPT-Scratch submodule

This repository includes the GPT-Scratch Laboratory as a git submodule. It's located at `gpt-scratch` and sourced from https://github.com/subho004/attention-to-gpt-scratch.

To initialize or update only this submodule after cloning:

```bash
git submodule update --init gpt-scratch
cd gpt-scratch
git pull origin main
cd ..
```

You can inspect the submodule contents in `gpt-scratch` and follow its README for usage examples.

### Long-Context Compliance submodule

This repository includes the Long-Context Compliance Retrieval API as a git submodule. It's located at `long-document-context` and sourced from https://github.com/subho004/agentic-deep-reader.

To initialize or update only this submodule after cloning:

```bash
git submodule update --init long-document-context
cd long-document-context
git pull origin main
cd ..
```

You can inspect the submodule contents in `long-document-context` and follow its README for usage examples.

### RLM Research Agent submodule

This repository includes the In-Memory RLM Research Agent as a git submodule. It's located at `rlm-test` and sourced from https://github.com/subho004/bm25-rlm-agent.

To initialize or update only this submodule after cloning:

```bash
git submodule update --init rlm-test
cd rlm-test
git pull origin main
cd ..
```

You can inspect the submodule contents in `rlm-test` and follow its README for usage examples.

### RPG World Simulator submodule

This repository includes the RPG World Simulator as a git submodule. It's located at `world-simulator` and sourced from https://github.com/subho004/llm-rpg-world-simulator.

To initialize or update only this submodule after cloning:

```bash
git submodule update --init world-simulator
cd world-simulator
git pull origin main
cd ..
```

You can inspect the submodule contents in `world-simulator` and follow its README and docs folder for usage examples.

#### Overview & Mechanics
- **World Transition Engine:** LLM parses player intent and NPC actions to output structured state diffs, processed via a validation choke point (`DiffApplier`).
- **Emergent Quests:** short supply triggers fetch quests; completing them pays rewards, resolves shortages, and spawns rumors.
- **Cognitive Agent Memory:** episodic memories are periodically reflected upon and consolidated into abstract insights.
- **Social Cliques & Rumor Decay:** community detection groups NPCs, while rumors decay in truth value as they propagate through the locations graph.
- **Interactive Sandbox UI:** visual cytoscape.js map, command parser, detail logs, and save/load state functionality.

Refer to the companion documentation inside the submodule for further details:
- [GAME_GUIDE.md](file:///Users/subhajithait/Documents/testing/ai-forge-lab/world-simulator/docs/GAME_GUIDE.md): Guide on how to play, command lists, and UI controls.
- [MANUAL.md](file:///Users/subhajithait/Documents/testing/ai-forge-lab/world-simulator/docs/MANUAL.md): Technical architecture, API reference, configuration settings, and database schema.
- [future_notes.md](file:///Users/subhajithait/Documents/testing/ai-forge-lab/world-simulator/docs/future_notes.md): Future expansion roadmap including continent-scale grid, semantic vector memory, multi-agent conversation, and isometric WebGL rendering.

### 3. Explore Projects

Each project resides in its own directory and has a specific `README.md` with installation and usage instructions.

---

## 🧪 Research Themes

### 🧠 Autonomous Evolution

Exploring how LLMs can iteratively improve their own logic and tools through self-correction and performance-based evolution (see **OpenEvolve**).

### 📖 Model Fine-Tuning & Alignment

Reference guide for advanced alignment strategies including Supervised Fine-Tuning (SFT), LoRA/QLoRA, and preference optimization (DPO) (see **Fine-Tuning Guide**).

### 🕸️ Graph-Based Reasoning

Moving beyond flat vector embeddings toward structured wisdom using Knowledge Graphs for more accurate and traceable RAG (see **Graph LLMs**).

### 🎙️ AI Content Pipelines

Streamlining the path from raw data/ideas to polished media outputs like podcasts (see **Podcast Automate**).

### 📚 Recursive Research & Long-Context Compliance

Multi-agent pipelines designed to synthesize structured evidence from massive (1000+ page) corpora using iterative refinement, BM25 dependency resolution, and LangGraph-driven self-correction (see **Long-Context Compliance** and **RLM Research Agent**).

### 🗺️ Generative World Simulations & RPGs

Designing LLM-driven role-playing simulations where models act as structured intent parsers and planners, with episodic memory reflection, emergent trade economies, and rumor propagation (see [**RPG World Simulator**](file:///Users/subhajithait/Documents/testing/ai-forge-lab/world-simulator)).

---

## 📜 Contributing & License

We welcome contributions to any of the sub-modules! Please refer to the individual project directories for specific contribution guidelines.

This lab is provided under the **MIT License**.

---

---

\*Created with ❤️ by the [subho004](https://github.com/subho004)
