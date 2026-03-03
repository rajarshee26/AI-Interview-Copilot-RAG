# AI Interview Copilot (RAG-Based)

An intelligent AI Interview Copilot built using Retrieval-Augmented Generation (RAG), FAISS-based semantic search, and LLM-based rubric evaluation.

---

##  Project Overview

This system simulates a technical interview session by:

1. Retrieving relevant interview questions using semantic search
2. Generating structured interview questions using an LLM
3. Evaluating candidate answers using rubric-based LLM scoring
4. Producing a final performance summary

---

## Architecture

User Query
↓
SentenceTransformer Embeddings
↓
FAISS Vector Search
↓
LLM Question Generation (FLAN-T5)
↓
Candidate Answer
↓
LLM-Based Rubric Evaluation
↓
Final Performance Report

---

##  Tech Stack

- Python
- SentenceTransformers
- FAISS (Vector Database)
- HuggingFace Transformers
- FLAN-T5 Base (Lightweight LLM)
- Google Colab

---

## Evaluation Metrics

Each answer is evaluated across:

- Technical Depth (1–5)
- Clarity (1–5)
- Confidence (1–5)

Evaluation is grounded using expected key answer points from the dataset.

---

## Dataset

Synthetic structured dataset containing:

- Skill-tagged interview questions
- Topic classification
- Difficulty levels
- Expected key answer points
- Follow-up questions

---

##  Future Improvements

- Use larger instruction-tuned models (e.g., Mistral-7B)
- Hybrid retrieval (BM25 + dense vectors)
- Streamlit-based UI
- Fine-tuned evaluation model
- Interview session analytics dashboard

---

##  Why RAG?

Instead of relying solely on pretrained LLM knowledge, this system grounds generation using a curated interview question dataset, improving relevance and reducing hallucination.
