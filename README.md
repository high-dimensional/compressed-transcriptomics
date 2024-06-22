# Compressed Transcriptomics
![abstract](assets/graphical_abstract.png)

This repository open sources code and model weights for automated optimum compression of brain transcriptomic data using deep autoencoding, as detailed in our [article](https://arxiv.org/abs/2310.16113).

## Table of Contents
- [What is this repository for?](#what-is-this-repository-for)
- [Why should I use this model?](#why-should-i-use-this-model)
    - [Expressive and accurate compression of transcriptomic data](#expressive-and-accurate-compression-of-transcriptomic-data)
    - [Downstream inference](#downstream-inference)
- [Usage instructions](#usage-instructions)
- [Use queries](#use-queries)
- [Citation](#citation)
- [Funding](#funding)

## What is this repository for?
- The architecture of the brain is too complex to be intuitively surveyable without the use of *compressed representations* that project its variation into a compact, navigable space. 
- The task is especially challenging with high-dimensional data, such as transcriptomic / gene expression data (for example provided by the [Allen Brain Atlas](https://portal.brain-map.org)) where the joint complexity of anatomical and transcriptional patterns demands maximum compression. 
- The **current established practice** is to use standard principal component analysis (PCA), which comes at the cost of *limited expressibility*, which can impact quality of research findings.
- **As an alternative, we here provide the [code](Usage_Tutorial.ipynb) and [model weights](/model_weights) for a series of trained deep autoencoders.**

## Why should I use this model?
### Expressive and accurate compression of transcriptomic data

#### Expressive
![brain](assets/brain_figure.png)
Even when reducing *15,633 gene expression values into merely 2 components*, note the intricate variational structure across autoencoded (AE) representations, especially in comparison to methods such as PCA, kPCA, or NMF.   

#### Accurate
![reconstruction](assets/reconstruction_error.png)
Across a number of possible latent dimensionalities, the autoencoder achieves superior accuracy in reconstructing original source transcriptomic data in comparison to UMAP, PCA, NMF, and kPCA.

*N.B. reconstruction evaluation is not possible with t-SNE.*

### Downstream inference
![prediction](assets/prediction.png)
Deep autoencoders yield superior predictive utility across signalling, microstructural, and metabolic targets in applied machine prediction using transcriptomic data. 

## Usage instructions
In the uploaded [Jupyter Notebook](Usage_Tutorial.ipynb) we provide a tutorial that:
- 1. Overviews running inference to compress transcriptomic data into a latent space of 2,4,8,16,32,64, or 128 dimensions.
- 2. Provides the code and architecture to retrain the a autoencoder for use with other data.

The model weights are open-sourced [here](/model_weights).

## Use queries
Via github issue log or email to j.ruffle@ucl.ac.uk.

## Citation
If using these works, please cite the following [paper](https://arxiv.org/abs/2310.16113):
```
Compressed representation of brain genetic transcription. James K Ruffle, Henry Watkins, Robert J Gray, Harpreet Hyare, Michel Thiebaut de Schotten, Parashkev Nachev. arXiv, 2023. DOI https://doi.org/10.48550/arXiv.2310.16113. 
```

## Funding
The Medical Research Council; The Wellcome Trust; UCLH NIHR Biomedical Research Centre; Guarantors of Brain.
![funders](assets/funders.png)
