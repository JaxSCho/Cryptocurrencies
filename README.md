# Cryptocurrencies

## Project Overview
Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. We helped Martha create a report that includes what cryptocurriences are on the trading market and how they could be grouped to create a classification system for this investment.

## Summary

The following deliverables include:

1. Preprocessing the Data for Principal Component Analysis (PCA) using Pandas:
    - Keep all cryptocurrencies that are being traded and mined
    - Remove rows that have at least 1 null values
    - Drop the IsTrading and CoinName columns that won't be used on the clustering algorithm
    - Create dummy variables for the two text features: Algorithm and ProofType
    - Use StandardScaler to standardized the features

2. Reducing Data Dimensions Using PCA algorithm to three principal components

3. The K-means algorithm is used to cluster the cryptocurrencies using the PCA data:
    - Create an elbow curve using hvPlot to find the best value for K
    - Predict K clusters of the cryptocurrencies' data
    - Create new DataFrame including predicted clusters and cryptocurrencies features

4. Visualizing Cryptocurrencies Results:
    - Plot a 3D scatter plot of the clusters - each data point shows the CoinName and Algorithm on hover
    - Create a table of 532 tradable cryptocurrencies using the hvplot.table() function
    - Create new DataFrame including the scaled data 
    - Create hvplot scatter plot - Total Coins Mined vs Total Coined Supply - by classification

## Resources
- Data Sources: crypto_data.csv
- Languages: Jupyter Notebook