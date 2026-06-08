# 🧠 06_RAG_LLM_Integration

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Groq](https://img.shields.io/badge/Groq-LLM-orange)
![ChromaDB](https://img.shields.io/badge/ChromaDB-Vector%20Database-purple)
![Sentence Transformers](https://img.shields.io/badge/SentenceTransformers-Embeddings-green)
![RAG](https://img.shields.io/badge/RAG-End%20to%20End-red)

---

## 🚀 About

This project completes the core Retrieval-Augmented Generation (RAG) workflow by integrating an LLM with the retrieval pipeline.

The system retrieves relevant document chunks from a vector database, combines them with the user's query, constructs a prompt, and generates a context-aware response using an LLM.

---

# 🔄 Complete RAG Pipeline

```text
PDF Documents
      ↓
Document Loading
      ↓
Chunking
      ↓
Embeddings
      ↓
ChromaDB Vector Store
      ↓
Retriever
      ↓
User Query
      ↓
Query Embedding
      ↓
Top Relevant Chunks
      ↓
Prompt Construction
      ↓
LLM (Groq)
      ↓
Generated Answer
```

---

# 🧠 What I Learned

## 📌 Retrieval-Augmented Generation (RAG)

Instead of sending only the user query to the LLM:

```text
Question
   ↓
LLM
```

RAG provides relevant context:

```text
Question
    +
Retrieved Context
        ↓
       LLM
```

This helps the model generate more informed answers.

---

## 📌 Prompt Construction

Built prompts dynamically using:

```text
Context:
[Retrieved Chunks]

Question:
[User Query]

Answer:
```

This allows the LLM to answer using retrieved knowledge rather than relying solely on its training data.

---

## 📌 Context Injection

Learned how retrieved chunks are combined into a single context block before being passed to the model.

Example:

```text
Retrieved Chunk 1
Retrieved Chunk 2
Retrieved Chunk 3
        ↓
Combined Context
        ↓
LLM
```

---

## 📌 LLM Integration

Integrated a Groq-hosted language model to generate final responses.

Responsibilities of the LLM:

* Understand the query
* Read retrieved context
* Generate a relevant answer
* Use retrieved knowledge as reference

---

# ⚙️ Technologies Used

* Python
* LangChain
* Groq
* ChromaDB
* Sentence Transformers
* NumPy
* Jupyter Notebook

---

# 🔍 Key Concepts Explored

✅ Prompt Engineering

✅ Context Injection

✅ Query Processing

✅ Retrieval Pipeline

✅ LLM Integration

✅ Context-Aware Generation

✅ Retrieval-Augmented Generation

✅ End-to-End RAG Workflow

---

# 📊 Example Flow

```text
User Query:
"What is Regression?"

        ↓

Retriever finds relevant chunks

        ↓

Context is assembled

        ↓

Prompt is created

        ↓

LLM generates answer

        ↓

Final Response
```

---

# 🎯 Learning Outcome

Through this project, I understood how retrieval systems and language models work together to form a complete RAG application.

I learned how retrieved context can be injected into prompts, enabling LLMs to generate responses grounded in external knowledge rather than relying solely on pretrained information.

---

## 📌 Part of My ModelByModel AI Learning Journey

Building AI systems from first principles by understanding every component of the RAG pipeline—from document ingestion to retrieval and LLM-powered answer generation.
