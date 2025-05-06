# Clustering-with-K-Means

##  Wholesale Customers Clustering using K-Means

This project applies "K-Means Clustering" to group wholesale customers based on their annual spending on various product categories. 

---

### Steps

#### 1. Load and Visualize Dataset

- The dataset is loaded using pandas.
- Basic histograms are created to visualize the distribution of each feature (e.g., Fresh, Milk, etc.).

#### 2. Fit K-Means and Assign Cluster Labels

- The features are standardized using `StandardScaler` to bring all values to the same scale.
- K-Means is applied (with an initial choice of `k=3` clusters).
- Each customer is assigned to a cluster, and the cluster labels are stored in the dataset.

#### 3. Use the Elbow Method to Find Optimal K

- The Elbow Method is used to determine the best number of clusters.
- A plot of inertia vs. number of clusters (K) helps visualize the optimal K where the curve starts to bend ("elbow point").

#### 4. Visualize Clusters with Color-Coding

- PCA (Principal Component Analysis) is used to reduce data to 2 dimensions for visualization.
- A scatter plot shows how customers are grouped into clusters using different colors.
- Cluster centroids are marked with red ‘X’ symbols.

#### 5. Evaluate Clustering Using Silhouette Score

- The Silhouette Score is calculated to measure how well each customer fits within its cluster.
- Score ranges from -1 to 1 (higher is better).
- This helps confirm if the chosen number of clusters is appropriate.

---

