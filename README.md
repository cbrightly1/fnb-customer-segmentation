# fnb-customer-segmentation
This project used a Kmeans after PCA model to segment retail customers to optimize marketing efforts. The segmentation was performed on 3 main types of accounts (consumer, small business, and mixed) on 2 data levels (customer and household) for 6 models total. The same process outlined below was performed on each of the models. For simplicity's sake, only one model is included in this repo. 

When the model repeatedly returned a single cluster, the project goals had to be updated. In the end, the model was used to prove the customer's homogenous characteristics. The findings were presented to the Chief Marketing Officer and influenced the bank's marketing strategies and initiatives. Developed in Jupyter Notebook with Python for FNB.

## Segmentation Process
1. We used SQL Studio Management Services to extract the data (half a million data points and nearly a hundred variables). 
2. The pandas package was used to clean the data. This includes pulling the SQL data, merging multiple tables together, replacing null values, and consolidating demographic variables.
3. The variables were standardized and the categorical variables were dummied out.
4. We determined the optimal number of PCA components using a cumulative variance graph.
5. The number of clusters were determined using the silhouette coefficient and inertia. The average silhouette score and inertia were calculated for every cluster size from 2 to 8, then the silhouette score was calculated for every data point. 

## Project Highlights
- We also explored the cluster centers to try and explain the clusters. But the addition of the principal components made the interpretation difficult.
- While my teammate and I were surprised about the homogeneous characteristics, our management team was not surprised with the results.
- The data was not on the same timeline which could have an effect on the results. But
- The SQL script and overall data preparation process was very complicated. It took us 7 full working days to get a reliable data set and it had to be updated several times throughout the process.
