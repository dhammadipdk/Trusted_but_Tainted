# Dataset

The experiments reported in this work were conducted using the following face datasets:

* FERET
* FRGC

A demonstration subset of the datasets required to execute the released notebooks is included in the downloadable Demo Inference Package available under the repository Artifact Downloads section.

## Obtaining the Original Datasets

The original datasets can be obtained from the U.S. National Institute of Standards and Technology (NIST):

### FERET

Face Recognition Technology (FERET)

https://www.nist.gov/programs-projects/face-recognition-technology-feret

### FRGC

Face Recognition Grand Challenge (FRGC)

https://www.nist.gov/programs-projects/face-recognition-grand-challenge-frgc

## Dataset Preprocessing

The experiments do not use the raw FERET and FRGC images directly.

Before executing the perturbation and evaluation pipeline, all images must be:

1. Face detected using MTCNN.
2. FFHQ-style aligned.
3. Cropped and normalized.
4. Stored using the expected directory structure.

The preprocessing pipeline follows:

https://github.com/Blazkowiz47/morph_generator

Only the aligned and cropped images should be used by the subsequent notebooks.

The downloadable Demo Inference Package already contains preprocessed images and therefore does not require this step.

## Citation

Please cite the original FERET and FRGC publications when using this work.

In addition, please cite the original dataset providers and accompanying documentation available through NIST.
