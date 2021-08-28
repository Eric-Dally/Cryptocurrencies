# Cryptocurrencies

## Overview

The purpose of this project was to explore cryptocurrencies being traded in the market and how they could be grouped to create a classification system for a new investment. In order to do this, I cleaned a crypto currency csv file using python pandas, reduced the dimensions of the data using PCA, grouped the data by using an unsupervized kmeans machine learning algorithm, and created graphs to visualize the results. 

## Analysis

1.) Preprocessing the data:

Initial Dataframe: 

<img width="530" alt="Screen Shot 2021-08-27 at 8 05 07 PM" src="https://user-images.githubusercontent.com/82424250/131201340-78d3fa57-a8f5-440d-b399-f763525cde53.png">

Cleaned DataFrame: In order to run unsupervised algorithms, I had to remove unecessary clumns, filter all null values, and turn all string objects into numerical values.

<img width="1008" alt="Screen Shot 2021-08-27 at 8 07 44 PM" src="https://user-images.githubusercontent.com/82424250/131201392-72e45d57-f460-4e95-af6d-f4b00ed2ef23.png">

2.) Used PCA to reduce the data's dimensions to three principal components:

<img width="931" alt="Screen Shot 2021-08-27 at 8 12 21 PM" src="https://user-images.githubusercontent.com/82424250/131201516-e5b767db-10ac-477b-840d-1cb5ddae414b.png">


## Summary
