---
title: "Domain-Specific RAG Pipeline"
date: 2024-06-01
image:
  filename: "work-project1.png"
  preview_only: false
summary: "Built a production-grade RAG pipeline for aerospace maintenance documentation, combining dense vector search with BM25 retrieval and a domain-specific semantic layer to support operations analysts."
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
- Designed hybrid retriever combining dense vector search (pgVector) with BM25 lexical matching
- Fine-tuned embedding models on aerospace maintenance documentation for domain alignment
- Query expansion optimized for domain-specific terminology
- Fallback chains ensuring graceful degradation under edge cases

**Semantic Business Layer**
- Built component lifecycle management system tracking maintenance states and dependencies
- Ontology-driven classification enabling compliance reporting and maintenance planning
- Integration with existing maintenance tracking systems

**Deployment & Infrastructure**
- Deployed CloudFoundry-hosted applications with GitLab CI/CD pipelines
- Monitoring dashboards tracking query performance and system health
- Collaborated with Agile teams using Jira

## Technologies Used

- **NLP & ML:** PyTorch, Transformers (HuggingFace), LangChain, RAG frameworks
- **Data Infrastructure:** PostgreSQL, pgVector
- **Deployment:** CloudFoundry, Docker, GitLab CI/CD
- **Monitoring:** Prometheus, Grafana

