# DLAI-project

# VQ-VAE a posteriori with Geodesic Quantisation

## Overview
This project revisits Vector-Quantised Variational Autoencoders (VQ-VAEs) and tests
whether a geometry-aware distance metric can improve codebook usage and
reconstruction quality.

* **Baseline:** Euclidean $k$-means on latent vectors from a β-VAE trained on MNIST.  
* **Proposed:** Isomap embedding to approximate geodesic distances, followed by
  $k$-means in the embedded space.  
* **Comparison:** reconstruction BCE, codebook utilisation, cluster statistics,
  UMAP visualisations.

  ## Requirements
Python 3.10 or later.

| Package            | Tested version |
|--------------------|----------------|
| torch              | 2.2.0+cu118    |
| torchvision        | 0.17.0         |
| scikit-learn       | 1.3.2          |
| umap-learn         | 0.5.5          |
| matplotlib         | 3.8.4          |

Install with:

```bash
pip install -r requirements.txt
```
You can run the code in Google Colab
