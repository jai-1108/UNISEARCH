# 🌌 UNISEARCH — Multimodal Academic Search Engine  
### 🔍 *Search across lectures, transcripts, keyframes, and research papers in one unified system.*

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Colab](https://img.shields.io/badge/Run%20on-Colab-yellow?logo=googlecolab)
![FAISS](https://img.shields.io/badge/FAISS-Vector%20Search-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 🔍 UNISEARCH — Cross-Modal Academic Search Engine

UNISEARCH is a production-style multimodal retrieval and RAG system for searching lecture videos, transcripts, images and research papers in a unified pipeline.

## 🚀 What It Does

Text → Text / Image semantic search across lectures and papers

Image → Text retrieval via aligned keyframes

Grounded QA with citations (lecture, timestamp, transcript snippet)

## 🧠 System Architecture
<p align="center"> <img width="5970" height="3570" alt="unisearch_v2_style1_glass" src="https://github.com/user-attachments/assets/8a80a29c-fe58-44f3-b424-4ecbaddad807" />
 </p>

## Pipeline

Multimodal ingestion (videos + PDFs)

Whisper transcription + keyframe extraction

Transcript–keyframe alignment

Hybrid retrieval (BM25 + dense)

FAISS vector search

RAG with citation-backed answers

## 🛠️ Tech Stack

Embeddings: Fine-tuned BGE (text), SigLIP (images)

Indexing: FAISS

RAG: Gemma-4B (grounded generation only)

Backend: FastAPI

UI: Gradio

Evaluation: Recall, MRR, NDCG

## 📊 Evaluation Highlights
<p align="center"> <img width="1470" height="925" alt="Screenshot 2025-12-12 at 5 21 34 PM" src="https://github.com/user-attachments/assets/61598681-d14e-4b77-8b6c-471ed5221953" /> </p>

Corpus: 38,121 academic passages

Test Set: 93 queries

Recall@300 improved 84% → 96% using fine-tuned BGE

Significant gains in MRR and NDCG, especially on harder conceptual queries

## 🔑 Why It Matters

UNISEARCH demonstrates that retrieval quality—not just generation—drives reliable QA.
Fine-tuning the retriever before generation led to more accurate, grounded, and trustworthy answers compared to LLM-only approaches.


## 🛠️ Getting Started
1. Open **Phase 1** notebook in Colab → run preprocessing, embedding, and indexing  
2. Open **Phase 2** notebook → load FAISS indexes and manifests, run queries using Gradio UI and test multimodal retrieval with evaluation metrics  

---

## 📬 Contact
If you’d like to discuss multimodal retrieval, embeddings, or search engine design, feel free to reach out.

