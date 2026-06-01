# 📚 02_RAG_Data_Ingestion

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![LangChain](https://img.shields.io/badge/LangChain-Framework-green)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![VS Code](https://img.shields.io/badge/VSCode-Editor-blue?logo=visualstudiocode)
![PyMuPDF](https://img.shields.io/badge/PyMuPDF-PDF%20Loader-red)

## 🚀 About This Project

This project is part of my **ModelByModel** AI learning journey.

In this project, I explored the **Data Ingestion Pipeline** of RAG (Retrieval-Augmented Generation) systems using LangChain.
Instead of jumping directly into AI chatbots, I focused on understanding how raw documents are converted into structured data for AI applications.

The project includes:

* Loading text files
* Loading PDF documents
* Creating custom `Document` objects
* Working with metadata
* Understanding document ingestion workflows

---

# 🧠 What I Learned

## 📌 Understanding RAG Workflow

I studied the overall flow of a RAG system:

```text
Raw Data
   ↓
Document Loaders
   ↓
Document Objects
   ↓
Text Splitting
   ↓
Embeddings
   ↓
Vector Database
   ↓
Retriever
   ↓
LLM Response
```

---

# 📂 Topics Covered

## ✅ Document Objects

Created custom LangChain `Document` objects using:

* `page_content`
* `metadata`

Example metadata:

* source
* author
* pages
* created date

---

## ✅ Text File Loading

Learned how to:

* Create sample `.txt` files
* Read files using `TextLoader`
* Convert text files into LangChain documents

---

## ✅ Directory Loading

Used `DirectoryLoader` to:

* Load multiple files together
* Process files automatically using glob patterns

---

## ✅ PDF Loading

Used `PyMuPDFLoader` to:

* Read PDF files
* Extract document contents
* Access metadata from PDFs

---

# ⚙️ Tools & Technologies Used

* Python
* LangChain
* Jupyter Notebook
* PyMuPDF
* VS Code

---

# 📁 Project Structure

```bash
02_RAG_Data_Ingestion/
│
├── data/
│   ├── pdf/
│   └── text_files/
│
├── notebook/
│   └── document.ipynb
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

# 📚 Key Concepts Understood

* RAG Architecture
* Data Ingestion Pipeline
* Retrieval Pipeline
* Document Loaders
* Metadata Handling
* Structured Document Processing

---

# ⚠️ Challenges & Insights

During learning, I also understood some practical limitations of RAG systems:

* Higher computational cost
* Retrieval latency
* Poor chunking can reduce answer quality
* Incorrect retrieval can still lead to hallucinated responses

This helped me understand that building a good RAG system is not only about using an LLM, but also about designing an effective retrieval pipeline.

---

# 🎯 Next Learning Goals

* Text Chunking
* RecursiveCharacterTextSplitter
* Embeddings
* Vector Databases
* Similarity Search
* Retriever Pipelines

---

# 📌 Part of My AI Learning Journey

This repository is one step in my journey of learning AI systems practically by building projects and understanding concepts deeply instead of only following tutorials.
