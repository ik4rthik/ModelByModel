# 📚 02_RAG_Data_Ingestion

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![LangChain](https://img.shields.io/badge/LangChain-RAG-green)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![PyMuPDF](https://img.shields.io/badge/PyMuPDF-PDF%20Loader-red)

## 🚀 About

A beginner-friendly RAG project focused on understanding how documents move through a Retrieval-Augmented Generation pipeline using LangChain.

Instead of directly building a chatbot, this project explores the core foundation of RAG systems:

* Document Loading
* Metadata Handling
* Data Ingestion
* Retrieval Flow Understanding

---

# 🔄 RAG Pipeline Flow

```text id="w0r7zc"
                 ┌────────────────────┐
                 │   Raw Documents    │
                 │ PDF / TXT Files    │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │ Document Loaders   │
                 │ TextLoader         │
                 │ PyMuPDFLoader      │
                 │ DirectoryLoader    │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │ LangChain Document │
                 │ page_content       │
                 │ metadata           │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │ Text Splitting     │
                 │ Chunk Creation     │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │ Embeddings Model   │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │ Vector Database    │
                 └─────────┬──────────┘
                           │
                    User Query
                           │
                           ▼
                 ┌────────────────────┐
                 │ Similarity Search  │
                 │ Retriever Pipeline │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │ Retrieved Context  │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │        LLM         │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │   Final Response   │
                 └────────────────────┘
```

---

# 🧠 What I Learned

* Creating LangChain `Document` objects
* Working with metadata
* Loading `.txt` files using `TextLoader`
* Loading multiple files using `DirectoryLoader`
* Reading PDFs using `PyMuPDFLoader`
* Understanding Data Ingestion Pipeline
* Understanding Retrieval Pipeline
* Understanding why RAG systems can fail
* Understanding how AI systems process external knowledge

---

# ⚙️ Technologies Used

* Python
* LangChain
* Jupyter Notebook
* PyMuPDF
* VS Code

---

# 📂 Project Structure

```bash id="0wqk0s"
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
├── .gitignore
└── README.md
```

---

# 🎯 Next Step

* Text Chunking
* Embeddings
* Vector Databases
* Similarity Search
* Retriever Systems

---

## 📌 Part of My ModelByModel AI Learning Journey

Learning AI by understanding systems deeply instead of blindly following tutorials.

