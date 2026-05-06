---
title: "Labor Optimizer: Min-Max Algorithm for Dwarf Fortress"
date: 2012-06-01
external_link: ""
summary: "3-year collaborative algorithm development for labor optimization in Dwarf Fortress. Modified min-max transform with statistical measures (means, medians). Implemented in C++ and deployed in Dwarf Therapist tool suite."
tags:
  - algorithms
  - optimization
  - game-modding
  - collaborative-research
  - min-max-transform
---

## Labor Optimizer: Min-Max Algorithm for Dwarf Fortress

3-year collaborative effort (with Josh Butgerist) developing novel labor optimization algorithms for the game Dwarf Fortress—a complex simulation with emergent gameplay and massive data.

### Problem

Dwarf Fortress manages 100+ dwarves with 100+ labor categories. Optimal labor assignment requires balancing:
- Skill levels across categories
- Dwarf personality traits (motivation, hazard tolerance)
- Priority of work (mining, crafting, defense, food production)
- Dynamic updates as dwarves level skills or die

Manual spreadsheet-based assignment was tedious and suboptimal.

### Solution

**Modified Min-Max Transform with Statistical Measures**
- Base algorithm: min-max normalization for labor priorities
- Enhancement: incorporated means and medians as additional measures of central tendency
- Result: More robust assignment under uncertainty
- Iterative refinement over 3 years of testing against real gameplay scenarios

### Deployment

- Implemented in C++ 
- Integrated into **Dwarf Therapist** (community tool suite used by thousands)
- Discussed and validated on Bay12Forums with original game developers
- Video demonstration shared with Bay12Forums community

### Impact

Transformed manual labor assignment from hours of spreadsheet work into automated optimization. Community adoption demonstrates real-world utility and algorithmic soundness.

### References

- [Dwarf Therapist GitHub](https://github.com/thistleknot/Labor-Optimizer-Original)
- Bay12Games and Bay12Forums discussions
- YouTube presentation:
  - [Introduction (1:22)](https://www.youtube.com/watch?v=Jz_6hMZahU4&t=82s)
  - [Algorithm walkthrough (6:34)](https://www.youtube.com/watch?v=Jz_6hMZahU4&t=394s)
  - [Demonstration (7:20)](https://www.youtube.com/watch?v=Jz_6hMZahU4&t=440s)

