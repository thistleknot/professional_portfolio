---
title: "Automated Graph Ontologies from Text"
date: 2024-05-15
external_link: ""
image:
  filename: "automated-graph-ontology.png"
  preview_only: false
summary: "Automatically extract and build interconnected knowledge graphs from unstructured text using a dual-model architecture combining entity extraction with predicate identification. Converts dense academic abstracts and technical documents into queryable semantic networks for enhanced RAG systems."
tags:
  - knowledge-graphs
  - nlp
  - entity-extraction
  - semantic-systems
---

## Automated Graph Ontologies from Text

Building a system to automatically extract structured knowledge graphs from unstructured text, creating machine-readable representations of complex concepts and their relationships.

### Technical Approach

**Entity & Predicate Extraction**
- Uses GLiNER for robust entity extraction identifying anything resembling concepts, entities, or modifying terms
- Decoder-based entity model identifies entities and predicates (modifying terms vs. relationships)
- Encoder model for classifying relations between identified entities

**Graph Construction**
- Cosine similarity merging with synonyms and lemmatization for deduplication
- Builds interconnected graph of boiled-down ideas from source material
- Handles nested list comprehensions and hierarchical relationships

### Current Development

- Successfully extracts high-level entities/predicates from academic abstracts
- Applied to dense technical documents (e.g., deep learning hyperparameter guides)
- Working on predicate connection logic—treating predicates as modifying terms rather than simple relationships
- Unit testing phase with plans to scale across entire text corpora

### Intended Application

Support vector for Retrieval-Augmented Generation (RAG) systems:
- Build semantic business layers from domain-specific text
- Create queryable knowledge structures for maintenance and lifecycle management
- Enable more precise and context-aware information retrieval

### Impact
Demonstrates advanced NLP architecture, semantic system design, and practical application of transformer-based models for knowledge extraction and graph reasoning.
