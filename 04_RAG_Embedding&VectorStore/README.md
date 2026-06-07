# 🧠 04_RAG_Embeddings_VectorStore

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Sentence Transformers](https://img.shields.io/badge/SentenceTransformers-Embeddings-green)
![ChromaDB](https://img.shields.io/badge/ChromaDB-Vector%20Database-purple)

---

## 🚀 About

This project explores how text chunks are converted into vector embeddings and stored inside a vector database.

After completing document loading and chunking, I learned how modern RAG systems transform text into numerical representations that can later be used for semantic retrieval.

---

# 🔄 Pipeline Implemented

```text
PDF Documents
      ↓
Document Loaders
      ↓
Text Chunks
      ↓
SentenceTransformer
      ↓
Embeddings (Vectors)
      ↓
ChromaDB Vector Store
```

---

# 🧠 What I Learned

## 📌 Embeddings

Embeddings convert text into numerical vectors that capture semantic meaning.

Example:

```text
Chunk:
"Computer networks allow devices to communicate"

Embedding:
[-0.12, 0.44, ..., 0.83]
```

Each chunk is transformed into a dense vector representation.

---

## 📌 Sentence Transformers

Used:

```python
all-MiniLM-L6-v2
```

to generate embeddings from document chunks.

Concepts learned:

* Text Embeddings
* Vector Representations
* Semantic Meaning
* Embedding Models

---

## 📌 Vector Databases

Used ChromaDB to store:

* Embeddings
* Chunk Content
* Metadata
* Unique Document IDs

This enables efficient storage of vectorized knowledge.

---

# ⚙️ Technologies Used

* Python
* Sentence Transformers
* ChromaDB
* NumPy
* Jupyter Notebook

---


# 🔍 Key Concepts Explored

✅ Text Embeddings

✅ Sentence Transformers

✅ Vector Representations

✅ ChromaDB Collections

✅ Metadata Storage

✅ Unique Document IDs

✅ Vector Databases

---

# 🎯 Next Step

* Query Embeddings
* Similarity Search
* Retrieval Pipeline
* Semantic Search
* Retriever Systems

---

## 📌 Part of My ModelByModel AI Learning Journey

Learning RAG systems step by step by understanding each component before building a complete retrieval pipeline.
