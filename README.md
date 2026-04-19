<<<<<<< HEAD
# RAG-based-MultiPDF-Analyzer
A modular RAG system for multi-document question answering that converts PDFs into embeddings, stores them in a FAISS index, and retrieves relevant context using adaptive query-based retrieval and hybrid re-ranking. Includes a fallback keyword search for robustness.

# 📄 Multi-PDF Research Assistant (RAG-Based QA System)

An AI-powered **Multi-PDF Question Answering System** built using a **Retrieval-Augmented Generation (RAG)** pipeline.
This project demonstrates how large language models can be combined with document retrieval to answer questions based on uploaded PDFs.

---

## 🚀 Features

* 📂 Upload and process **multiple PDF documents**
* 🔍 Semantic search using embeddings
* ⚡ Fast similarity retrieval using FAISS
* 💬 Interactive chat interface
* 🔁 Fallback keyword-based search (when API is unavailable)

---

## 🧠 System Overview

The system follows a **RAG (Retrieval-Augmented Generation)** approach:

### 🔹 Phase 1: Knowledge Base Creation

1. Upload PDFs
2. Extract text from documents
3. Split text into smaller chunks
4. Convert chunks into embeddings
5. Store embeddings in a FAISS index

---

### 🔹 Phase 2: Question Answering

1. User inputs a query
2. Query is converted into an embedding
3. FAISS retrieves relevant chunks
4. Retrieved context is passed to the language model
5. Model generates an answer based on the context

---

## 🛠️ Tech Stack

* **Frontend:** Streamlit
* **LLM & Embeddings:** Google Gemini
* **Vector Search:** FAISS
* **Language:** Python

---

## 📁 Project Structure

```
Multi-PDFs_ChatApp_AI-Agent-main/
│
├── app.py
├── multipdf_chat/
│   ├── config.py
│   ├── knowledge_base.py
│   ├── qa.py
│   ├── text_utils.py
│   ├── ui.py
│   └── styles.py
│
├── assets/
├── tests/
├── requirements.txt
└── LICENSE
```

---

## ⚙️ Installation

```bash
git clone <your-repo-url>
cd Multi-PDFs_ChatApp_AI-Agent-main
pip install -r requirements.txt
```

---

## 🔐 Environment Setup

Create a `.env` file:

```
GOOGLE_API_KEY=your-api-key-here
```

---

## ▶️ Run the Application
=======
# RAG-based-MultiPDF-Analyzer
A modular RAG system for multi-document question answering that converts PDFs into embeddings, stores them in a FAISS index, and retrieves relevant context using adaptive query-based retrieval and hybrid re-ranking. Includes a fallback keyword search for robustness.
# 📄 Multi-PDF Research Assistant (RAG-Based QA System)

An AI-powered **Multi-PDF Question Answering System** built using a **Retrieval-Augmented Generation (RAG)** pipeline.
This project demonstrates how large language models can be combined with document retrieval to answer questions based on uploaded PDFs.

---

## 🚀 Features

* 📂 Upload and process **multiple PDF documents**
* 🔍 Semantic search using embeddings
* ⚡ Fast similarity retrieval using FAISS
* 💬 Interactive chat interface
* 🔁 Fallback keyword-based search (when API is unavailable)

---

## 🧠 System Overview

The system follows a **RAG (Retrieval-Augmented Generation)** approach:

### 🔹 Phase 1: Knowledge Base Creation

1. Upload PDFs
2. Extract text from documents
3. Split text into smaller chunks
4. Convert chunks into embeddings
5. Store embeddings in a FAISS index

---

### 🔹 Phase 2: Question Answering

1. User inputs a query
2. Query is converted into an embedding
3. FAISS retrieves relevant chunks
4. Retrieved context is passed to the language model
5. Model generates an answer based on the context

---

## 🛠️ Tech Stack

* **Frontend:** Streamlit
* **LLM & Embeddings:** Google Gemini
* **Vector Search:** FAISS
* **Language:** Python

---

## 📁 Project Structure

```
Multi-PDFs_ChatApp_AI-Agent-main/
│
├── app.py
├── multipdf_chat/
│   ├── config.py
│   ├── knowledge_base.py
│   ├── qa.py
│   ├── text_utils.py
│   ├── ui.py
│   └── styles.py
│
├── assets/
├── tests/
├── requirements.txt
└── LICENSE
```

---

## ⚙️ Installation

```bash
git clone <your-repo-url>
cd Multi-PDFs_ChatApp_AI-Agent-main
pip install -r requirements.txt
```

---

## 🔐 Environment Setup

Create a `.env` file:

```
GOOGLE_API_KEY=your-api-key-here
```

---

## ▶️ Run the Application
>>>>>>> b95c21e8f4507b6c63441b9fa2272f41f59bb6da

```bash
streamlit run app.py
```

<<<<<<< HEAD
```bash
streamlit run app.py
```

Then open: `http://localhost:8501`

## 🎯 Learning Objectives

This project was developed to understand:
* Retrieval-Augmented Generation (RAG)
* Embeddings and semantic search
* Vector databases (FAISS)
* Integration of LLMs with external data

## Acknowledgment

This project is based on existing open-source RAG implementations and was developed for learning and experimentation purposes.

## ⚠️ Limitations

* Depends on embedding and model quality
* Large PDFs may increase processing time
* Keyword fallback is less accurate than semantic search

## 🔮 Future Improvements

* Better retrieval strategies
* Improved ranking of results
* Enhanced UI and performance
* More advanced query understanding

## 📜 License

This project is licensed under the MIT License.
>>>>>>> b95c21e8f4507b6c63441b9fa2272f41f59bb6da
