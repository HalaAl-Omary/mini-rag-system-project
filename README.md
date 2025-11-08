# 🧠 Mini RAG System Project

This project implements a **Retrieval-Augmented Generation (RAG)** system built from scratch using Python and Hugging Face Transformers.

The system combines **retrieval** and **generation** to answer user questions based on a specific knowledge base — reducing hallucinations and improving factual accuracy.

---

## 🚀 Features

- **Retrieval**: Finds the most relevant context from a knowledge base using `SentenceTransformer (all-MiniLM-L6-v2)`.  
- **Generation**: Extracts precise answers from that context using `DistilBERT`.  
- **Expandable Knowledge**: You can add new facts to the knowledge base and re-run the embeddings.  
- **Self-Assessment**: Includes an automatic evaluation system to test RAG accuracy.  
- **Interactive Web App**: Built with **Streamlit**, allowing you to ask questions in real time.  
- **Live Access via ngrok**: Host your Streamlit app directly from Google Colab.

---

## 🧩 Tech Stack

- **Python**
- **Hugging Face Transformers**
- **SentenceTransformers**
- **PyTorch**
- **Streamlit**
- **ngrok**

---

## ⚙️ How It Works

1. The retriever encodes all sentences in the knowledge base into semantic embeddings.  
2. When a user asks a question, its embedding is compared using cosine similarity.  
3. The most relevant context is selected.  
4. The generator model uses that context to extract the best possible answer.

---

## 💡 Example

**Input Question:**
> What is the highest mountain?

**Retrieved Context:**
> "Mount Everest is the highest mountain on Earth, located in the Himalayas."

**Generated Answer:**
> Mount Everest

---

## 🌐 Streamlit App

You can run the interactive app inside **Google Colab** with ngrok tunneling enabled.

```python
!streamlit run app.py & npx localtunnel --port 8501
