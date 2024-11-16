# Business Owner Clustering using K-Means
This project aims to identify and analyze different clusters of business owners based on data from the Survey of Consumer Finances (SCF) by the U.S. Federal Reserve. Using K-Means clustering, the goal is to group business owners into distinct clusters based on various financial and demographic features. The project includes two main components: a data analysis and model-building Jupyter Notebook, and an interactive user-friendly dashboard for data visualization and exploration.

## Objective
To perform K-Means clustering on a subset of features from the SCF survey data to segment business owners into distinct groups. The clustering helps to understand the characteristics and financial behaviors of different categories of business owners.

### Key Steps:
* Data Preprocessing: Cleaned and prepared the SCF survey data, focusing on selecting features with the highest variance for clustering.
* Feature Selection: Identified the most relevant features for clustering using variance-based selection.
* Model Building: Applied the K-Means algorithm to cluster business owners into different segments.
* Visualization: Analyzed the clusters using visual tools such as scatter plots and summary statistics to understand the characteristics of each cluster.
* PCA for Visualization: Applied Principal Component Analysis (PCA) for dimensionality reduction, allowing for a 2D scatter plot visualization of the clustering results. PCA helps to reduce the complexity of the 
  data while retaining the most important features for visual analysis.
* Interactive Dashboard: Developed a user-friendly dashboard to explore the results of the clustering interactively.

### Requirements
Before running the notebooks, ensure that you have the following dependencies installed:

* pandas (for data manipulation)
* numpy (for numerical operations)
* matplotlib & seaborn (for visualization)
* scikit-learn (for K-Means clustering)
* plotly (for interactive plots)
* dash (for the dashboard)

You can install the required libraries using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn plotly dash
```
## Getting Started
1. Clone the Repository
To get started with the project, clone this repository to your local machine:

```bash
git clone https://github.com/samriddhinechali1/Color-Extraction-Tool.git
```
2. Explore the Jupyter Notebooks
**Data Analysis and Model Building:**
* Open and run the business_owner_clustering.ipynb notebook.
* Review the data cleaning, feature selection, and clustering model steps.
* You can explore the various visualizations and metrics used to assess the performance of the clustering, including PCA scatter plots.
**Interactive Dashboard:**
* Open and run the interactive_dashboard.ipynb notebook.
* The dashboard allows you to visualize the clustering results dynamically and interact with the different segments of business owners.
3. Interactive Features:
* **Bar Chart of High Variance Features:**
Visualize the features with the highest variance, which are the most significant for clustering.

* **Trimmed vs. Non-Trimmed Data:**
Toggle between trimmed and non-trimmed versions of the dataset using a Radio Button. This affects how the data is processed before clustering.

* **Adjustable Number of Clusters:**
Use the K-Means Slider to adjust the number of clusters (k) for the K-Means algorithm, ranging from 2 to 10. The clustering model and visualizations update dynamically as you change the value of k.

* **Model Metrics:**
The dashboard displays two key metrics for evaluating the K-Means clustering model:

* **Inertia:** Measures the sum of squared distances between data points and their respective cluster centers. Lower inertia indicates better clustering.
* **Silhouette Score:** Assesses the quality of the clusters, with higher scores (closer to 1) indicating well-defined, distinct clusters.

* **PCA Scatter Plot:**
Visualize the clustering results in a 2D scatter plot using Principal Component Analysis (PCA). This allows you to explore how the data points are distributed across the first two principal components and how clusters are formed in the reduced space.
## Results
The K-Means clustering model generate 3 distinct clusters, each representing a distinct group of business owners based on the highest variant features in the dataset. These clusters can provide valuable insights into how different types of business owners behave financially, which can be useful for targeted marketing, policy-making, or further research.

By applying PCA, the clustering results are visualized in two dimensions, making it easier to interpret and analyze the relationships between different clusters.
## Conclusion
By using unsupervised machine learning (K-Means) and dimensionality reduction (PCA), this project uncovers underlying patterns in the financial behaviors of business owners. The interactive dashboard makes it easy for users to explore and understand the results of the clustering analysis.
