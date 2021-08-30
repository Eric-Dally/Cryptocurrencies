# Cryptocurrencies

## Overview

The purpose of this project was to explore how cryptocurrencies could be grouped to create a classification system for a new investments. In order to do this, I cleaned a crypto currency csv file using python pandas, reduced the dimensions of the data using PCA, grouped the data by using an unsupervized kmeans machine learning algorithm, and created graphs to visualize the results. 

## Analysis

1.) Preprocessing the data:

Initial Dataframe: 

<img width="530" alt="Screen Shot 2021-08-27 at 8 05 07 PM" src="https://user-images.githubusercontent.com/82424250/131201340-78d3fa57-a8f5-440d-b399-f763525cde53.png">

Cleaned DataFrame: In order to run unsupervised algorithms, I had to remove unecessary columns, filter null values, turn all string objects into numerical values, and scale the data.

<img width="1008" alt="Screen Shot 2021-08-27 at 8 07 44 PM" src="https://user-images.githubusercontent.com/82424250/131201392-72e45d57-f460-4e95-af6d-f4b00ed2ef23.png">

2.) Used PCA to reduce the data's dimensions to three principal components:

<img width="931" alt="Screen Shot 2021-08-27 at 8 12 21 PM" src="https://user-images.githubusercontent.com/82424250/131201516-e5b767db-10ac-477b-840d-1cb5ddae414b.png">


3.) Created Elbow curve to determine the statistically appropriate number of clusters to group. 

<img width="836" alt="Screen Shot 2021-08-27 at 8 15 25 PM" src="https://user-images.githubusercontent.com/82424250/131201587-b85e01a3-7774-4f87-84ff-5b4ef21ab06f.png">


4.) Ran K-Means Algorithm for four clusters. Then, I added the clusters to a Dataframe. Side note: In K-means algorithm, each class was defined by creating a centroid for each group. The centroids are the center of the cluster, which captures the points closest to them and adds them to the cluster. 

<img width="630" alt="Screen Shot 2021-08-27 at 8 17 25 PM" src="https://user-images.githubusercontent.com/82424250/131201681-0e8da5fc-8901-4b9b-9cfa-8787e99a8213.png">

<img width="796" alt="Screen Shot 2021-08-27 at 8 17 39 PM" src="https://user-images.githubusercontent.com/82424250/131201683-301fa92f-91d6-4c92-8569-25f3c6cb0ca1.png">


5.) Visualized the results by graphing 2D and 3D plots using the hvplot import in pandas:

<img width="679" alt="Screen Shot 2021-08-27 at 6 47 31 PM" src="https://user-images.githubusercontent.com/82424250/131201809-768a0923-969a-476b-82af-e8db8508b4ad.png">

<img width="777" alt="Screen Shot 2021-08-27 at 8 26 22 PM" src="https://user-images.githubusercontent.com/82424250/131201897-7b853db5-a1a0-43f2-b0bb-19c9568ed7e2.png">


* BitTorrent was the only coin classified into Class 1. It had the highest number of coins mined and one of the highest coin supply.

<img width="556" alt="Screen Shot 2021-08-27 at 8 31 50 PM" src="https://user-images.githubusercontent.com/82424250/131202078-c5510d78-2d8e-44a8-b6c8-aeec7962eb1f.png">

<img width="669" alt="Screen Shot 2021-08-27 at 8 36 57 PM" src="https://user-images.githubusercontent.com/82424250/131202258-4baeefdb-a82d-47e9-86b7-436cae980893.png">


* TurtleCoin tied BitTorrent with a large coin supply while having average number of coins mined. 

<img width="667" alt="Screen Shot 2021-08-27 at 8 35 31 PM" src="https://user-images.githubusercontent.com/82424250/131202242-6a1bc119-ed60-41d9-beff-d0c4ee0c6980.png">



## Summary

 533 cryptocurrencies were randomly classified using the K-Means algorithm. All cryptocurrencies were grouped into 4 clusters and graphs were used to visualize each cluster as well as illustrate the relationship between the Total Coin Supply and the Total Coins Mined. Between these two factors, each coin shared a similar relationship. However, there were two outliers: the BitTorrent coin and the TurtleCoins coin. BitTorrent had the highest number of coins mined reaching 5 times more than the other coins as well as a significantly large coin supply. TurtleCoin had a large coin supply and average number of coins mined. This information is important to the crypto world because it gives one an idea on which coins are worth mining. For example, with mining difficuty set aside, one would not want to mine BitTorrent and TurtleCoins because the market is flooded with them. In other words, the return on selling those coins would be much less than coins that have a low supply and or a small number of coins mined. 

 It is worth mentioning that further research needs to go into evalutating the risk reward of mining each coin. Different coins are harder to mine than others which may be a major factor when deciding which coins to mine. Building on this, the price of each coin fluctuates with the market. On a day by day basis higher priced coins will have more incentive to mine. If I was to continue this project, I would explor a way to factor in these variables into my K-Means model. 
