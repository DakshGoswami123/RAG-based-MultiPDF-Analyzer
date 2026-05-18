# Multi-PDF Research Assistant

This is a RAG-based (Retrieval-Augmented Generation) project I worked on to understand how large language models can answer questions using external document data instead of relying only on pretrained knowledge.

The main idea is simple: upload one or more PDF documents, ask questions in natural language, and get answers based on the uploaded content.

I built this as a learning project to explore document retrieval, embeddings, vector databases, and integrating LLMs into a practical application.

---

## Features

- Upload and process multiple PDF documents
- Semantic search using embeddings
- Fast document retrieval using FAISS
- Question answering using Google Gemini
- Local fallback keyword-based retrieval if API/vector retrieval fails
- Simple interactive Streamlit interface

---

## How It Works

This project follows a Retrieval-Augmented Generation (RAG) workflow.

### 1. Document Processing

When PDFs are uploaded:

- Text is extracted from the uploaded files
- The extracted content is split into smaller chunks
- Each chunk is converted into embeddings
- Embeddings are stored in a FAISS vector index for retrieval

### 2. Question Answering

When a user asks a question:

- The query is processed
- Relevant document chunks are retrieved
- Retrieved context is passed to the language model
- The model generates an answer based on the available context

If the primary retrieval pipeline fails, the app falls back to local keyword-based retrieval.

---

## Tech Stack

**Frontend**
- Streamlit

**Backend**
- Python

**AI / LLM**
- Google Gemini
- LangChain

**Retrieval**
- FAISS
- Semantic embeddings

---

## Project Structure

```bash
multipdf_chat/
│
├── app.py                # Main Streamlit application
├── config.py             # Central configuration
├── knowledge_base.py     # PDF processing and vector index creation
├── qa.py                 # Retrieval and question answering logic
├── text_utils.py         # Helper functions
├── ui.py                 # UI rendering
├── styles.py             # Custom styling
```

---

## Installation

Clone the repository:

```bash
git clone <your-repository-url>
cd Multi_PDFs_AI-main
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Environment Setup

Create a `.env` file in the project directory:

```env
GOOGLE_API_KEY=your_api_key_here
```

You can generate a Gemini API key from Google AI Studio.

---

## Running the Application

If running from inside the `multipdf_chat` folder:

```bash
streamlit run app.py
```

If running from the project root:

```bash
streamlit run multipdf_chat/app.py
```

---

## What I Learned

Working on this project helped me understand:

- how Retrieval-Augmented Generation works
- document chunking and preprocessing
- embeddings and semantic similarity search
- vector databases like FAISS
- grounding LLM responses using retrieved context
- handling fallback logic for better reliability

---

## Current Limitations

Some current limitations:

- response quality depends on document quality and retrieval relevance
- large PDFs may increase processing time
- keyword fallback is less accurate than vector similarity search
- this is a prototype/learning implementation, not production deployment

---

## Future Improvements

Things I would improve next:

- source citation highlighting in responses
- better reranking for retrieval quality
- persistent chat history
- authentication
- deployment support
- performance optimization for larger document sets

---

## Note

This project was built as a learning-focused implementation using open-source tools and frameworks, with modifications and experimentation to better understand RAG system design.