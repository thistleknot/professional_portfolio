---
title: Chess AI with Deep Q-Learning & Russian Doll MCTS
date: 2024-01-01
external_link: "https://github.com/thistleknot/chess-deep-q"
summary: "RL-based chess engine using Deep Q-Networks with progressive Monte Carlo Tree Search. Combines value-based learning with tree search for strategic decision-making."
tags:
  - Reinforcement Learning
  - Deep Q-Learning
  - MCTS
  - PyTorch
---

## Overview

A chess AI that learns from its mistakes using Deep Q-Learning and Russian Doll Monte Carlo Tree Search (MCTS). The agent progressively narrows its search space, combining value-based learning with tree search for strategic board decisions.

## Key Features

- **Deep Q-Network**: PyTorch-based value network for board state evaluation
- **Russian Doll MCTS**: Progressive action narrowing from all legal moves to top-K candidates
- **Experience Replay**: Stable training with priority sampling
- **Target Network**: Periodic synchronization to reduce divergence
- **Hyperparameter Tuning**: Automated Optuna search for learning rates, discount factors, epsilon decay
- **Visualization**: Training plots for loss, reward, and win rate convergence

## Architecture

- **Q-Network**: Multi-layer neural network that learns board state → action value mapping
- **Action Space**: Legal moves narrowed via MCTS tree expansion
- **Reward Signal**: Chess outcomes (win/loss/draw) + intermediate board evaluation
- **Exploration**: Epsilon-greedy strategy with decay schedule

## Technical Stack

- PyTorch (neural networks)
- Chess library (game logic & move validation)
- Optuna (hyperparameter optimization)
- NumPy (numerical computation)

## Links

- [GitHub Repository](https://github.com/thistleknot/chess-deep-q)

