# Trusted but Tainted

**Official implementation of:**

**Trusted but Tainted: Enrolment Perturbations that Undermine Morphing Attack Detection and Face Recognition**

Accepted at **ICPR 2026**.

---

## Overview

This repository provides a complete pipeline for evaluating the robustness of face recognition systems against adversarial enrolment perturbations in the context of:

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

## Status

Repository under active preparation.

Code, notebooks, evaluation scripts, and reproducibility artifacts are being released.

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

## Installation

Clone the repository:

```bash
git clone https://github.com/dhammadipdk/Trusted_but_Tainted.git
cd Trusted_but_Tainted
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Tested using:

* Python 3.10+
* PyTorch
* CUDA-enabled GPU (recommended)

---

## Notebook Overview

| Notebook                                | Description                                                    |
| --------------------------------------- | -------------------------------------------------------------- |
| 00_setup.ipynb                          | Environment setup, dependency installation, repository cloning |
| 01_generate_perturbations.ipynb         | Generation of adversarial enrolment perturbations              |
| 02_morph_generation.ipynb               | Morph generation using Greedy, MIPGAN-II, and UBO              |
| 03_embedding_and_delta_embeddings.ipynb | Embedding extraction and delta embedding generation            |
| 04_gmap_evaluation.ipynb                | GMAP evaluation                                                |
| 05_dmad_evaluation.ipynb                | D-MAD evaluation                                               |

---

## Datasets

The experiments reported in the paper were conducted using:

* FERET
* FRGC

A demonstration subset of the datasets is included in the downloadable demo inference package available under **Artifact Downloads**.

Users interested in reproducing the full experimental pipeline may use the provided artifacts or obtain the original datasets from their respective sources.

Please cite the original dataset publications when using this work.

---

## Face Recognition Systems

The following face recognition systems are used:

* AdaFace
* ArcFace
* MagFace
* ElasticFace
* EdgeFace

The demonstration inference package includes all model checkpoints required to execute the released notebooks.

Users may therefore run the complete demonstration pipeline directly from the downloadable artifacts without separately obtaining model checkpoints.

Please cite the original model repositories and publications when using this work.

---

## Reproducibility

Two reproduction modes are supported.

### Full Reproduction

Execute all notebooks in order:

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

### Fast Reproduction

Precomputed artifacts are provided to reproduce the reported GMAP and D-MAD results without rerunning the complete pipeline.

---

## Precomputed Artifacts

To facilitate reproducibility, precomputed artifacts are provided.

### Full Experimental Artifacts

The following archives contain embeddings generated for the complete experimental setup:

* Embeddings.zip
* Embeddings_Diff.zip

These artifacts allow direct reproduction of:

* GMAP results
* D-MAD results

without recomputing perturbations, morphs, and embeddings.

### Demo Inference Package

A lightweight demonstration package is also provided.

The package contains:

* FERET Dataset
* FRGC Dataset
* Face recognition checkpoints
* External repositories
* Generated perturbations
* Morphs
* Embeddings
* Delta embeddings
* GMAP results
* D-MAD results

allowing users to execute the complete pipeline with minimal setup and without separately downloading datasets or model checkpoints.

---

## Artifact Downloads

### Full Experimental Artifacts

Embeddings.zip

[Google Drive Link]

Embeddings_Diff.zip

[Google Drive Link]

### Demo Inference Package

Demo_Working_Directory.zip

[Google Drive Link]

---

## Acknowledgements

This repository builds upon the following face recognition systems:

* AdaFace
* ArcFace
* MagFace
* ElasticFace
* EdgeFace

and uses the following datasets:

* FERET
* FRGC

The demo inference package includes the resources required to execute the released notebooks.

We gratefully acknowledge the authors of the original face recognition systems, morph generation frameworks, and datasets used throughout this work.

Please cite the corresponding publications and repositories when using this repository.

---

## Citation

If you use this repository, please cite:

```bibtex
@inproceedings{kamble2026trusted,
  title={Trusted but Tainted: Enrolment Perturbations that Undermine Morphing Attack Detection and Face Recognition},
  author={Kamble, Dhammadip and others},
  booktitle={International Conference on Pattern Recognition (ICPR)},
  year={2026}
}
```

The citation entry will be updated after publication.

---

## Contact

Dhammadip Kamble

GitHub: https://github.com/dhammadipdk
