# Multi-format-Document-Embedding-Pipeline
Efficiently transform multi-format documents (.txt, .pdf, .docx, .csv) into high-quality vector representations using E5 embeddings for downstream NLP tasks.

- This project demonstrates converting APA 7th edition writing guidelines into vector embeddings for semantic search and QA tasks.

## ✨ Task Goal
To build a reliable preprocessing and embedding pipeline that:
- Supports various document formats
- Applies semantic-aware chunking and embedding
- Outputs a searchable vector database using FAISS

## 🪛 Methodology
1. **Document Loading**: Supports `.txt`, `.pdf`, `.docx`, and `.csv` formats via `langchain-community` loaders.
2. **Text Chunking**: Uses `RecursiveCharacterTextSplitter` to preserve contextual integrity.
3. **E5 Embedding**: Customizes `HuggingFaceEmbeddings` to align with the E5 format (`"passage: "` and `"query: "` prefixes).
4. **Vector Database**: Stores chunk embeddings using FAISS, with optional local saving and compression.

## 🟢 Results
- Successfully embedded and indexed in four documents
- 1. APA 7_Reference Guide.pdf
  2. APA 7_Common Reference Examples.pdf
  3. APA 7_Numbers & Statistics.pdf
  4. APA 7_Student Paper Setup Guide.pdf
- Produced a reusable FAISS database in `.zip` format
- Verified cross-format compatibility (TXT, PDF, DOCX, CSV)

## 🌷 Application
The generated vector store can be plugged into:
- Personalized learning content format instruction and recommendation
- Retrieval-Augmented Generation (RAG) systems
- Semantic search tools
- Chatbots with contextual memory

