# 🏦 EDA Project and Customer Segmentation in Bank


![Bank](https://tse2.mm.bing.net/th/id/OIP.vdcDMKwke20rx-F7_CWcIQHaEK?pid=Api&P=0&h=220)


## 📝 Overview

This project explores recent customer account data to segment clients into key groups. The goal is to help the bank improve targeting strategies and enhance risk assessment by identifying distinct customer profiles.

## 🗂️ Dataset

The dataset “data_retail.csv” contains information about customer transactions from a retail
bank. It includes **1,048,556** rows of data and the following **9 variables**.

After EDA and preprocessing, the new dataset created contains over **884,256** customer transaction records across **15 variables**. This refined dataset is used in the next step for customer segmentation.

## 🛠️ Project Structure

1. **Exploratory Data Analysis (EDA)**:

* Assessed dataset structure, variable distributions, and descriptive statistics.

* Evaluated and handled missing data using appropriate imputation strategies.

* Detected outliers and high-cardinality categorical features.

Feature Engineering:

* Created new behavioral features (recency, frequency, monetary value, balance stability, transaction patterns).

* Derived time-based variables (transaction hour, month phase) and grouped location data.

* Standardized and transformed features to prepare for modeling.

The step will focus on issues such as **data cleaning**, **visualization and exploration** and they will mostly be done using Pandas, Seaborn, Matplotlib and Plotly libraries. 

2. **Segmentation Modeling**:

- Applied K-Means clustering to identify customer segments.

- Determined the optimal number of clusters using both the Elbow Method and Silhouette Analysis.

- Visualized clusters using PCA for dimensionality reduction.

## 🔍 Segmentation Result

After evaluating two methods, the optimal K value was determined to be **4**. Customers were segmented into **four groups** with **distinct characteristics and behaviors**, each suggesting different levels of risk and requiring the bank to develop appropriate strategies for management and engagement.

## 🎯 Business Insights

Based on the K-Means segmentation with 4 clusters, the following strategies are recommended to tailor products, marketing, and risk management for each segment:

**Cluster 0 — Mainstream Low-Balance Customers**

- Focus on onboarding and reactivation initiatives. Recommend micro-savings accounts, simple banking products, and educational content on building financial security. 

- This segment shows high risk due to low balances and limited engagement.

**Cluster 1 — Mature Mid-Balance Customers**

- Prioritize engagement and cross-selling strategies. Offer retirement planning support, insurance products, and loyalty programs to encourage retention. 

- Risk is low to moderate, with steady balances.

**Cluster 2 — High-Balance, High-Variance Customers**

- Emphasize premium retention and proactive monitoring. Provide dedicated relationship management, wealth advisory services, and exclusive investment opportunities. 

- This group is low risk but requires close oversight due to large balance fluctuations.

**Cluster 3 — Mid-Balance but Volatile Customers**

- Drive growth and stabilization with targeted financial planning and risk-adjusted credit offers. Recommend flexible credit products, transaction monitoring tools, and incentives for consistent balances. 

- Risk is moderate, with potential for significant value capture.