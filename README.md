# Clustering Techniques

## Introduction
Clustering is a technique used in fault diagnosis to identify groups of unlabelled data points based on their similarities and differences. The aim is to group together similar data points and assign them a label or category based on these similarities. The following clustering techniques are commonly used:

- K-Means Clustering
- Gaussian Clustering
- Hierarchical Clustering
- Clustering after Discrete Wavelet Transform approach
- Dynamic Time Warping based Clustering 

## Pre-requisites
- Jupyter Notebook

## Libraries required
- python==3.9.13
- pandas==1.5.3
- sklearn==0.0.post1
- matplotlib==3.7.0
- scipy==1.8.1
- seaborn==0.11.2
- pyarrow==11.0.0
- fastcluster==1.2.6
- numpy==1.23.1
- pywt==1.4.1
- dtw==1.4.0
- tslearn==0.5.3.2
- fastdtw==0.3.4

## Dataset
The dataset used for clustering should be pre-processed and saved as a file. The path to the file should be updated in the `datasource_config.py` file.

## Running the clustering algorithm notebooks
1. Update the path to the pre-processed dataset in the `datasource_config.py` file.
2. Run each of the Jupyter notebooks for the different clustering algorithms.
3. Check the crosstab heatmaps and scatter plots generated in each notebook to understand the cluster label assignment and how they are distributed amongst different fault labels.
