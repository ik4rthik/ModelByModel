## ✂️ Text Chunking

After loading documents, I explored text chunking using LangChain's
`RecursiveCharacterTextSplitter`.

### Why Chunking?

Large documents cannot be directly sent to an LLM due to context limits.
Chunking breaks documents into smaller pieces that can be embedded,
stored, and retrieved efficiently.

### Experiment

| Chunk Size | Overlap | Observation |
|------------|----------|-------------|
| 1000 | 200 | Few chunks created |
| 100 | 20 | More granular chunks |

### Pipeline

Raw Document
↓
Document Loader
↓
Document Object
↓
RecursiveCharacterTextSplitter
↓
Chunks
↓
Embeddings
↓
Vector Database
