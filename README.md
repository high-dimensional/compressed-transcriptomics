# Compressed Transcriptomics
![abstract](assets/graphical_abstract.png)

This repository open sources code and model weights for automated optimum compression of brain transcriptomic data using deep auto-encoding, as detailed in the article [article](URL).

## Table of Contents
- [What is this repository for?](#what-is-this-repository-for)
- [Usage instructions](#usage-instructions)
- [Downstream inference](#downstream-inference)
- [Retraining](#retraining)
- [Usage queries](#usage-queries)
- [Citation](#citation)
- [Funding](#funding)

## What is this repository for?
- The architecture of the brain is too complex to be intuitively surveyable without the use of *compressed representations* that project its variation into a compact, navigable space. 
- The task is especially challenging with high-dimensional data, such as gene expression, where the joint complexity of anatomical and transcriptional patterns demands maximum compression. The established practice is to use standard principal component analysis (PCA), whose computational felicity is offset by limited expressivity, especially at great compression ratios. Employing whole-brain, voxel-wise Allen Brain Atlas transcription data, here we systematically compare compressed representations based on the most widely supported linear and non-linear methods—PCA, kernel PCA, non-negative matrix factorisation (NMF), t-stochastic neighbour embedding (t-SNE), uniform manifold approximation and projection (UMAP), and deep auto-encoding—quantifying reconstruction fidelity, anatomical coherence, and predictive utility fork signalling, microstructural, and metabolic targets, drawn from large-scale open-source MRI and PET data. We show that deep auto-encoders yield superior representations across all metrics of performance and target domains, supporting their use as the reference standard for representing transcription patterns in the human brain.

![overview](assets/latent_space.png)
![brain](assets/brain_figure.png)
![representations](assets/representations.png)


## Usage instructions
1. X

![reconstruction](assets/reconstruction_error.png)


## Downstream inference
Downstream prediction


![prediction](assets/prediction.png)

## Usage queries
Via github issue log or email to j.ruffle@ucl.ac.uk

## Citation
If using these works, please cite the following [paper](URL):

*Citation here*

## Funding
The Medical Research Council; The Wellcome Trust; UCLH NIHR Biomedical Research Centre; Guarantors of Brain.
![funders](assets/funders.png)
