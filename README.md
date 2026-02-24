# Chess Endgame Evaluation with Neural Networks

Bachelor Thesis – Artificial Intelligence  
Johannes Kepler University Linz  
Author: Kilian Pockenauer  
February 2026  

---

## Overview

This project explores whether neural networks can learn to evaluate and compare chess endgame positions purely from board geometry — without search, handcrafted heuristics, or engine logic.

Perfect ground truth labels are obtained from Gaviota tablebases (DTM).  
The focus lies on supervised learning and pairwise comparison using Siamese architectures.

---

## Implemented Models

- **Single-Position Regression** (predict normalized DTM)
- **Siamese Classification** (predict which position is better)
- **Siamese Regression** (predict continuous relative advantage)

All models share a CNN-based encoder operating on multi-channel 8×8 board tensors.

---

## Endgames

- KRK  
- KRKP  
- KPK  
- KQKR  
- KPKP  
- KNKP  

---

## Key Ideas

- Full legality filtering and symmetry reduction
- Canonical board representations
- Validation-optimized thresholding for fair model comparison
- Cross-endgame transfer experiments
- Magnitude-sensitive error analysis

---


## Thesis

The full thesis document is included in this repository.

---

## License

Academic and research use.
