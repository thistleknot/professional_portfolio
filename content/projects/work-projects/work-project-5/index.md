---
title: "High-Impact Document Drafting Acceleration"
date: 2024-09-01
image:
  filename: "work-project5.png"
  preview_only: false
summary: "Developed a RAG-based system to reduce flow time for drafting high-impact critical documents, saving 400 engineering hours per quarter through structured JSON schema output and hallucination detection."
tags:
  - rag-systems
  - hallucination-detection
  - aerospace
---

## High-Impact Document Drafting Acceleration

**Industry/Domain:** Aerospace & Defense

**My Role:** Data Scientist & AI Engineer

**Timeline:** 2022 – Present

## Impact

- **400 engineering hours saved per quarter** through automated drafting assistance

## Key Contributions

**RAG Pipeline for Critical Documentation**
- Built retrieval-augmented generation pipeline grounding drafts in authoritative source documentation
- Reduced manual research and drafting flow time by surfacing relevant precedents and regulatory references

**Structured Output & Validation**
- Enforced JSON schema on LLM outputs to ensure consistent, parseable document structure
- Schema validation catches malformed responses before they reach downstream consumers

**Hallucination Detection**
- Implemented hallucination detection layer comparing generated claims against retrieved source passages
- Flags low-confidence outputs for human review, preventing ungrounded content from entering drafts

## Technologies Used

- **LLM & Retrieval:** RAG pipeline, vector search, LangChain
- **Output Control:** JSON schema enforcement, structured generation
- **Reliability:** Hallucination detection, grounding verification
- **Infrastructure:** Python, GitLab CI/CD, CloudFoundry
