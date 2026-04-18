# Biomedical Syntactic Pattern Recognition
### Clustering DNA Sequences via Structural Grammar
**CSE424: Pattern Recognition - Group 15**

## 🧬 Project Overview
Traditional machine learning models in bioinformatics often rely on converting DNA into numerical features (e.g., GC content percentages). However, DNA is fundamentally a language governed by syntax and structural order. 

This project proposes a novel architecture to classify genetic patterns based purely on sequence grammar using **Levenshtein Edit Distance** and **Agglomerative Hierarchical Clustering**.

## ⚙️ System Architecture Pipeline
This repository contains the ongoing implementation of a 4-phase pipeline:
1. **Raw DNA Data Ingestion:** Sourcing 8,000+ genomic sequences (Human, Chimpanzee, Dog).
2. **Distance Matrix Computation:** Calculating $O(N^2)$ Levenshtein distances to measure syntactic similarity.
3. **Agglomerative Clustering:** Applying bottom-up hierarchical grouping to construct genetic taxonomies.
4. **Evaluation:** Validating structural groups against ground-truth gene families using the Adjusted Rand Index (ARI).

## 🚀 Current Status (Work-in-Progress)
- [x] Phase 1: Data Extraction & Environment Setup
- [x] Phase 2: GPU-Accelerated Matrix Computation (In Progress via Google Colab)
- [ ] Phase 3: Clustering Analysis
- [ ] Phase 4: Final Evaluation

*Note: Due to the computational complexity of Phase 2, the N-by-N distance matrix is being cached locally using RAPIDS cuDF/cuML on cloud GPUs.*
