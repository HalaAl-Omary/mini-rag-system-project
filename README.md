# Mini RAG System Project

This is a simple **Retrieval-Augmented Generation (RAG) system** built in Python using Hugging Face Transformers.  
It uses a **retriever model (SentenceTransformer)** to find relevant information and a **generator model (DistilBERT)** to extract answers.

---

## Features
- Retrieves relevant context from a knowledge base
- Extracts precise answers using a QA model
- Allows adding new knowledge and testing it
- Self-assessment included to check retrieval and generation accuracy

---

## Requirements
- Python 3.8+
- torch
- transformers
- sentence-transformers

Install libraries via:
```bash
pip install torch transformers sentence-transformers
