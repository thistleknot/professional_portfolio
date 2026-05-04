---
title: "Music Embedding & Clustering System"
date: 2024-11-15
external_link: ""
summary: "UMAP-based music discovery system clustering 751 songs via audio embeddings and metadata. Hierarchical micro/meso/macro clustering with interactive 3D visualization. Genre, artist, and band-size filtering. Real-time similarity-based music recommendations and exploration."
tags:
  - music-information-retrieval
  - embeddings
  - clustering
  - umap
  - interactive-visualization
  - recommendation-system
---

## Music Embedding & Clustering System

Interactive music discovery and recommendation system using high-dimensional audio embeddings projected to 3D space via UMAP. Hierarchical clustering reveals semantic music similarity across 751-song corpus.

### Architecture

**Embedding Pipeline:**
- Audio features extraction (spectral characteristics, temporal structure, perceptual properties)
- Feature normalization and dimensionality reduction
- UMAP projection to 3D space optimized for neighbor preservation and cluster separation

**Hierarchical Clustering:**
- Micro-clusters: Song-level similarity (typically 3-5 songs per cluster)
- Meso-clusters: Genre/style groupings (related artists, similar production)
- Macro-clusters: High-level music categories (Cumbia, Punk, Rock, Pop, Electronic, etc.)

**Interactive Interface:**
- 3D cluster visualization with hover tooltips
- Real-time song search and playback
- Multi-level filtering: Genre, Artist, Band Size
- Dynamic recommendations (find similar songs to current selection)
- Playlist generation from cluster neighborhoods

### Data & Scale

- **Corpus**: 751 songs across diverse genres
- **Dimensions**: High-dimensional embeddings → 3D UMAP projection
- **Hierarchy**: 3 clustering levels enabling exploration at different granularities
- **Metadata**: Genre, artist, year, band composition

### Technical Insights

Music similarity is not purely acoustic — genre, instrumentation, historical context, and artist relationships shape perceived similarity. This system captures both low-level audio properties and high-level semantic relationships through hierarchical clustering.

UMAP's neighbor preservation + cluster separation optimization maintains local song-to-song similarity while separating distinct musical genres — enabling both fine-grained discovery (micro-clusters) and broad browsing (macro-clusters).

### Use Cases

- Music discovery: Explore new songs similar to favorites
- Playlist generation: Generate coherent playlists from cluster neighborhoods
- Music analysis: Visualize genre/artist relationship landscape
- Recommendation: Suggest songs based on current listening context

