

## Clustering Analysis for Outbound Inventory Data

**Project Overview**

This project performs clustering analysis on outbound inventory data. It aims to discover patterns and groupings within the data to gain insights into the distribution of products, their attributes, and outbound behavior. The project utilizes various techniques such as K-means clustering, Agglomerative clustering, and Principal Component Analysis (PCA) to explore the data.

The project is designed for data analysts, supply chain managers, and professionals who work with outbound inventory data. It provides a systematic approach to analyze and understand the relationships between different variables and identify distinct clusters or segments within the dataset. The insights obtained from the clustering analysis can be used to optimize inventory management strategies, improve supply chain efficiency, and make data-driven decisions related to outbound operations.





## Usage/Examples

```python
import pandas as pd

in_vehicle_coupon = pd.read_csv("in-vehicle-coupon-recommendation.csv")

in_vehicle_coupon
```




## Author

- [@chrisinyama](https://github.com/chrisinyama/In-Vehicle-Coupon-Recommendation-Analysis)




## Tools
Jupyter Notebook

## Libraries used 

numpy

pandas

matplotlib.pyplot

seaborn

sklearn.impute.SimpleImputer

sklearn.preprocessing.StandardScaler

sklearn.cluster.KMeans

sklearn.cluster.AgglomerativeClustering

sklearn.decomposition.PCA

scipy.cluster.hierarchy.dendrogram

scipy.cluster.hierarchy.linkage

sklearn.metrics.silhouette_score
## Data preparation/Cleaning/Exploration
1. Data Loading/Import: The project involves loading the dataset and  importing the necessary libraries for data analysis

2. Data Reading: The project reads the stock-keeping data from a CSV file named "Sku_Data.csv" using Pandas


3. Data Inspection: The project inspects the imported data by displaying the first few rows of the dataset to understand its structure and contents

4. Data Cleaning: checks for duplicated rows and missing values in the dataset. It reports that there are no duplicated rows and no missing values in any of the columns

5. Summary Statistics: The project computes and displays summary statistics of the dataset, including measures such as mean, standard deviation, minimum, maximum, and quartiles for the numerical columns



## Data Preprocessing

The following data preprocessing tasks were performed:

a. Handling missing values: The "SimpleImputer" class from scikit-learn was imported, indicating that missing values might have been addressed using some imputation strategy.

b. Feature scaling: The "StandardScaler" class from scikit-learn was imported, suggesting that the features  have been standardized to have zero mean and unit variance.
## Data Visualization
This project incorporates diverse visualization methods, including pairplots, boxplots, histograms, and dendrograms, effectively illustrating the key characteristics and patterns within the stock-keeping data.
## Results/Findings

**Comparison of both clustering algorithms**:

The K-Means clustering analysis suggests 4 clusters as optimal using the Elbow Method and silhouette scores.
Hierarchical Clustering indicates 5 clusters.
Hierarchical Clustering shows more cohesive clusters with less overlap compared to K-Means.
The choice between 4 or 5 clusters depends on prioritizing within-cluster variance or data hierarchy.

**Discussion**:

K-Means suggests a more defined segmentation at four clusters.
Hierarchical Clustering indicates five clusters for deeper group understanding.
These findings are pivotal for SKU categorization and optimizing inventory management.
The results significantly impact inventory managers, enabling optimized stock levels and improved forecasting.
Limitations include the inherent assumptions of the algorithms and reliance on data quality.

**Conclusion**:

Both K-Means and Hierarchical Clustering offer valuable insights into the SKU data.
K-Means provides a simpler approach, while Hierarchical Clustering delves into more complex data structures.
The analysis suggests a choice between 4 or 5 clusters based on the method.
The effectiveness of these algorithms in inventory management depends on their specific application.
A combined approach could offer the most comprehensive insights for effective SKU management.
Integrating these findings into inventory systems promises significant operational advancements.
The practicality of K-Means algorithm:

K-Means algorithm is straightforward to implement and interpret.
It is a practical tool for inventory managers who may not have advanced data science expertise.
The number of clusters (K) can be tuned to meet specific inventory management strategies, such as grouping SKUs by sales velocity, variability, or other relevant metrics.
## Recommendations
**Based on the  analysis, We recommend the following actions**:

a. it is recommended to consider using both K-Means and Hierarchical Clustering algorithms in SKU categorization and inventory management. The combination of these approaches can provide more comprehensive insights into the data and enable better decision-making.

b. Ensure the quality and reliability of the data used for clustering. Data inaccuracies or inconsistencies can significantly impact the clustering results and subsequent inventory management decisions. Implement data validation and cleansing processes to improve the accuracy of the clustering analysis.

c. Regularly review and update the clustering results as the inventory and business dynamics change. Clustering is not a one-time process, and it should be periodically reassessed to reflect the evolving nature of the SKU data and inventory management needs.
## Limitations

One common limitation I encountered was the availability and quality of data
## Installation
**To reproduce the analysis, follow these steps**:

Ensure that the necessary libraries are installed.

Download the Jupyter Notebook and the CSV file.

Run the Jupyter Notebook and execute the code cells to perform the analysis.

    
## Acknowledgements

 The stock-keeping data used in this project is sourced from [https://archive.ics.uci.edu/dataset/531/stock+keeping+units].


