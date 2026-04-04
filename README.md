<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,12,20&height=200&section=header&text=Cortex-RAG&fontSize=55&fontColor=fff&animation=twinkling&fontAlignY=38&desc=From%20Embeddings%20to%20Full%20RAG%20Systems%20%E2%80%94%20Built%20From%20Scratch&descAlignY=58&descSize=14" width="100%"/>

[![Python](https://img.shields.io/badge/Python-3.10-f97316?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![SentenceTransformers](https://img.shields.io/badge/SentenceTransformers-Latest-06b6d4?style=for-the-badge&logoColor=white)](https://sbert.net)
[![Status](https://img.shields.io/badge/Status-Active%20Building-22c55e?style=for-the-badge&logoColor=white)]()
[![Notebooks](https://img.shields.io/badge/Notebooks-2%20of%205-f97316?style=for-the-badge&logoColor=white)]()

</div>

---

## What is Cortex-RAG?

This repository is a **hands-on RAG system built from scratch** — every concept explained, every line of code written and understood.

RAG = Retrieval Augmented Generation

It means: instead of asking an LLM to remember everything, we give it the ability to **search a knowledge base** and answer from real retrieved documents.

```
User Query
    ↓
Embed query into vector
    ↓
Search vector database for similar documents
    ↓
Pass retrieved documents + query to LLM
    ↓
LLM generates grounded, accurate answer
```

---

## Repository Structure

```
Cortex-RAG/
├── 01_Embeddings_Basics_to_Advanced.ipynb   ← Start here
├── 02_Netflix_Semantic_Search_Pipeline.ipynb ← Full pipeline
├── 03_Vector_Databases_Chroma.ipynb          ← Coming soon
├── 04_LLM_Response_Generation.ipynb          ← Coming soon
├── 05_Complete_RAG_System.ipynb              ← Final project
├── Netflix_Dataset.csv
├── My_New_Netflix_Dataset.csv
└── README.md
```

---

## Notebooks

### 01 — Embeddings: From Zero to Semantic Search
**What you learn:**

| Concept | Description |
|---------|-------------|
| One-Hot Encoding | Why it fails to capture meaning |
| Embedding Matrix | How dense vectors solve the problem |
| Cosine Similarity | Measure meaning — not just spelling |
| SentenceTransformer | State-of-the-art pretrained embeddings |
| Semantic Search | Ask anything — find meaning not keywords |
| Save to CSV | Persist embeddings for reuse |

**Key insight:** King and Queen are close in embedding space. King and Pizza are far apart. That is how machines understand language.

---

### 02 — Netflix Semantic Search Pipeline
**Full end-to-end pipeline on real data:**

**EDA Dashboard — 6 Charts:**

| Chart | What it shows |
|-------|--------------|
| Pie chart | Movies vs TV Shows split |
| Horizontal bar | Top 10 content-producing countries |
| Genre bars | Most popular genres on Netflix |
| Line chart | Content release growth over years |
| Bar chart | Audience rating distribution |
| Dual line | Movies vs TV Shows trend over time |

**Semantic Search Results:**

| Query | Top Result |
|-------|-----------|
| "Romantic movies" | Ankahi Kahaniya — love stories |
| "Action movies" | Prey — survival thriller |
| "Steven Spielberg" | Jaws — exact director match |
| "Comedy movies" | Relevant comedy titles |
| "Indian content" | Kota Factory, Indian productions |

**Custom vs Sklearn cosine similarity:** Both give identical results. Custom helps you understand the math. Sklearn runs faster at scale.

---

## The RAG Learning Path

```
Week 1  — Notebook 01 + 02 (Embeddings + Semantic Search)
Week 2  — Notebook 03 (Chroma vector database)
Week 3  — Notebook 04 (HuggingFace LLM response)
Week 4  — Notebook 05 (Complete RAG pipeline)
```

---

## Related Repository

This repo builds on top of foundational ML work done in:

**ML with Scikit-Learn** — github.com/ather-ops/ML-with-Scikit-Learn

That repo covers the complete classical ML pipeline:
- End-to-end pipelines for classification and regression
- Feature engineering, EDA, model evaluation
- ROC curves, AUC, confusion matrix, threshold tuning
- Production-ready code patterns

**Cortex-RAG is the next level** — moving from classical ML into modern AI with embeddings and language models.

---

## Prerequisites

```bash
pip install pandas numpy matplotlib seaborn
pip install sentence-transformers scikit-learn
pip install chromadb transformers   # for notebooks 03-05
```

---

## Skills Demonstrated

[![Embeddings](https://img.shields.io/badge/Embeddings-From%20Scratch-f97316?style=flat-square)]()
[![Cosine Similarity](https://img.shields.io/badge/Cosine%20Similarity-Custom%20%2B%20Sklearn-f97316?style=flat-square)]()
[![Semantic Search](https://img.shields.io/badge/Semantic%20Search-Real%20Data-06b6d4?style=flat-square)]()
[![SentenceTransformers](https://img.shields.io/badge/SentenceTransformers-MiniLM-06b6d4?style=flat-square)]()
[![EDA](https://img.shields.io/badge/EDA-6%20Chart%20Dashboard-22c55e?style=flat-square)]()
[![Error Handling](https://img.shields.io/badge/Error%20Handling-Production%20Ready-22c55e?style=flat-square)]()

---

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-ather--ops-f97316?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ather-ops)
[![Live App](https://img.shields.io/badge/Live%20App-Rain%20Predictor-f97316?style=for-the-badge&logo=streamlit&logoColor=white)](https://rain-predictor-app.streamlit.app)
[![ML Scratch](https://img.shields.io/badge/Repo-ML%20from%20Scratch-06b6d4?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ather-ops/Machine-Learning-from-scratch)

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,12,20&height=100&section=footer" width="100%"/>

</div>
