# Evaluating Chess Endgame Positions Using Neural Networks and Symmetry Transformations

Bachelor Thesis – Artificial Intelligence  
Johannes Kepler University Linz  
Author: Kilian Pockenauer  
Supervisor: Univ.-Prof. Dr. Johannes Fürnkranz  
February 2026  

---

## Overview

This project investigates whether neural networks can learn to evaluate and compare chess endgame positions purely from spatial board representations — without handcrafted heuristics, search algorithms, or embedded engine logic.

The work focuses on supervised learning using perfect Distance-to-Mate (DTM) labels derived from Gaviota tablebases.  
Three model families are implemented and evaluated:

- **Single-Position Regression Model** (predicting normalized DTM)
- **Siamese Classification Model** (predicting which of two positions is better)
- **Siamese Regression Model** (predicting continuous relative advantage)

A symmetry-aware preprocessing pipeline is used to eliminate redundant positions and improve learning efficiency.

---

## Key Contributions

- Full endgame data generation pipeline with legality filtering
- Integration of Gaviota tablebases for perfect ground truth labels
- Canonical symmetry reduction (full and half symmetric modes)
- CNN-based encoder architecture for board geometry learning
- Pairwise Siamese architectures for relative evaluation
- Threshold-based and neural post-classification for regression models
- Cross-endgame transfer experiments
- Error magnitude analysis beyond simple classification accuracy

---

## Supported Endgames

The following endgames are implemented:

- KRK
- KRKP
- KPK
- KQKR
- KPKP
- KNKP

For large endgames, datasets are capped at 1,000,000 positions.

---

## Project Structure
