# Clustering for Fault Diagnosis

## Introduction
Clustering is a technique used in fault diagnosis to identify groups of unlabelled data points based on their similarities and differences. The aim is to group together similar data points and assign them a label or category based on these similarities. The following clustering techniques are used in these Jupyter notebooks:

- K-Means Clustering : `Kmeans_clustering.ipynb`
- Gaussian Clustering : `Gaussian_clustering.ipynb`
- Hierarchical Clustering : `Hierarchical_clustering.ipynb`
- Clustering after Discrete Wavelet Transform approach : `Wavelet_transform_clustering.ipynb` 
- Dynamic Time Warping based Clustering : `DTW_clustering.ipynb`

## Pre-requisites
- Jupyter Notebook

## Libraries required
- python==3.9.13 `pip install python==3.9.13`
- pandas==1.5.3 `pip install pandas==1.5.3`
- sklearn==0.0.post1 `pip install sklearn==0.0.post1`
- matplotlib==3.7.0 `pip install matplotlib==3.7.0`
- scipy==1.8.1 `pip install scipy==1.8.1`
- seaborn==0.11.2 `pip install seaborn==0.11.2`
- pyarrow==11.0.0 `pip install pyarrow==11.0.0`
- fastcluster==1.2.6 `pip install fastcluster==1.2.6`
- numpy==1.23.1 `pip install numpy==1.23.1`
- pywt==1.4.1 `pip install pywt==1.4.1`
- dtw==1.4.0 `pip install dtw==1.4.0`
- tslearn==0.5.3.2 `pip install tslearn==0.5.3.2`
- fastdtw==0.3.4 `pip install fastdtw==0.3.4`

## Dataset
The dataset used for clustering is to be saved in a folder after performing pre-processing. The path to the dataset folder created after pre-processing should be updated by changing the path in the `CLUSTERING_SOURCE_DATA_PATH` variable in `datasource_config.py` file.

## Parquet Files
The folder `parquet files` contain the datasets already created after pre-processing. Feel free to use these parquet files as your dataset created after pre-processing for applying clustering techniques.

## Running the clustering algorithm notebooks
1. Update the path to the pre-processed dataset in the `datasource_config.py` file.
2. Run each of the Jupyter notebooks for different clustering algorithms.
3. Check the crosstab heatmaps and scatter plots generated in each notebook to understand the cluster label assignment and how they are distributed amongst different fault labels.

## Understanding the scatter plots and crosstab heatmaps
Upon assigning a cluster label to each of the data rows, the accuracy of the clustering algorithm is checked by comparing the cluster label assigned to each data row with the actual fault label of that data row by creating a crosstab heat map to decide which cluster label is most likely to resemble which fault label. We can use the crosstab heatmap to understand which of the cluster labels assigned are most uniquely assigned to a true fault label and which of the clusters are most related to one another based on how they are distributed amongst different fault labels. 
