# Conversational RAG Agent with LangChain & Ollama

This project implements a conversational AI agent powered by a Retrieval-Augmented Generation (RAG) pipeline using LangChain, Ollama (LLaMA 3), and FAISS. The agent can answer questions from documentation, execute Python code, and perform real-time web searches through a simple Gradio interface.

---

## Features

- LangChain documentation retrieval using FAISS and contextual compression
- Local large language model served via Ollama (LLaMA 3)
- Tool integration with Python REPL and SerpAPI web search
- Conversational memory for context-aware Q&A
- Web-based interface built with Gradio

---

## Tech Stack

- **Language Model**: LLaMA 3 (via Ollama)
- **Framework**: LangChain
- **Retrieval**: FAISS with ContextualCompressionRetriever
- **Interface**: Gradio
- **Tools**: SerpAPI for search, PythonREPL for code execution
- **Embeddings**: OllamaEmbeddings

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
