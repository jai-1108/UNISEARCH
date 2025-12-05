# 🌌 UNISEARCH — Multimodal Academic Search Engine  
### 🔍 *Search across lectures, transcripts, keyframes, and research papers in one unified system.*

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Colab](https://img.shields.io/badge/Run%20on-Colab-yellow?logo=googlecolab)
![FAISS](https://img.shields.io/badge/FAISS-Vector%20Search-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## ✨ Overview
UNISEARCH is a multimodal search engine built to make academic content easily discoverable.  
It connects **video transcripts**, **keyframes**, **images**, and **research papers** using modern embedding models like **BGE** and **SigLIP**, combined with **FAISS**, **BM25**, and **cross-encoder reranking**.

The project is split into two phases for clarity, modularity, and reproducibility.

---

## 🧠 Key Features
- Multimodal retrieval (text, images, keyframes, PDFs)  
- Dense embeddings using **BGE** for text and **SigLIP** for images  
- Scalable vector search powered by **FAISS**  
- Hybrid retrieval with **BM25 + vector search**  
- Cross-encoder reranking for higher-quality results  
- Transcript–keyframe alignment for richer context  
- Evaluation block for Recall@k, Precision@k, ranking quality  


---

## ⚙️ How the System Works

### 🔷 Phase 1 — Data, Embeddings, and Indexing
This phase prepares everything the search engine needs:
- Extracts lecture transcripts and keyframes  
- Cleans and chunks text into meaningful units  
- Generates BGE text embeddings  
- Generates SigLIP visual embeddings  
- Builds FAISS vector indices  
- Stores metadata, manifests, and ID mappings  

**Output:** A complete multimodal vector database.

---

### 🔶 Phase 2 — Query Engine, Ranking, Evaluation
This phase delivers the search experience:
- Accepts text queries  
- Performs dense retrieval (FAISS)  
- Performs sparse retrieval (BM25)  
- Combines them using hybrid scoring  
- Reranks results with a cross-encoder  
- Evaluates with Recall@k, Precision@k, ranking metrics  

**Output:** Ranked multimodal results optimized for relevance.

---

## ⭐ Why UNISEARCH Stands Out
- It is a **full end-to-end ML pipeline**, not a toy example  
- Handles **messy real academic data** across modalities  
- Implements **industry-standard retrieval components**  
- Designed to be modular, debuggable, and extensible  
- Includes a clean evaluation suite for rapid experimentation  

---

## 🎯 Potential Use Cases
- Academic content search  
- Multimodal retrieval-augmented generation (RAG)  
- Lecture and course material exploration  
- Research paper discovery  
- Video content understanding systems  

---

## 🚀 Future Improvements
- Temporal video embeddings for long-context understanding  
- Domain-specific fine-tuning of BGE / SigLIP  
- Hallucination-resistant RAG summarization  
- Streamlit or web-based interface for interactive search  

---

## 🛠️ Getting Started
1. Open **Phase 1** notebook in Colab → run preprocessing, embedding, and indexing  
2. Open **Phase 2** notebook → load FAISS indexes and manifests  
3. Run queries and test multimodal retrieval with evaluation metrics  

---

## 📬 Contact
If you’d like to discuss multimodal retrieval, embeddings, or search engine design, feel free to reach out.

