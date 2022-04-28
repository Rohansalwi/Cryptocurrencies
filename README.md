# Cryptocurrencies
## Overview
The purpose of this project was to analyze a dataset from many alternative cryptocurrencies to spot trends that make anyone want to invest in them. The problem with cryptos is that the most common ones, like bitcoin or ethereum, are becoming unaffordable for the common public so will be using unsupervised machine learning to see if we can spot any trends that result in opportunities of these altcoins.
## Software
Python 3.7
scikit-learn 0.24
hvPlot 0.7.0
Plotly 4.14.3
## Results
Following the preprocessing and cleaning phase we have a total of 532 tradable cryptocurrencies.


## Clustering Cryptocurrencies using K-Means - Elbow Curve
We don't know what would be the output of the analysis so we are using unsupervised machine learning to identify clusters of the cryptocurrencies.
We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10.

![Screen Shot 2022-04-28 at 3 47 53 PM](https://user-images.githubusercontent.com/96554223/165833899-af5d421e-5592-42c5-8225-40e3899c16a8.png)


The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies.

## Visualizing Cryptocurrencies Results
### 3D-Scatter plot with clusters

![Screen Shot 2022-04-28 at 3 49 02 PM](https://user-images.githubusercontent.com/96554223/165834400-229e7e17-f07c-4f1f-a83c-a02147f89b3a.png)


This 3-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to three principal components.

### Tradable Cryptocurrencies Table

![Screen Shot 2022-04-28 at 3 54 04 PM](https://user-images.githubusercontent.com/96554223/165834772-107c4a8e-1fa2-4d5e-b1cd-7c37177a0ad2.png)

Most of the cryptocurrencies are part of class #0 and #1.
The snapshot above shows that BitTorrent is the only cryptocurrency in class #2.

### 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply

![Screen Shot 2022-04-28 at 3 50 33 PM](https://user-images.githubusercontent.com/96554223/165834884-36f4bb30-e3c2-47dc-b01d-cbeb084ac51c.png)

Plotting the scatter plot from two cryptocurrency features directly does not efficiently segregate the different classes. Then using the PCA algorithm is the right method for better visualizations.

## Summary
We have identified the classification of 532 cryptocurrencies based on similarities of their features.
Particularities of each group need to be analyzed to determined their performance and potential interest for the investment bank's clients.
