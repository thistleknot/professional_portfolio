---
title: "Soft Policy Optimization: Reasoning Model Training"
date: 2026-03-15
external_link: "https://github.com/thistleknot/spo-reasoning-training-regimen"
summary: "Complete pipeline for generating synthetic reasoning datasets and training Qwen3.5-0.6B models with soft policy optimization. Three-phase workflow: synthetic dataset generation (LLM-powered triplet extraction), QLoRA fine-tuning, and SPO confidence calibration. Demonstrates production infrastructure for efficient reasoning models."
tags:
  - reasoning-models
  - policy-optimization
  - qwen
  - efficient-ai
  - training-infrastructure
---

## Soft Policy Optimization: Reasoning Model Training

Complete production pipeline for building reasoning models through three phases: synthetic dataset generation, QLoRA fine-tuning, and SPO confidence calibration.

### Three-Phase Architecture

**Phase 1: Synthetic Dataset Generation**
- Extracts structured reasoning from quotes dataset
- Generates triplets (subject | predicate | object) with evidence tags
- Produces pedagogical ordering: Non-Entailed (negatives) → Entailed (positives) → Throughline (summary)
- Supports multiple LLM backends: GPT-4, Qwen, Claude, HuggingFace models, or manual templates
- Confidence tags are NOT training labels — they emerge during inference

**Phase 2: QLoRA Fine-Tuning**
- Base model: Qwen3.5-0.6B (efficient, reasoning-capable)
- 4-bit quantization for 8GB VRAM efficiency
- Configurable rank, learning rate, epoch scheduling
- Multi-GPU support with gradient accumulation
- WandB/TensorBoard monitoring of training curves

**Phase 3: SPO Confidence Optimization**
- Learns accurate confidence calibration using downstream task rewards
- Reward signal: correctness × confidence (only high-confidence correct outputs rewarded)
- Bridges supervised fine-tuning and pure RL
- Ensures model is confident when right, uncertain when wrong

### Technical Insights

Soft policy optimization uses soft constraints with learnable thresholds rather than binary rejection, preventing training instability while maintaining tighter control than standard supervised fine-tuning.

The key design principle: **confidence is emergent**, not a training label. This enables:
- Separation of structure learning from calibration
- Better transfer to new tasks
- Interpretable confidence scores (confidence ≈ actual accuracy)
- Avoidance of confidence overfitting to training data

### Data Format: Pedagogical Ordering

Training data follows Non-Entailed → Entailed → Throughline structure because:
1. **Negative inference first** — Model learns what's irrelevant
2. **Contrastive learning** — Discriminate true from false facts  
3. **Better convergence** — Explicit negatives improve final performance

### Results

Model achieves improved reasoning trajectory on validation set while maintaining inference efficiency, demonstrating feasibility of SOTA training techniques on resource-constrained architectures.

**Repository**: Full source code, documentation, training scripts, and data format specifications available on GitHub.

