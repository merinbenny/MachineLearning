Gaussian Mixture Model (GMM) Face Generation & Anomaly Detection — Description
This code trains a Gaussian Mixture Model (GMM) on the Olivetti Faces dataset after applying PCA dimensionality reduction for efficiency. The workflow includes:

Stratified splitting of the dataset into train/validation/test sets

PCA compression to preserve 97% variance while reducing dimensionality

Training a GMM with 40 components (one per identity)

Sampling new faces from the learned mixture model and reconstructing them back to 64×64 images

Creating modified (anomalous) samples by rotating, flipping, and darkening original faces

Computing log‑likelihood scores for both normal and modified samples

Comparing likelihoods to show how GMMs identify anomalies: normal faces have high likelihoods, while altered faces produce extremely low scores

This project demonstrates how GMMs can be used for unsupervised generative modeling and probabilistic anomaly detection on facial image data.
