# CryptoClustering

## Prepare the Data
-Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

## Find the Best Value for k Using the Original Scaled DataFrame
### Use the elbow method to find the best value for k using the following steps:
- Create a list with the number of k values from 1 to 11.
- Create an empty list to store the inertia values.
- Create a for loop to compute the inertia with each possible value of k.
- Create a dictionary with the data to plot the elbow curve.
- Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

<img width="671" alt="Screenshot 2024-08-02 at 9 09 11 PM" src="https://github.com/user-attachments/assets/428426e9-5773-42be-a07f-b40ec461b2c9">

## Cluster Cryptocurrencies with K-means Using the Original Scaled Data
### Use the following steps to cluster the cryptocurrencies for the best value for k on the original scaled data:
- Initialize the K-means model with the best value for k.
- Fit the K-means model using the original scaled DataFrame.
- Predict the clusters to group the cryptocurrencies using the original scaled DataFrame.
- Create a copy of the original data and add a new column with the predicted clusters.
- Create a scatter plot using hvPlot

<img width="658" alt="Screenshot 2024-08-02 at 9 08 47 PM" src="https://github.com/user-attachments/assets/df04d230-edaf-49a4-9aec-afee8f37b347">

## Optimize Clusters with Principal Component Analysis
- Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components.
- Retrieve the explained variance to determine how much information can be attributed to each principal component.
- Create a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.
  
## Find the Best Value for k Using the PCA Data
### Use the elbow method on the PCA data to find the best value for k using the following steps:
- Create a list with the number of k-values from 1 to 11.
- Create an empty list to store the inertia values.
- Create a for loop to compute the inertia with each possible value of k.
- Create a dictionary with the data to plot the Elbow curve.
- Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

<img width="671" alt="Screenshot 2024-08-02 at 9 09 32 PM" src="https://github.com/user-attachments/assets/50f26a30-1d40-4b54-b63e-51cd25ec7dea">

## Cluster Cryptocurrencies with K-means Using the PCA Data
### Use the following steps to cluster the cryptocurrencies for the best value for k on the PCA data:
- Initialize the K-means model with the best value for k.
- Fit the K-means model using the PCA data.
- Predict the clusters to group the cryptocurrencies using the PCA data.
- Create a copy of the DataFrame with the PCA data and add a new column to store the predicted clusters.
- Create a scatter plot using hvPlot

<img width="664" alt="Screenshot 2024-08-02 at 9 09 53 PM" src="https://github.com/user-attachments/assets/e1b210ed-cf38-43e0-ba8e-8592b9882c8b">

  
