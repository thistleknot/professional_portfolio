---
title: "Early Semantic Retrieval: Web QA with DPR & Haystack"
date: 2021-10-15
external_link: ""
summary: "Web question-answering system using Dense Passage Retrieval (DPR) before widespread adoption. Semantic search layer for retrieving relevant documents, answer span extraction via BERT. Built on Haystack framework. Demonstrates early adoption of neural retrieval patterns now standard in RAG."
tags:
  - semantic-retrieval
  - dense-passage-retrieval
  - question-answering
  - haystack
  - early-adoption
  - information-retrieval
---

## Early Semantic Retrieval: Web QA with DPR & Haystack

Pre-RAG era implementation of semantic question-answering using Dense Passage Retrieval (DPR). Demonstrates foresight in adopting neural retrieval patterns years before they became industry standard.

### System Design

**Dense Passage Retrieval (DPR):**
- Dual-encoder architecture: question encoder + passage encoder
- Contrastive learning: similar (Q,A) pairs close in embedding space, dissimilar pairs far
- Efficient retrieval: FAISS index for sub-millisecond nearest neighbor search
- Pre-trained on SQuAD, fine-tuned on domain-specific QA pairs

**Answer Extraction:**
- BERT-based span prediction (start/end token positions)
- Confidence scoring via softmax probabilities
- Multi-span answers: ranking candidate spans by relevance

**Haystack Integration:**
- Document store abstraction (Elasticsearch, InMemory, custom backends)
- Retriever → Reader pipeline (retrieve candidate passages → extract answer)
- Prompt template system for LLM-based answer generation
- Caching and batch processing for efficiency

### Timeline & Impact

Implemented in 2021 — before:
- ChatGPT (2022)
- LLaMA + instruction tuning (2023)
- RAG becoming standard practice (2023+)

This project shows early recognition that semantic search beats keyword matching for QA and that embeddings encode semantic meaning better than sparse retrieval.

### Technical Decisions

**Why DPR over BM25?**
- Semantic matching: captures meaning, not just keyword overlap
- Handles lexical variation: "vehicle" matches "car" semantically
- Works across domains without keyword tuning

**Why Haystack over custom?**
- Composable pipeline abstractions
- Multiple backend support
- Community ecosystem
- Extensibility for custom components

### Legacy & Current Relevance

This architecture is the foundation of modern RAG:
- DPR → ColBERT → embedding models (OpenAI, Anthropic)
- Retriever + Generator pattern → now universal in LLM systems
- Early adoption signals understanding of information retrieval fundamentals

