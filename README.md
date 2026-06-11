# Trusted_but_Tainted

Official implementation of:

**Trusted but Tainted: Enrolment Perturbations that Undermine Morphing Attack Detection and Face Recognition**

---

## Overview

This repository provides a complete pipeline for evaluating the robustness of face recognition systems against adversarial perturbations in the context of:

* Differential Morphing Attack Detection (D-MAD)
* Generalized Morph Attack Potential (GMAP)

The framework supports:

* Perturbation Generation
* Morph Generation
* Embedding Extraction
* Delta Embedding Generation
* D-MAD Evaluation
* GMAP Evaluation

---

## Supported Face Recognition Systems

* AdaFace
* ArcFace
* MagFace
* ElasticFace
* EdgeFace

---

## Supported Perturbations

* PGD
* DCT-HF
* DWT-HF
* BPDA-EOT

---

## Supported Morph Generators

* Greedy
* MIPGAN-II
* UBO

---

## Datasets

* FERET
* FRGC

---

## Repository Structure

```text
Trusted_but_Tainted/

├── notebooks/
├── Dataset/
├── models/
├── repos/
├── image-output/
├── Embeddings/
├── Embeddings_Diff/
├── GMAP_Results/
├── DMAD_Results/
├── assets/

├── README.md
├── LICENSE
├── requirements.txt
├── CITATION.cff
└── .gitignore
```

---

## Pipeline

```text
00_setup.ipynb
        ↓
01_generate_perturbations.ipynb
        ↓
02_morph_generation.ipynb
        ↓
03_embedding_and_delta_embeddings.ipynb
        ↓
04_gmap_evaluation.ipynb
        ↓
05_dmad_evaluation.ipynb
```

---

## Status

🚧 Repository under active preparation.

Artifacts, notebooks, and reproducibility resources are being released.

---

## Contact

Dhammadip Kamble
