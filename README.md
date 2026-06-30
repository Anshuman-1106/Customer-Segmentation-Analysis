# Marketing Analytics: Customer Segmentation

A complete end-to-end Marketing Analytics project that applies Exploratory Data Analysis (EDA), Feature Engineering, and K-Means Clustering to identify meaningful customer segments and provide actionable marketing recommendations.

📌 Project Overview

Customer segmentation helps businesses understand different groups of customers based on their characteristics and purchasing behavior. By identifying these segments, companies can create personalized marketing campaigns, improve customer retention, and maximize revenue.

In this project, customer data is analyzed to:

Clean and prepare the dataset
Perform exploratory data analysis (EDA)
Engineer new customer features
Build customer segments using K-Means clustering
Interpret the resulting clusters
Recommend targeted marketing strategies for each segment
🎯 Objectives
Explore customer demographics and purchasing behavior.
Identify the key factors influencing total customer spending.
Segment customers using an unsupervised machine learning approach.
Provide business-focused marketing recommendations based on customer segments.
📂 Dataset

The dataset contains 2,205 customer records with 39 features, including:

Customer Information
Age
Income
Marital Status
Education
Number of Children
Purchase Behavior
Total Spending
Spending on Wines
Meat Products
Fruits
Fish Products
Sweet Products
Gold Products
Purchase Channels
Web Purchases
Store Purchases
Catalog Purchases
Discount Purchases
Marketing Information
Campaign Acceptance
Response to Marketing Campaigns
Customer Complaints
Customer Tenure
Recency of Purchase
🛠️ Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
SciPy
📊 Project Workflow
1. Data Preparation
Loaded dataset
Checked missing values
Verified data types
Removed constant columns
Removed spending outliers
2. Exploratory Data Analysis (EDA)

Performed analysis on:

Spending distribution
Income distribution
Age distribution
Correlation analysis
Point-Biserial correlation for binary variables

Visualizations include:

Histograms
Boxplots
Heatmaps
Scatterplots
Bar charts
3. Feature Engineering

Created two new features:

Marital – Human-readable marital status
In_relationship – Binary feature indicating whether a customer is married or living with a partner
4. Customer Segmentation

Features used for clustering:

Income
Total Spending (MntTotal)
In_relationship

Steps:

Standardized data using StandardScaler
Applied Principal Component Analysis (PCA) for visualization
Determined optimal number of clusters using:
Elbow Method
Silhouette Score
Built K-Means clustering model
📈 Results

The optimal number of clusters was 4.

Cluster 0 – Low-Value Customers in Relationships
Largest customer group
Lower income
Lower spending
Family-oriented customers
Cluster 1 – Low-Value Single Customers
Lower income
Lower spending
Single customers
Cluster 2 – High-Value Customers in Relationships
High income
High spending
Strong purchasing power
Significant spending on premium products
Cluster 3 – High-Value Single Customers
High income
High spending
Premium customers
Similar purchasing behavior to Cluster 2 but single
💡 Business Recommendations
Cluster 0
Family discount campaigns
Bundle offers
Seasonal promotions
Cluster 1
Coupons and discounts
Loyalty rewards
Personalized email campaigns
Cluster 2
Premium product recommendations
Exclusive wine promotions
VIP loyalty programs
Cluster 3
Luxury product campaigns
Lifestyle-focused marketing
Personalized premium offers
📊 Key Insights
Income has the strongest positive relationship with customer spending.
Customers with children generally spend less overall.
Marital status alone has little impact on spending.
High-income customers purchase significantly more premium products.
Four distinct customer segments were identified using K-Means clustering.
