# Leukemia Gene Expression Analysis

This repository contains a Jupyter Notebook project that analyzes gene expression data to differentiate between Acute Myeloid Leukemia (AML) and Acute Lymphoblastic Leukemia (ALL). The analysis includes a classification model, model interpretation, unsupervised clustering, and visualization of results.

## Overview

The project performs the following tasks:
- **Classification Model**: Uses an interpretable logistic regression model to predict leukemia type (AML vs. ALL) from gene expression data. The model is trained on a training set and evaluated on an independent test set.
- **Model Interpretation**: Analyzes the model coefficients to identify the most influential genes for each class. The visualization displays the top 5 genes for AML (with positive coefficients) and the top 5 genes for ALL (with negative coefficients), with labels formatted as `row_number FirstWordOfDescription`.
- **Unsupervised Clustering**: Applies k-means clustering (without class labels) to group samples into two clusters, evaluates clustering purity, and discusses the relevance of such techniques in gene expression analysis.
- **Visualization**: Provides colorful visualizations, including a horizontal bar chart for influential genes and a colorful confusion matrix.

## Data

The project uses the following files:
- **`data_set_ALL_AML_train.csv`**: Training dataset containing gene expression values and associated gene information.
- **`data_set_ALL_AML_independent.csv`**: Independent test dataset for evaluating the classification model.
- **`actual.csv`**: Contains the true class labels for the samples.

*Note: The dataset is pre-normalized, and the pre-processing steps include removing non-numeric columns and transposing the data so that each row represents a sample.*

## Requirements

The project is implemented in Python 3.12 and requires the following packages:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `jupyter`

A `requirements.txt` file is included with the exact package list.
