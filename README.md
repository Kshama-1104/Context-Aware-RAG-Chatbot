# 🤖 Context-Aware RAG Chatbot

🚀 A production-ready **Retrieval-Augmented Generation (RAG) chatbot** with conversational memory, built using **LangChain (LCEL), OpenAI, FAISS, and Streamlit**.

💡 Designed to reduce hallucinations and deliver accurate, context-aware responses from external knowledge sources.

---

## 📌 Overview

Large Language Models (LLMs) are powerful but often:

- Hallucinate incorrect information  
- Lack awareness of external/private data  
- Fail in multi-turn conversations  

This project solves these problems by implementing a **Context-Aware RAG pipeline** that retrieves relevant information and generates grounded, reliable answers while maintaining conversation history.

---

## 🎯 Objectives

- Build a **context-aware chatbot** using RAG  
- Enable accurate Q&A over external knowledge  
- Maintain **multi-turn conversational memory**  
- Reduce hallucinations via document grounding  
- Use **modern LangChain v1.0+ (LCEL)**  
- Provide a **secure & user-friendly UI**

---

## 🏗️ System Architecture

### 🔹 Core Components

- **Frontend:** Streamlit (interactive chat UI)
- **Document Loader:** WebBaseLoader (Wikipedia source)
- **Text Splitter:** RecursiveCharacterTextSplitter
- **Vector Store:** FAISS
- **Embeddings:** OpenAI (`text-embedding-3-small`)
- **LLM:** OpenAI (`gpt-4o-mini`)
- **Pipeline:** LCEL-based RAG chain

---

## ⚙️ Workflow

1. 🔑 User enters OpenAI API key  
2. 📄 Data is loaded from external source  
3. ✂️ Text is split into chunks  
4. 🧠 Embeddings are created & stored in FAISS  
5. ❓ Query is reformulated (if context exists)  
6. 🔍 Relevant chunks are retrieved  
7. 🤖 LLM generates grounded response  
8. 💬 Chat history is maintained  

---

## ✨ Key Features

- 🧠 Context-aware multi-turn conversations  
- 📚 Retrieval-Augmented Generation (RAG)  
- ⚡ Modern LangChain LCEL implementation  
- 🔐 Secure API key handling  
- 🧹 Clear chat history option  
- 🚀 Cached vector store for performance  

---

## 💼 Use Cases

- Enterprise knowledge assistant  
- Customer support chatbot  
- Internal document search system  
- AI-powered research assistant  

---

## 🛠️ Tech Stack

| Category        | Technology |
|----------------|------------|
| Language       | Python 3.10+ |
| Frontend       | Streamlit |
| Framework      | LangChain v1.0+ |
| Vector DB      | FAISS |
| LLM & Embedding| OpenAI |

---

## 📦 Installation & Setup

```bash
# Clone repository
git clone https://github.com/Kshama-1104/context-aware-rag-chatbot.git
cd context-aware-rag-chatbot

# Create virtual environment
python -m venv venv

# Activate environment
source venv/bin/activate     # Linux/Mac
venv\Scripts\activate        # Windows

# Install dependencies
pip install -r requirements.txt

# Run app
streamlit run app.py
---
