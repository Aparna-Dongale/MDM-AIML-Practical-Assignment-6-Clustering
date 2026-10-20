# Practical Assignment 6: Clustering Algorithms

## Objective
To implement and compare clustering algorithms on a real-world dataset and evaluate clustering quality using appropriate performance metrics.

## Dataset
**UCI Wholesale Customers Dataset**

The dataset contains 440 customer records and annual spending information for six product categories.

Dataset source: https://archive.ics.uci.edu/dataset/292/wholesale+customers

## Algorithms Used
- K-Means Clustering
- Hierarchical Agglomerative Clustering

## Technologies and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Methodology
1. Load the real-world dataset.
2. Select the six annual spending features.
3. Apply log transformation and standardization.
4. Evaluate K-Means for different cluster counts using the Elbow Method and Silhouette Score.
5. Apply K-Means and Hierarchical Clustering.
6. Compare the models using the Silhouette Score and Davies–Bouldin Index.
7. Visualize the clusters using PCA.

## Results
The best tested K-Means configuration used two clusters, with a Silhouette Score of 0.2903.

| Algorithm | Silhouette Score | Davies–Bouldin Index |
|---|---:|---:|
| K-Means | 0.2903 | 1.3515 |
| Hierarchical Clustering | 0.2585 | 1.6004 |

K-Means performed better on both evaluation metrics for this implementation.

## How to Run
1. Download the Python source file.
2. Open Google Colab or Jupyter Notebook.
3. Run the source code with an internet connection to access the dataset.
4. Review the generated graphs, evaluation tables, and cluster labels.

## Output Files
The program generates:
- `elbow_method.png`
- `silhouette_scores.png`
- `cluster_visualization.png`
- `kmeans_metrics_by_k.csv`
- `algorithm_comparison.csv`
- `cluster_profiles.csv`
- `customers_with_cluster_labels.csv`

