---
title: "Domain-Specific RAG Pipeline"
date: 2024-06-01
image:
  filename: "work-project1.png"
  preview_only: false
summary: "Built a production-grade RAG pipeline for aerospace maintenance documentation, combining hybrid retrieval and domain-specific semantic modeling to reduce service cycle time for operations analysts."
tags:
  - rag-systems
  - nlp
  - retrieval
  - aerospace
---

## Domain-Specific RAG Pipeline

**Industry/Domain:** Aerospace & Defense

**My Role:** Data Scientist & AI Engineer

**Timeline:** Feb 2022 – Present

## Key Contributions

**RAG Pipeline Architecture**
- Designed hybrid retrieval combining dense vector search with lexical matching for aerospace maintenance documentation
- Fine-tuned embedding models and query expansion for domain-specific terminology
- Built retrieval behavior around operational analyst workflows rather than generic document search

**Semantic Business Layer**
- Mapped component lifecycle relationships into a queryable business layer for maintenance operations
- Structured maintenance states and dependencies so downstream workflows could reason over them consistently

**Deployment & Scale**
- Introduced Dask for scalable pipeline execution beyond single-machine capacity
- Operationalized Docker and CloudFoundry with GitLab CI/CD for reproducible deployment
- Coordinated delivery across data science and engineering through Jira and Azure DevOps

## Technologies Used

- **NLP & ML:** PyTorch, Transformers, LangChain
- **Data Infrastructure:** PostgreSQL, pgVector, Dask
- **Deployment:** Docker, CloudFoundry, GitLab CI/CD
- **Collaboration:** Jira, Azure DevOps
