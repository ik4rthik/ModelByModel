# 🚀 RAG with MongoDB Atlas Vector Search

<p align="center">
  <img src="https://img.shields.io/badge/Retrieval-Augmented%20Generation-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/MongoDB-Vector%20Search-green?style=for-the-badge&logo=mongodb"/>
  <img src="https://img.shields.io/badge/LangChain-RAG-success?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Groq-LLM-orange?style=for-the-badge"/>
</p>

---

## 📖 Overview

This project demonstrates how to build a complete **Retrieval-Augmented Generation (RAG)** pipeline using **MongoDB Atlas Vector Search** instead of traditional vector databases like ChromaDB.

The workflow includes:

- 📄 Loading PDF documents
- ✂️ Splitting documents into chunks
- 🧠 Generating vector embeddings
- 💾 Storing embeddings in MongoDB Atlas
- 🔍 Semantic retrieval using MongoDB Vector Search
- 🤖 Answer generation using Groq LLM

---

# 🛠 Tech Stack

<p align="center">

<img src="https://skillicons.dev/icons?i=python,mongodb,vscode,git,github" />

<br><br>

<img src="https://img.shields.io/badge/LangChain-121212?style=for-the-badge&logo=chainlink&logoColor=white"/>

<img src="https://img.shields.io/badge/SentenceTransformers-FF6F00?style=for-the-badge"/>

<img src="https://img.shields.io/badge/Groq-000000?style=for-the-badge"/>

<img src="https://img.shields.io/badge/PyMongo-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>

<img src="https://img.shields.io/badge/PyPDF-DC143C?style=for-the-badge"/>

</p>

---

# ⚙️ Workflow

```text
                PDF
                 │
                 ▼
          PyPDF Loader
                 │
                 ▼
 RecursiveCharacterTextSplitter
                 │
                 ▼
 Sentence Transformer Embeddings
                 │
                 ▼
        MongoDB Atlas
        (Store Vectors)
                 │
                 ▼
    MongoDB Vector Search
                 │
                 ▼
 Retrieve Relevant Chunks
                 │
                 ▼
         Prompt Creation
                 │
                 ▼
            Groq LLM
                 │
                 ▼
        Generated Answer
```

---

# 📂 Project Structure

```text
📦 RAG_MongoDB_Vector_Search
│
├── rag.ipynb
├── README.md
├── requirements.txt
└── sample.pdf
```

---

# ✨ Features

- ✅ PDF Document Loading
- ✅ Intelligent Text Chunking
- ✅ Sentence Transformer Embeddings
- ✅ MongoDB Atlas Vector Storage
- ✅ Vector Search Index Creation
- ✅ Semantic Similarity Search
- ✅ Retrieval-Augmented Generation
- ✅ Groq LLM Integration

---

# 📚 Concepts Covered

- Retrieval-Augmented Generation (RAG)
- Vector Embeddings
- Semantic Search
- MongoDB Atlas Vector Search
- Document Chunking
- Vector Databases
- Prompt Engineering
- Context Retrieval
- Large Language Models (LLMs)

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/ik4rthik/ModelByModel.git
```

Move into the project

```bash
cd RAG_MongoDB_Vector_Search
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file.

```env
MONGO_URI=your_mongodb_connection_string

GROQ_API_KEY=your_groq_api_key
```

---

# 💬 Example Query

```
What is MongoDB Vector Search?
```

### Output

```
MongoDB Atlas Vector Search performs semantic search by comparing
vector embeddings instead of exact keyword matching...
```

---

# 🎯 Learning Outcomes

By completing this project, I learned:

- How vector embeddings are generated
- Why document chunking is important
- How MongoDB Atlas stores embeddings
- Creating MongoDB Vector Search Indexes
- Semantic Retrieval
- Integrating an LLM with retrieved context
- Building a complete RAG pipeline from scratch

---

# 🔮 Future Improvements

- Hybrid Search (BM25 + Vector Search)
- Metadata Filtering
- Multiple PDF Support
- Streamlit UI
- FastAPI Backend
- Conversation Memory
- Docker Deployment

---

# 👨‍💻 Author

**Karthik S**

Computer Science & Engineering (Artificial Intelligence)

Building AI projects one model at a time 🚀
