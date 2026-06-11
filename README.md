# Trusted but Tainted Enrollment

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

The notebooks were developed and tested using:

* Python 3.10+
* PyTorch
* CUDA-enabled GPU (recommended)

---

## Notebook Overview

| Notebook                                | Description                                                    |
| --------------------------------------- | -------------------------------------------------------------- |
| 00_setup.ipynb                          | Environment setup, dependency installation, repository cloning |
| 01_generate_perturbations.ipynb         | Generation of RRPR perturbations                               |
| 02_morph_generation.ipynb               | Morph generation using Greedy, MIPGAN-II, and UBO              |
| 03_embedding_and_delta_embeddings.ipynb | Embedding extraction and delta embedding generation            |
| 04_gmap_evaluation.ipynb                | GMAP evaluation                                                |
| 05_dmad_evaluation.ipynb                | D-MAD evaluation                                               |

---

## Datasets

This work uses the following face datasets:

* FERET
* FRGC

The datasets are not redistributed through this repository.

Please obtain the datasets from their respective providers and place them under:

```text
Dataset/
```

The expected dataset structure is documented in:

```text
Dataset/README.md
```

---

## Face Recognition Systems

The following face recognition systems are used:

* AdaFace
* ArcFace
* MagFace
* ElasticFace
* EdgeFace

Model checkpoints are not redistributed through this repository.

Expected model locations are documented in:

```text
models/README.md
```

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

Precomputed artifacts are provided to reproduce the paper tables without rerunning the complete pipeline.

---

## Precomputed Artifacts

To facilitate reproducibility, precomputed artifacts are provided.

### Full Evaluation Artifacts

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

* FERET subset
* FRGC subset
* Generated perturbations
* Morphs
* Embeddings
* Delta embeddings
* Evaluation results

allowing users to execute the complete pipeline on a reduced benchmark.

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

## Citation

If you use this repository, please cite:

```bibtex
@inproceedings{kamble2026trusted,
  title={Trusted but Tainted},
  author={Kamble, Dhammadip and others},
  booktitle={International Conference on Pattern Recognition (ICPR)},
  year={2026}
}
```

The final citation will be updated after publication.

```




## Status

🚧 Repository under active preparation.

Artifacts, notebooks, and reproducibility resources are being released.

---

## Contact

Dhammadip Kamble
