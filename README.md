Conversational RAG Agent with LangChain & Ollama
This project implements a conversational AI agent powered by a Retrieval-Augmented Generation (RAG) pipeline using LangChain, Ollama (LLaMA 3), and FAISS. The agent can answer questions from documentation, execute Python code, and perform real-time web searches through a simple Gradio interface.

Features
LangChain documentation retrieval using FAISS and contextual compression

Local large language model served via Ollama (LLaMA 3)

Tool integration with Python REPL and SerpAPI web search

Conversational memory for context-aware Q&A

Web-based interface built with Gradio

Tech Stack
Language Model: LLaMA 3 (via Ollama)

Framework: LangChain

Retrieval: FAISS with ContextualCompressionRetriever

Interface: Gradio

Tools: SerpAPI for search, PythonREPL for code execution

Embeddings: OllamaEmbeddings

Installation
Install required Python packages:

bash
Copy
Edit
pip install gradio langchain faiss-cpu langchain-community langchain-experimental google-search-results
Install and run Ollama:

bash
Copy
Edit
curl -fsSL https://ollama.com/install.sh | sh
ollama pull llama3
(Optional) Set your SerpAPI key:

python
Copy
Edit
SERPAPI_API_KEY = "your_key_here"
Running the Project
To launch the assistant, run:

bash
Copy
Edit
python main.py
Then open your browser and go to:

arduino
Copy
Edit
http://localhost:7867
Project Structure
main.py – Main script to launch Ollama, load tools, and start Gradio

faiss_index/ – Cached vector store of documentation

langchain_chunks.txt – Exported doc chunks for inspection

.ipynb – Optional notebook version for interactive exploration

Notes
The Ollama LLM must be running locally in the background (ollama serve)

First run may take time while downloading and embedding documents

This environment differs from Kaggle's; some additional setup may be required
