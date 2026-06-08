# 🧠 05_RAG_VectorRetriever

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Sentence Transformers](https://img.shields.io/badge/SentenceTransformers-Embeddings-green)
![ChromaDB](https://img.shields.io/badge/ChromaDB-Vector%20Database-purple)
![RAG](https://img.shields.io/badge/RAG-Retrieval%20Pipeline-orange)

---

## 🚀 About

This project explores the retrieval layer of a Retrieval-Augmented Generation (RAG) system.

Starting from document chunks, I generated embeddings, stored them in a vector database, and implemented a retriever that can find the most relevant chunks based on semantic similarity.

---

# 🔄 Retrieval Pipeline

```text
PDF Documents
      ↓
Document Loaders
      ↓
Text Chunks
      ↓
Embedding Model
      ↓
Vector Embeddings
      ↓
ChromaDB Vector Store
      ↓
User Query
      ↓
Query Embedding
      ↓
Similarity Search
      ↓
Top Relevant Chunks
```

---

# 🧠 What I Learned

## 📌 Embeddings

Generated dense vector representations using:

```python
all-MiniLM-L6-v2
```

Each text chunk is transformed into a numerical vector that captures semantic meaning.

---

## 📌 Vector Store

Used ChromaDB to store:

* Document Chunks
* Embeddings
* Metadata
* Unique Document IDs

This enables efficient semantic search across documents.

---

## 📌 Query Embeddings

Learned that user queries must also be converted into embeddings before retrieval.

Example:

```text
User Query
"What is a computer network?"
        ↓
Query Embedding
        ↓
Similarity Search
```

---

## 📌 Retriever

Implemented a retriever that:

* Generates query embeddings
* Searches the vector database
* Retrieves the most relevant chunks
* Returns content with metadata and similarity scores

---

# ⚙️ Technologies Used

* Python
* Sentence Transformers
* ChromaDB
* NumPy
* Scikit-Learn
* Jupyter Notebook


---

# 🔍 Key Concepts Explored

✅ Embedding Models

✅ Vector Representations

✅ ChromaDB Collections

✅ Metadata Management

✅ Query Embeddings

✅ Similarity Search

✅ Semantic Retrieval

✅ Top-K Retrieval

---

# 📊 Example Retrieval Flow

```text
Query:
"What is machine learning?"

      ↓

Retriever searches vector database

      ↓

Top Results:

1. Machine Learning Introduction
2. Supervised Learning Concepts
3. Neural Network Fundamentals
```

---

# 🎯 Learning Outcome

Through this project, I understood how modern RAG systems retrieve relevant information using embeddings, vector databases, and similarity search before passing context to an LLM.

---

## 📌 Part of My ModelByModel AI Learning Journey

Building Retrieval-Augmented Generation systems step by step by understanding every layer of the retrieval pipeline from document ingestion to semantic retrieval.
