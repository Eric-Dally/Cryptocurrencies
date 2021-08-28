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

3.) Created Elbow curve to determine the statistically appropriate number of clusters to group. 

<img width="836" alt="Screen Shot 2021-08-27 at 8 15 25 PM" src="https://user-images.githubusercontent.com/82424250/131201587-b85e01a3-7774-4f87-84ff-5b4ef21ab06f.png">

4.) Ran K-Means Algorithm for four clusters. Then, I added the clusters to a Dataframe.

<img width="630" alt="Screen Shot 2021-08-27 at 8 17 25 PM" src="https://user-images.githubusercontent.com/82424250/131201681-0e8da5fc-8901-4b9b-9cfa-8787e99a8213.png">

<img width="796" alt="Screen Shot 2021-08-27 at 8 17 39 PM" src="https://user-images.githubusercontent.com/82424250/131201683-301fa92f-91d6-4c92-8569-25f3c6cb0ca1.png">

5.) Visualized the results by graphing 2D and 3D plots using the hvplot import in pandas:

<img width="679" alt="Screen Shot 2021-08-27 at 6 47 31 PM" src="https://user-images.githubusercontent.com/82424250/131201809-768a0923-969a-476b-82af-e8db8508b4ad.png">

<img width="780" alt="Screen Shot 2021-08-27 at 6 53 22 PM" src="https://user-images.githubusercontent.com/82424250/131201813-77aea0dd-0f4b-4946-b002-c0382db05eba.png">


## Summary
