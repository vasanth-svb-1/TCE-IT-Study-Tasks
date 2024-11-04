# Malware Clustering using GMM and Agglomerative Clustering

This project clusters malware data based on network traffic features using Gaussian Mixture Models (GMM) and Agglomerative Clustering. The clustering provides insights into potential malware families and their behavior, contributing to proactive cybersecurity strategies.

## Table of Contents
- [Introduction](#introduction)
- [Project Objectives](#project-objectives)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Feature Selection](#feature-selection)
- [Clustering Algorithms](#clustering-algorithms)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [Usage](#usage)
---

## Introduction
This project applies unsupervised machine learning techniques to group malware samples into clusters based on network traffic data. By using GMM and Agglomerative Clustering, the project aims to identify malware families, which helps in understanding malware behavior patterns and detecting malicious activities.

## Project Objectives
1. Extract relevant features from network traffic data for clustering.
2. Implement clustering using GMM and Agglomerative Clustering algorithms.
3. Evaluate and visualize clustering results to interpret potential malware families.

## Dataset
The dataset used in this project is the **CTU-IoT-Malware-Capture-8-1conn.log.labeled.csv**. It includes several network features that help in distinguishing malware samples based on their communication patterns. 
> For complete dataset, refer [Dataset](https://www.stratosphereips.org/datasets-iot23)

> **Note**: Ensure appropriate licensing and legal usage of the dataset.

## Methodology
1. **Data Loading and Preprocessing**: The dataset is loaded, and relevant features are selected. Missing values are filled using feature-wise mean imputation.
2. **Feature Scaling**: Standard scaling is applied to the data to normalize feature values.
3. **Dimensionality Reduction**: PCA is applied to reduce features to two principal components for visualization.
4. **Clustering**: Both GMM and Agglomerative Clustering are applied, and results are compared.

## Feature Selection
The following network features are used for clustering:
- `duration`: Connection duration
- `orig_bytes`: Number of bytes from the originator
- `resp_bytes`: Number of bytes from the responder
- `orig_pkts`: Number of packets from the originator
- `resp_pkts`: Number of packets from the responder

## Clustering Algorithms
1. **Gaussian Mixture Models (GMM)**: A probabilistic clustering method that models clusters based on Gaussian distributions.
2. **Agglomerative Clustering**: A hierarchical clustering technique that groups samples based on their similarity.

## Evaluation Metrics
- **Silhouette Score**: Measures how similar a sample is to its own cluster compared to other clusters.
- **Cluster Counts**: Provides insight into the distribution of samples across clusters.

## Results
- **GMM Clustering**: Results include cluster counts, iteration count, and silhouette score.
- **Agglomerative Clustering**: Results include cluster counts and silhouette score.

Both clustering methods are visualized using PCA-reduced data to show cluster separations.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/malware-clustering.git
   cd malware-clustering
