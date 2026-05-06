---
title: "Safety Message Drafting Acceleration"
date: 2024-09-01
image:
  filename: "work-project5.png"
  preview_only: false
summary: "Developed a RAG-based system to reduce flow time for drafting safety messages, using structured JSON schema output and hallucination detection to ensure reliable, grounded generation."
tags:
  - rag-systems
  - safety
  - hallucination-detection
  - aerospace
---

## Safety Message Drafting Acceleration

**Industry/Domain:** Aerospace & Defense

**My Role:** Data Scientist & AI Engineer

**Timeline:** 2022 – Present

## Key Contributions

**RAG Pipeline for Safety Messaging**
- Built retrieval-augmented generation pipeline grounding drafts in authoritative source documentation
- Reduced manual research and drafting flow time by surfacing relevant precedents and regulatory references

**Structured Output & Validation**
- Enforced JSON schema on LLM outputs to ensure consistent, parseable message structure
- Schema validation catches malformed responses before they reach downstream consumers

**Hallucination Detection**
- Implemented hallucination detection layer comparing generated claims against retrieved source passages
- Flags low-confidence outputs for human review, preventing ungrounded content from entering drafts

## Technologies Used

- **LLM & Retrieval:** RAG pipeline, vector search, LangChain
- **Output Control:** JSON schema enforcement, structured generation
- **Safety:** Hallucination detection, grounding verification
- **Infrastructure:** Python, GitLab CI/CD, CloudFoundry
