# Analysis of Cryptocurrencies
Domain 		  : Unsupervised Machine Learning

Techniques	: Clustering using K-means, Ploting using hvplot

Application	: Investment analysis

## Purpose of Analysis:
- The goal of this analysis is to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system  for anyone interested in a new investment in Crypto Currency Market.

## Tools:
Languages           : Python

Tools               : Anaconda, Jupyter Notebook

Libraries           : pandas, hvplot, sklearn-StandardScaler, PCA, KMeans

## Methods and Results:
#### Processing of Data:
- The pre processing involves cleaning of dataset with pandas. 
- The initial dataset is not ideal for working with Machine Learning models as they have both text and numeric values. 
- So get_dummies() function was used to transform data to create variables for text features.

<img width="534" alt="image" src="https://user-images.githubusercontent.com/94877067/167275473-126d80a1-bff4-4c43-b4c1-45a14cdd2de8.png">

- The data was scaled using StandardScaler()
- The data dimension was reduced to three principal componenets using PCA

<img width="163" alt="image" src="https://user-images.githubusercontent.com/94877067/167275400-0b556b34-32d4-4030-b350-06e68fa5da78.png">

- Elbow curve was created using hvplot to make an educated guess on the number of clusters/ best number for K

<img width="502" alt="image" src="https://user-images.githubusercontent.com/94877067/167275763-a74595e9-9faa-421d-b5d7-b3905caa42ee.png">

- The best K value was determined to be 4 from the Elbow Curve.
- The data was clustered using KMeans

- The tradable crypto currencies were grouped in to 4 clusters based on Algorithm used for trading, Proof type (Proof of stake is a type of consensus mechanism used to validate cryptocurrency transactions, Total Coins mined and Total coin supply.

<img width="523" alt="image" src="https://user-images.githubusercontent.com/94877067/167275805-040c2d46-285a-4702-bed7-82dc22b5c21d.png">

- A 2D scatter was created to visualize the clustering of trading cryptocurrency by class for Total Coin Supply and Total Coins Mined
- The results show that majority of the coins were in cluster 0 and 3

<img width="518" alt="image" src="https://user-images.githubusercontent.com/94877067/167276164-07975bcf-21c7-4efe-879e-dae7f6d03258.png">








