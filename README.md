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

1. **Preprocess the data**:
Run Single_File_Creation_and_encoding.ipynb
2. **Run clustering**
Run kmeans.ipynb using the full_data.csv file output from the previous step
3. **Run LSTM**
Run LSTM.ipynb using the cluster dataframes created at the previous step

## Authors

- Oscar LEGOUPIL
- Dmitri LERBUN
- Sandra NGUEMOGNE
