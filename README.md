# ML2 – Customer Segmentation and Promotion Strategy

## Project Overview

This project was developed for the Machine Learning 2 course at NOVA IMS. The objective was to identify meaningful customer segments using unsupervised learning techniques and propose targeted promotional campaigns based on customer purchasing behaviour.

The project combines customer segmentation using K-Means clustering with association rule mining through the Apriori algorithm to generate actionable business insights.

---

## Project Objectives

- Explore and preprocess customer data.
- Investigate potential outliers using DBSCAN.
- Segment customers using K-Means clustering.
- Evaluate cluster quality and stability.
- Visualize the segmentation using PCA.
- Discover product associations using Apriori.
- Develop segment-specific promotional campaigns.

---

## Methodology

### 1. Exploratory Data Analysis and Preprocessing

- Missing value analysis.
- Feature selection.
- Data standardization using StandardScaler.

### 2. DBSCAN Outlier Analysis

DBSCAN was applied to investigate potential outliers before clustering.

- 1,870 customers (5.66%) were identified as noise points.
- Additional analyses showed that these observations represented legitimate customer behaviours rather than data quality problems.
- Since these customers displayed meaningful spending patterns and purchasing characteristics, they were retained in the final analysis.

### 3. Customer Segmentation

K-Means clustering was selected as the final segmentation approach.

The segmentation solution was evaluated using:

- Silhouette analysis.
- Cluster stability across multiple random initializations.
- Reduced-feature experiments.
- PCA visualization.

The final solution consisted of four customer segments.

### 4. Principal Component Analysis (PCA)

PCA was used exclusively for visualization purposes.

The first two principal components explained approximately 35.1% of the total variance and provided a two-dimensional representation of the customer segments.

### 5. Association Rule Mining

Apriori was used to identify products frequently purchased together.

Association rules were evaluated using:

- Support
- Confidence
- Lift

These rules were translated into practical promotional campaigns.

---

## Customer Segments

### Cluster 0 – Occasional Traditional Customers

Lower-value customers with lower engagement levels. Promotions should focus on increasing basket size and purchase frequency.

### Cluster 1 – Loyal High-Value Customers

Highly valuable and loyal customers characterized by broader purchasing behaviour and higher spending levels.

### Cluster 2 – Family-Oriented Customers

Customers exhibiting stronger household purchasing patterns and grocery-oriented behaviour.

### Cluster 3 – Specialised Customers

Customers showing niche spending behaviours and responding well to personalized promotional strategies.

---

## Example Promotional Campaigns

- Buy Eggs and Cereals together and receive an extra discount.
- Purchase Bluetooth Headphones and receive a discount on AirPods.
- Family Breakfast Bundle: Fresh Bread + Cereals promotion.
- Healthy Basket Campaign: Discount on Asparagus when purchasing Tomatoes.

---

## Repository Structure

ML2-Customer-Segmentation/

├── data/

├── notebooks/

│ └── Customer_Segmentation.ipynb

├── outputs/

│ └── customer_clusters.csv

├── report/

│ └── Executive_Report.pdf

├── README.md

└── LICENSE

---

## Deliverables

- Executive Report (PDF)
- Jupyter Notebook (.ipynb)
- Customer cluster assignment CSV
- GitHub repository containing all project materials

---

## Author

Saif Hoque
20241418

Machine Learning 2 – NOVA IMS