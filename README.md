# 🛒 SmartCart Customer Segmentation System

> **Unsupervised Machine Learning | Customer Analytics | E-Commerce Intelligence**

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-blue)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
a
---

## 📌 Problem Statement

**SmartCart** is a growing e-commerce platform serving customers across multiple countries. The company collected data from **2,240 customers** across **22 attributes** — covering demographics, purchase behaviour, website activity, and campaign responses.

**The Challenge:**
- SmartCart was using a single, generic marketing strategy for all customers
- This led to **inefficient marketing spend**, missed retention opportunities, and delayed identification of churn-prone users

**The Solution:**
Build an **intelligent customer segmentation system** using **unsupervised machine learning** to group customers into meaningful clusters based on their purchasing behaviour, engagement levels, and loyalty indicators — enabling **data-driven, personalised marketing**.

---

## 🎯 Objectives

- Analyse historical customer transaction data to discover hidden behavioural patterns
- Segment customers into distinct groups using clustering algorithms
- Provide actionable insights to support personalised marketing and customer retention strategies
- Identify high-value customers, at-risk customers, and disengaged segments

---

## 📊 Dataset Overview

| Category | Features |
|---|---|
| **Customer Demographics** | ID, Year_Birth, Education, Marital_Status, Income, Kidhome, Teenhome, Dt_Customer |
| **Spending Behaviour** | MntWines, MntFruits, MntMeatProducts, MntFishProducts, MntSweetProducts, MntGoldProds |
| **Purchase Frequency** | NumDealsPurchases, NumWebPurchases, NumCatalogPurchases, NumStorePurchases, NumWebVisitsMonth |
| **Feedback & Recency** | Recency, Complain |

**Dataset Size:** 2,240 records × 22 features

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| `Python 3.8+` | Core programming language |
| `Pandas` | Data loading, cleaning, and manipulation |
| `NumPy` | Numerical computations |
| `Scikit-learn` | K-Means clustering, PCA, preprocessing |
| `Matplotlib` | Data visualization |
| `Seaborn` | Statistical plots and heatmaps |
| `Jupyter Notebook` | Interactive development and presentation |

---

## 🔄 Project Workflow

```
Raw Data
   │
   ▼
Exploratory Data Analysis (EDA)
   │  - Distribution analysis
   │  - Correlation heatmaps
   │  - Missing value detection
   ▼
Feature Engineering
   │  - Customer age from Year_Birth
   │  - Total spend across all categories
   │  - Campaign response score
   │  - Outlier treatment
   ▼
Data Preprocessing
   │  - Standard scaling
   │  - Label encoding
   ▼
Dimensionality Reduction (PCA)
   │  - Reduce to 2–3 principal components
   │  - Retain maximum variance
   ▼
K-Means Clustering
   │  - Elbow method to find optimal K
   │  - Silhouette score evaluation
   ▼
Cluster Analysis & Visualisation
   │  - Spending profiles per cluster
   │  - Demographic breakdown
   │  - Engagement patterns
   ▼
Business Insights & Recommendations
```

---

## 📈 Key Features

- **End-to-End ML Pipeline:** From raw data ingestion to actionable cluster insights
- **Feature Engineering:** Created derived features including `Age`, `Total_Spend`, `Children`, and `Campaign_Response`
- **Optimal Cluster Selection:** Used Elbow Method and Silhouette Score to determine the best number of clusters
- **PCA Visualisation:** Reduced dimensionality for clear 2D cluster visualization
- **Business-Oriented Output:** Each cluster is profiled with marketing recommendations

---

## 📂 Project Structure

```
SmartCart-Clustering/
│
├── data/
│   └── marketing_campaign.csv        # Raw dataset
│
├── notebooks/
│   └── smartcart.ipynb               # Main analysis notebook
│
├── outputs/
│   ├── cluster_profiles.png          # Cluster spending heatmap
│   ├── pca_clusters.png              # PCA 2D cluster plot
│   └── elbow_curve.png               # Optimal K selection
│
├── requirements.txt                  # Python dependencies
└── README.md                         # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

```bash
Python 3.8+
Jupyter Notebook
```

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/SmartCart-Clustering.git
cd SmartCart-Clustering

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook notebooks/smartcart.ipynb
```

### Requirements

```txt
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyter
```

---

## 💡 Business Insights

After clustering, customers are grouped into distinct segments such as:

| Segment | Profile | Strategy |
|---|---|---|
| **High-Value Loyalists** | High spenders, frequent buyers, high income | Loyalty rewards, premium offers |
| **At-Risk Customers** | Previously active, declining engagement | Re-engagement campaigns, discounts |
| **Budget Shoppers** | Deal-driven, low spend, high web visits | Targeted discount offers |
| **New / Inactive Users** | Low recency, minimal transactions | Onboarding nudges, introductory offers |

---

## 📝 Results

- Successfully segmented 2,240 customers into **distinct behavioural clusters**
- Achieved strong cluster separation confirmed by **Silhouette Score**
- Identified spending patterns across wine, meat, fish, fruits, and gold product categories
- Provided cluster-level profiles ready for direct use by marketing and CRM teams

---


> *Built as part of an AI/ML project to demonstrate real-world unsupervised learning and customer analytics skills.*
