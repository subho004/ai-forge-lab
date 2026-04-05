# 🛠️ AI Forge Lab

![AI Forge Lab Header](assets/header.png)

Welcome to the **AI Forge Lab**, a premier collection of cutting-edge AI research, autonomous agents, and experimental demos. This repository serves as a centralized hub for projects exploring the boundaries of LLM reasoning, autonomous workflows, and innovative RAG architectures.

---

## 🚀 Featured Projects

| Project | Description | Key Tech |
| :--- | :--- | :--- |
| [**OpenEvolve**](./openevolve-guide) | Framework for building self-evolving AI agents that improve their own code. | Python, LLMs, Process Isolation |
| [**Auto-Research**](./auto-research-guide) | Automated technical and scientific research workflows powered by AI. | LangChain, Research APIs |
| [**Fine-Tuning Guide**](./finetuning-guide) | Comprehensive reference for fine-tuning LLMs (LoRA, QLoRA, DPO, RLHF). | PEFT, bitsandbytes, TRL |
| [**MCP Chatbot**](./mcp-chatbot) | A modular chatbot implementation using the Model Context Protocol (MCP). | LangChain, MCP, Groq |
| [**Podcast Automate**](./podcast-automate) | End-to-end automation for podcast production, from script to speech. | Maya1, TTS, LLMs |
| [**Vectorless RAG**](./vectorless-llm-evals) | Evaluating RAG systems using PageIndex for hierarchical, vectorless retrieval. | PageIndex, LangSmith |
| [**Graph LLMs**](./graph-llms) | Integrating Knowledge Graphs (Neo4j) with LLM reasoning for complex queries. | Neo4j, Cypher, Groq |

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

---

## 📜 Contributing & License

We welcome contributions to any of the sub-modules! Please refer to the individual project directories for specific contribution guidelines.

This lab is provided under the **MIT License**.

---
*Created with ❤️ by the AI Forge Lab Team*
