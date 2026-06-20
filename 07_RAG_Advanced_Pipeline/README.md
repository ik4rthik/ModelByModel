# 07_RAG_Advanced_Pipeline

Building an enhanced Retrieval-Augmented Generation (RAG) pipeline with source citation, confidence scoring, and structured responses.

---

## Overview

In this stage, I extended my basic RAG implementation by improving the response generation process.

Instead of returning only an answer, the system now provides:

- Generated Answer
- Retrieved Context
- Source Information
- Confidence Score
- Structured Output Format

This makes the RAG pipeline more transparent and easier to evaluate.

---

## Pipeline Flow

PDF Documents
↓
Document Loading
↓
Chunking
↓
Embedding Generation
↓
ChromaDB Vector Store
↓
Retriever
↓
Similarity Search
↓
Context Creation
↓
LLM (Groq)
↓
Structured Response

---

## Features Implemented

### Source Citation

The pipeline tracks the source of retrieved information using metadata.

Example:

- Source PDF
- Page Number
- Retrieval Rank

This helps verify where the answer originated from.

---

### Confidence Score

A confidence score is calculated using the highest similarity score among retrieved chunks.

```python
confidence = max(
    [doc["similarity_score"] for doc in results]
)
