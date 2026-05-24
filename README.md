# Cortex-RAG

A hands-on repository for building Retrieval Augmented Generation systems from scratch — every concept explained, every line of code written and understood.

RAG means: instead of asking an LLM to remember everything, you give it the ability to search a knowledge base and answer from real retrieved documents. This repository builds that system step by step, starting from what an embedding actually is and ending with a complete working pipeline.

---

## How RAG Works

```
User Query
    ↓
Embed query into a vector
    ↓
Search vector database for similar documents
    ↓
Pass retrieved documents + original query to LLM
    ↓
LLM generates a grounded, accurate answer
```

The key shift from classical ML: the model is no longer memorizing answers during training. It is retrieving relevant context at inference time and reasoning over it.

---

## Repository Structure

```
Cortex-RAG/
├── 01_Embeddings_Basics_to_Advanced.ipynb    # Start here
├── 02_Netflix_Semantic_Search_Pipeline.ipynb  # Full pipeline on real data
├── 03_Vector_Databases_Chroma.ipynb           # Coming soon
├── 04_LLM_Response_Generation.ipynb           # Coming soon
├── 05_Complete_RAG_System.ipynb               # Final project
├── Netflix_Dataset.csv
├── My_New_Netflix_Dataset.csv
└── README.md
```

---

## Notebooks

### 01 — Embeddings: From Zero to Semantic Search

Starts at the beginning and builds up to state-of-the-art embeddings without skipping the fundamentals.

| Concept | What it covers |
|---------|----------------|
| One-Hot Encoding | Why it fails to capture meaning |
| Embedding Matrix | How dense vectors solve the problem |
| Cosine Similarity | Measuring meaning, not spelling |
| SentenceTransformer | Pretrained embeddings with MiniLM |
| Semantic Search | Finding meaning rather than keywords |
| Saving to CSV | Persisting embeddings for reuse |

The core insight: King and Queen are close in embedding space. King and Pizza are far apart. That geometric relationship is how machines represent language meaning.

---

### 02 — Netflix Semantic Search Pipeline

An end-to-end pipeline applied to a real Netflix dataset. Covers exploratory analysis, embedding generation, and semantic search with custom and sklearn cosine similarity implementations side by side.

**EDA covers:** content type split, top producing countries, genre distribution, release year trends, audience ratings, and movies vs TV shows over time.

**Semantic search results on real queries:**

| Query | Top Result |
|-------|-----------|
| "Romantic movies" | Ankahi Kahaniya — anthology love stories |
| "Action movies" | Prey — survival thriller |
| "Steven Spielberg" | Jaws — exact director match |
| "Indian content" | Kota Factory and related productions |

**Custom vs sklearn cosine similarity:** both return identical results. The custom implementation shows the math. The sklearn version shows how it scales. Understanding both matters.

---

### 03 — Vector Databases with Chroma

Coming soon. Covers storing and querying embeddings at scale using ChromaDB rather than in-memory arrays.

### 04 — LLM Response Generation

Coming soon. Connects the retrieval pipeline to a HuggingFace language model to generate answers grounded in retrieved documents.

### 05 — Complete RAG System

The final project. A full pipeline from raw document ingestion to query answering — every component from notebooks 01 through 04 assembled into one working system.

---

## Learning Path

```
Week 1  — Notebooks 01 and 02 (Embeddings and Semantic Search)
Week 2  — Notebook 03 (Chroma vector database)
Week 3  — Notebook 04 (LLM response generation)
Week 4  — Notebook 05 (Complete RAG pipeline)
```

---

## Prerequisites

```bash
pip install pandas numpy matplotlib seaborn
pip install sentence-transformers scikit-learn
pip install chromadb transformers        # required for notebooks 03 to 05
```

---

## Where This Fits

This repository is the next step after classical ML. The foundation work lives in two companion repositories.

| Repository | What it covers |
|------------|----------------|
| [Machine-Learning-from-scratch](https://github.com/ather-ops/Machine-Learning-from-scratch) | Linear regression, logistic regression, gradient descent — pure NumPy |
| [ML-with-Scikit-Learn](https://github.com/ather-ops/ML-with-Scikit-Learn) | Same algorithms using sklearn, pipelines, and real projects |
| Cortex-RAG (this repo) | Embeddings, semantic search, vector databases, and LLM integration |

The three repositories together form a complete path from ML fundamentals to modern AI systems.

---

## License

MIT. Use freely.

---

## Author

[ather-ops](https://github.com/ather-ops)
