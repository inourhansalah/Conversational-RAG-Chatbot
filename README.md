## Project Overview

This project is a **Retrieval-Augmented Generation (RAG) chatbot** built using **LangChain**, **Ollama**, and **FAISS**, with an interactive interface powered by **Gradio**. It is designed to provide intelligent responses based on LangChain documentation, execute Python code, and perform real-time web searches.

The system utilizes the **LLaMA 3** model through Ollama, enabling local inference. It also integrates additional tools such as **SerpAPI** for web search and a Python REPL environment for code execution.

---

##  How It Works

- **Document Loading & Vectorization**  
  LangChain documentation is scraped from the web, split into smaller chunks, embedded using Ollama, and indexed with **FAISS** for fast vector-based search.

- **LLM via Ollama**  
  The system uses **LLaMA 3**, running locally through **Ollama**, to generate natural language responses.

- **Tool-Augmented Agent**  
  The chatbot is powered by a LangChain agent capable of using multiple tools: a retriever for documentation, a Python code executor, and a live web search tool.

- **Conversational Memory**  
  The chatbot maintains chat history using LangChain’s **ConversationBufferMemory**, enabling context-aware interactions.

- **Web Interface with Gradio**  
  Users interact through a simple, user-friendly **Gradio** interface, where they can ask questions and receive live, intelligent responses.

---

##  Features

-  **Context-aware answers** from LangChain documentation
-  **LLaMA 3 integration** via Ollama for offline inference
-  **Python code execution** within the chatbot
-  **Real-time web search** using SerpAPI
-  **Interactive chatbot UI** powered by Gradio
-  **FAISS vector index** for fast document retrieval
-  **Memory support** for ongoing conversations

---

##  Tools & Libraries Used

| Tool / Library         | Purpose                                          |
|------------------------|--------------------------------------------------|
| **LangChain**          | Framework for building LLM-powered apps          |
| **Ollama**             | Local LLM inference with models like LLaMA 3     |
| **FAISS**              | Efficient similarity search for vector retrieval |
| **Gradio**             | Web UI for interacting with the chatbot          |
| **SerpAPI**            | Real-time search for current web content         |
| **Python REPL Tool**   | Executes Python code submitted by users          |
| **LangChain Memory**   | Tracks conversation context across messages      |

---

##  Use Cases

- Learn and explore LangChain documentation interactively  
- Run Python snippets for experimentation and debugging  
- Ask technical questions or request code examples  
- Retrieve real-time info using web search  
- Experiment with tool-augmented LLMs and RAG architecture
