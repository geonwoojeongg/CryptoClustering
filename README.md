# CryptoClustering
A comparison between the results of the StandardScaler() method of data normalization vs. dimensional reduction using Principal Component Analysis (PCA). Each data (normalized and reduced, respectively) is first used to retrive the optimal k-value using the Elbow Curve method, as shown below: 
<img width="750" alt="Screenshot 2023-03-15 at 2 58 41 PM" src="https://user-images.githubusercontent.com/115575880/225416241-d06d8d4e-26a5-41c7-a4d6-b8f74a8f9a49.png">
<img width="771" alt="Screenshot 2023-03-15 at 2 59 10 PM" src="https://user-images.githubusercontent.com/115575880/225416262-1bff17e0-be98-4558-bdfe-6307e844539c.png">

As one can see above, the impact of using fewer features, a.k.a. using PCA to cluster the data using K-Means is to make the clusters more visibly definite, though losing some accuracy. The k-value of the elbow curve (pca) is steeper, supporting more confidence in the claim that the optimal k-value is 4, whereas the optimal k-value of the original elbow curve is not as clear. 

Below are the scatter plots of cluster predictions depicted in scatter plots using original data and PCA: 
<img width="765" alt="Screenshot 2023-03-15 at 2 58 48 PM" src="https://user-images.githubusercontent.com/115575880/225417365-14f71eea-78db-45ba-aeb0-809c0462ac6d.png">
<img width="755" alt="Screenshot 2023-03-15 at 2 59 18 PM" src="https://user-images.githubusercontent.com/115575880/225417377-1a566fc2-03af-49f8-99c4-c847f6935d31.png">

The PCA scatter plot shows a clearer distinction between the clusters, whereas the original scatter plot shows congested areas with different clusters together. Again, PCA loses an insignificant amount of data accuracy while providing distinctiveness of clusters.
