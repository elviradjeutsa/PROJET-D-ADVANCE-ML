# Behavioral Analysis of Mutual Insurance Clients to Optimize Portfolio Management

This project uses K-means clustering to create groups of customers to then train LSTM models on, in order to predict their claims.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Reproducing Results](#reproducing-results)
3. [Authors](#authors)

---

## Introduction

The idea of this project is to use the socio-demographic data on clients of a health insurance provider to apply k-means methods to create clusters before training LSTM models on these clusters. Our goal is to make predictions on the monthly medical consumption of individuals, in order to demonstrate the effectiveness of combining clustering and time-series forecasting for healthcare analytics, as well as provide actionable insights for the health insurance provider, in order to improve planning and resource allocation

### Techniques
- **K-Means Clustering**: For grouping customers.
- **PCA**: To visualize the clusters in 2D.
- **LSTM**: To make predictions on customer claims over time

---

## Reproducing Results
1. **Load the data**
Load the three data frames base_ano22, base_ano23, base_24 from the google drive link
3. **Preprocess the data**:
Run Single_File_Creation_and_encoding.ipynb on these 3 dataframes. It outputs a dataframe full_data.csv that has been preprocessed and contains the data from the three years
4. **Run clustering**
Run kmeans.ipynb using the full_data.csv file output from the previous step. It outputs 3 dataframes, one for each cluster
To visualize the clusters and interpret their signification, run caracterisation_classes.ipynb
6. **Run LSTM**
Run LSTM.ipynb using the cluster dataframes created at the previous step




## Authors

- Oscar LEGOUPIL
- Dmitri LEBRUN
- Sandra NGUEMOGNE
