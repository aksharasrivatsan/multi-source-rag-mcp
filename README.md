# Multi-Source RAG System (with GitHub & Web Connectors)

This project implements a robust **Retrieval-Augmented Generation (RAG)** pipeline that goes beyond static documents. It uses a local LLM to answer questions by dynamically pulling context from local PDFs, GitHub repositories, and live web searches.

 *(Note: Replace with your architecture diagram or screenshot)*

## Key Features
- **Local LLM:** Powered by Ollama (Llama 3.2) for private, local inference.
- **Multi-Source Context:** - **Local PDFs:** Deep-dive into personal documents using PyPDF and FAISS.
  - **GitHub MCP:** Search and ingest code directly from GitHub repositories.
  - **Web Search:** Fetch the latest news and trends via DuckDuckGo.
- **Smart Query Routing:** Automatically detects if a query needs "Live Web Search" or "Code Implementation" and fetches context accordingly.

## Tech Stack
- **Framework:** LangChain
- **Vector Store:** FAISS (Facebook AI Similarity Search)
- **Embeddings:** HuggingFace (`all-MiniLM-L6-v2`)
- **LLM:** Ollama (Llama 3.2)
- **APIs:** PyGithub, DuckDuckGo Search

## Getting Started

1. **Install Ollama:**
   Download and install from [ollama.com](https://ollama.com).
   ```bash
   ollama pull llama3.2
