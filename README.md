# Mall-Customer-Segmentation-Data
Mall Customers Clustering with K-Mean
Project Overview
This project demonstrates the application of unsupervised machine learning techniques to segment mall customers into meaningful groups using the Mall_Customers datase.
The objective is to identify customer segments based on purchasing behavior to enable targeted marketing strategies.

The workflow encompasses clustering from exploratory data analysis to advanced evaluation, including:
* Data preprocessing and scaling
* Exploratory Data Analysis (EDA)
* K-Means clustering
* Determination of optimal cluster number using Elbow Method and Silhouette Score
* Cluster visualization using Principal Component Analysis (PCA)
* Evaluation of clustering quality using multiple metrics
* Comparison with alternative clustering algorithms such as MiniBatch K-Means, DBSCAN, and Agglomerative Clustering

Dataset
* File: `Mall_Customers.csv`
* Columns:
  * `CustomerID` – unique identifier
  * `Gender`
  * `Age`
  * `Annual Income (k$)`
  * `Spending Score (1-100)`
For clustering analysis, the focus was on Age, Annual Income, and Spending Score.


Tools and Libraries
* Python 3.x
* Jupyter Notebook

Python Libraries:
* `pandas` and `numpy` – data handling and numerical operations
* `matplotlib` and `seaborn` – visualization
* `scikit-learn` – clustering algorithms and evaluation metrics
* `scipy` – hierarchical clustering

Project overview
1. Data Preprocessing
* Cleaned the dataset by removing unused columns, such as `CustomerID`
* Scaled numeric features using `StandardScaler` for better clustering performance

2. Exploratory Data Analysis
* Examined feature distributions for Age, Annual Income, and Spending Score
* Generated correlation heatmaps to understand relationships between variables

3. K-Means Clustering
* Applied K-Means algorithm with various values of `k`
* Determined the optimal number of clusters using the **Elbow Method** and **Silhouette Score**
* Visualized clusters in a two-dimensional space after PCA dimensionality reduction

4. Cluster Evaluation
* Measured clustering quality using:
  * Silhouette Score
  * Calinski-Harabasz Index
  * Davies-Bouldin Index
    
5. Comparison with Other Algorithms
* MiniBatch K-Means – efficient clustering for larger datasets
* Agglomerative Clustering – hierarchical clustering analysis
* DBSCAN – density-based clustering to handle irregular cluster shapes

Results and Insights
* Optimal number of clusters identified: 
* Customer segments identified include:
  * High income, high spenders
  * High income, low spenders
  * Young moderate spenders
  * Budget-conscious customers
  * Average customers
* K-Means provided clearly separated clusters, while DBSCAN showed sensitivity to parameter selection.

Learning Outcomes
* Gained a practical understanding of unsupervised learning and clustering
* Learned how to evaluate cluster quality using multiple metrics
* Compared performance across different clustering algorithms
* Applied hands-on skills in EDA, PCA-based visualization, and clustering evaluation

Conclusion
In this project, we successfully applied **K-Means clustering** to the Mall Customers dataset to segment customers based on their age, income, and spending patterns. The analysis revealed distinct customer groups, providing actionable insights for targeted marketing and business strategy.
The workflow demonstrated the importance of **data preprocessing, exploratory analysis, and cluster evaluation** in unsupervised learning. Comparing multiple clustering algorithms highlighted the strengths and limitations of each approach, reinforcing the value of selecting the right method for the dataset characteristics.
Overall, this project provided hands-on experience in customer segmentation and showcased how machine learning can uncover meaningful patterns in real-world data, laying the groundwork for more advanced clustering techniques and interactive analytics in future work.
